+++
author = "Loris Scandurra"
title = 'Printer deployment with Group Policy Preferences and error 0x80070bcb'
date = "2020-08-10"
description = 'Solving 0x80070bcb error when deploying printers with GPO'
disableComments = true
+++

**TL;DR**

If you get the error 0x80070bcb when deploying your printers follow the instructions below.  
Enable and configure these two GPO's for all clients you want to deploy the printers to:

> Computer Configuration > Policies > Administrative Templates > Printers > Package Point and print - Approved servers`

> Computer Configuration > Policies > Administrative Templates > Printers > Point and Print Restrictions`

Configure them as follows:

In the Policy `Package Point and print - Approved servers` I had to add the FQDN of the print server.

For the Policy `Point and Print Restrictions` I had to check the checkbox `Users can only point and print to these servers` and add the FQDN of the print server. The security prompts I configured as follow:

`When installing drivers for a new connection: Do not show warning or elevation prompt`

`When updating drivers for an existing connection: Show warning only`

---

This week we migrated an old print server from Windows Server 2008 R2 to Windows Server 2019. And we changed the way we deployed printers. Before the change, the user had to select the printer by himself, and there was no automatic deployment. So every employee who wanted a printer gad to go to the printer settings and added the printer. This implementation resulted in many calls to the IT office because the user doesn't know the nearest printer's name. So to avoid this situation, we decided to deploy printers using Group Policy Preferences (GPP). GPP's are like regular Group Policy Objects (GPO), and you can configure the same way. To learn more about the differences, I recommend this [article](https://docs.microsoft.com/en-us/previous-versions/windows/it-pro/windows-server-2012-r2-and-2012/dn581922(v=ws.11)).

After configuring the deployment for all printers, most deployed successfully, but a few printers seem to have difficulties. When I wanted to see the GPO result with the command `gpresult`, I saw the error 0x80070bcb with all printers that didn't successfully deploy. This problem seems to be a Windows 10 User Account Control (UAC) problem that exists since Windows Vista.  
To resolve this error, I had to enable and configure the two following GPO's for all Computers that I wanted to deploy the printers too.

> Computer Configuration > Policies > Administrative Templates > Printers > Package Point and print - Approved servers

> Computer Configuration > Policies > Administrative Templates > Printers > Point and Print Restrictions

In the Policy `Package Point and print - Approved servers` I had to add the FQDN of the print server.

For the Policy `Point and Print Restrictions` I had to check the checkbox `Users can only point and print to these servers` and add the FQDN of the print server. 

The security prompts I configured as follow:

`When installing drivers for a new connection: Do not show warning or elevation prompt`

`When updating drivers for an existing connection: Show warning only`

After having configured these two GPO's, I forced a GPO update with `gpupdate /force`, and the printers that didn't appear before appeared now with no errors.

**Acknowledgment:**  
Thanks a lot to this article that directed me in the right direction: [https://www.adamfowlerit.com/2017/07/deploying-printers-windows-10](https://www.adamfowlerit.com/2017/07/deploying-printers-windows-10)