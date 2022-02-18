+++
author = "Loris Scandurra"
title = "Exchange 2016 Hybrid setup false password/username"
date = "2020-07-23"
description = "Exchange 2016 Hybrid Setup has a bug that returns a false password/username error even if you copy the correct credentials"
+++

**TL;DR**  
Don't copy and paste the credentials. Type them in manually, and the setup will proceed normally.

---

I am currently doing a general infrastructure update for a customer. During this process, we migrated all Users from Exchange 2010 to Office 365 Mailboxes. But due to how Microsoft (sadly) designed their Office 365 with an On-premise Active Directory environment, you still need a local Exchange Server to manage the Exchange attributes in your On-Prem Active Directory [[read the doc](https://docs.microsoft.com/en-us/exchange/decommission-on-premises-exchange)]. And because we didn't want to leave an old Exchange Server with Windows 2008 R2 running in the network, we decided to install a new Exchange Server.  

You don't need to pay for a new Exchange License for this, because the new Exchange Server will only be a Hybrid Server that doesn't contain any mailboxes itself. So for this, Microsoft provides a Hybrid License for an Exchange Server 2016. After setting up a VM with Windows Server 2016, I started the Exchange installation. The Exchange installation detected a Hybrid setup and asked me to insert the user credentials of an Office 365 Admin. So I did just that, I copied the credentials and pasted them into the setup screen, but it told me that the credentials were wrong. And I knew that couldn't be because I just copied them like I always do. And I also couldn't move forward with the installation without providing the credentials.  

After some research on the Internet, I found the error [[read the forum post](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_outlook/exchange-2016-new-install-hybrid-deployment-check/1bd7bbef-cf48-441c-8989-1644fecea521)]. The problem was that I copy/pasted the credentials. If you do this, the installer will tell you that your credentials are wrong. So I had to copy them manually. After that, the installation proceeded successfully.