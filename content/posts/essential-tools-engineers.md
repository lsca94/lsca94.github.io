+++
author = "Loris Scandurra"
title = "Essential tools for engineers"
date = "2020-06-15"
description = "Some essential tools to make engineers life easier"
+++

In this post, I will list some tools I use daily, explain why I use them, and provide a link to download/use them. I will regularly update this post if I find new tools or when they get discontinued.

## Security

**1Password**  
Great tool for iOS and macOS users to save passwords (it's also available for other platforms). I would strongly suggest using a good password manager and not reuse passwords because the reuse of passwords is a serious security issue! 1Password is a paid tool, but there are also free options on the market like KeePass.  
Link: [1password.com](https://1password.com)

**KeePass**  
KeePass is another password manager. The big advantage of KeePass is that it's opensource and therefore free. It's a great tool that supports all major platforms, but if you want to have your password synchronized between different devices, you have to synchronize the password file yourself (for example, with Google Drive or Dropbox).  
Link: [keepass.info](https://keepass.info)

**ProtonVPN**  
This is an excellent VPN service. It's based in Switzerland (which has robust privacy laws), but it has servers worldwide. Also, it has a clean interface and some excellent features to protect your privacy. ProtonVPN was created from the makers of ProtonMail, which is a privacy-focused mail service. I don't use ProtonMail, but if I wanted to be sure that my mails are stored and transmitted safely, I would use it.  
Link: [protonvpn.com](https://protonvpn.com)

**Have I been pwned**  
Or "Have I been owned" is a website to check if your password/data has been leaked. You can type in your email address on the site, and the website will tell you if your email address was found in any known data leak in their database. If the website tells you that you have been affected, it's recommended to change your password for the affected service, and everywhere you use the same password (I strongly recommend using a password manager and to never reuse passwords).  
Link: [haveibeenpwned.com](https://haveibeenpwned.com)

**Hasso-Platner-Institut**  
Another website to check if your password/data has been leaked. It's basically the same as "Have I been pwned", you type in your email and get a report if your data has been leaked from a known data breach. I found that this tool has a more up to date data breach database, then "Have I been pwned". Nonetheless, I recommend using both tools to check if your data has been leaked.<br>If your data has been leaked, you should change your password for the affected service, and everywhere you use the same password (I strongly recommend using a password manager and never reuse passwords).  
Link: [sec.hpi.de/ilc/](https://sec.hpi.de/ilc/)

## Coding & Engineering

**VisualStudio Code**  
I have to hand it to Microsoft, they managed to create an excellent tool for developers. It is easily expandable through its many plugins, which makes it a superb all-rounder for many developers. I use it mainly for web development, but you can use it for a lot more. It has some great features and a well build IntelliSense that can make you a productive developer.  
Link: [code.visualstudio.com](https://code.visualstudio.com)

**PgAdmin**  
A tool for engineers that work with PostgreSQL database servers. It's a tool you can install on your computer and use it to manage PostgreSQL databases. It gives you a graphical interface instead of a CLI to manage your database, which can be convenient sometimes (especially if you have to look up all CLI/SQL commands, which wastes your time).  
Link: [pgadmin.org](https://www.pgadmin.org)

**Sourcetree**  
Sourcetree is a visual Git client. It's convenient to keep track of all your repositories. Not all Git features are available through the GUI, but it supports more than enough to replace the Git CLI for my daily use.  
Link: [sourcetreeapp.com](https://www.sourcetreeapp.com)

**Postman**  
This tool is useful to quickly test APIs. You can make a different API request and display the returning data in various ways. I like this tool to quickly get the hang of an API, besides using official documentation, I think trial and error is the fastest way to get to know a new API. You can also use it to document your API, but I never tried this feature before.  
Link: [postman.com](https://www.postman.com)

**StarWind V2V Converter**  
The StarWind V2V Converter is a great tool to migrate virtual machines or virtual machine disks. You can convert from Hyper-V Disk to VMware compatible disks. Or migrate a virtual machine from Azure direct to VMware. It's a great and easy tool to migrate VM's between different environments. And it's also free to use.  
Link: [starwindsoftware.com](https://www.starwindsoftware.com)

## Webservices

**Cloudflare**  
Cloudflare is basically an industry-standard CDN and DDoS protection service. And it also features a free tier, which is great for small websites that don't need the more advanced features. There are other CDN and DDoS protection tools on the market, but Cloudflare is definitely leading it. It is also reasonably easy to use and gives you meaningful insights about the traffic you get on your website or service.  
Link: [cloudflare.com](https://www.cloudflare.com)

**iloveimg**  
This is a great tool for images, it's ideal for small changes. If you are too lazy to open up an image editor like Photoshop that takes ages to open, just go to iloveimg.com and make the quick change you wish to make.  
Link: [iloveimg.com](https://www.iloveimg.com)

**ilovepdf**  
If you need to make any kind of changes to a PDF, do not look further. This tool can do almost anything with your PDF: merge, split, compress, convert, edit, watermark, and many more things.  
Link: [ilovepdf.com](https://www.ilovepdf.com)

**forwardemail**  
If you need to forward emails from one address to another without installing a mail server yourself or paying for one, you can use forwardemail. Some DNS nameserver hoster provide this feature out of the box, but there are some (Cloudflare, for example) that don't have this feature. With this web service, you can add this feature at zero cost. There are also more advanced features and paid plans available, but I currently don't use them.  
Link: [forwardemail.net](https://forwardemail.net/en)

**pdfgeneratorapi**  
It's an API that gives you the ability to create different PDF templates and send data to its interface, which then gives you back a filled-out PDF. It's a great tool for people that need many different templates, which change often. It gives you a visual template designer, which makes it possible for your end-users to create their templates themself. Which is a great way to make the developer's workload lighter so that they can focus on more important things than creating PDF templates.  
Link: [pdfgeneratorapi.com](https://pdfgeneratorapi.com)

**waymark.io**  
A simple tool to create Roadmaps and Timelines. It's a great tool to create those Roadmaps you see on every startup's website and presentation.  
Link: [waymark.io](https://waymark.io)

**MXToolBox**  
If you need to do any troubleshooting regarding E-Mail DNS configuration, I would suggest to checkout MXToolBox. MXToolBox offers a wide variety of tools to check E-Mail related DNS entries from MX, SPF, DMARC, and much more. It also provides tools to check if you got on an E-Mail Blacklist and other useful tools like WHOIS lockups.  
Link: [mxtoolbox.com](https://mxtoolbox.com/)

## System Administration

**mRemoteNG**  
Great tool for system administrators. You can do all in one tool instead of having a lot of different tools to connect to different types of servers. With this tool, you can connect to Linux servers, Windows servers, vCenter servers, and many more. It's also customizable, so you can connect to pretty much anything you wish. It keeps all your saved connection in a list, so you don't have to type out the server's names or IP addresses, and to connect, you just double-click the server. It's a great tool if you have new employees, so they don't have to always look for the server names and can just quickly connect on to the servers.  
Link: [mremoteng.org](https://mremoteng.org)

## Collaboration

**Discord**  
I really like discord to keep up with friends. And given the current Coronavirus pandemic situation, this tool was handy to work together in teams. It gives you all the necessary features to work together, it may lack behind Zoom with its features, but I didn't really miss any of its features. It may not be well integrated with other apps like Zoom, but that's because the target audience differs a lot between the two tools.  
Link: [discord.com](https://discord.com)

## MacOS

**Caffeinated**  
A simple tool that prevents your Mac from going into sleep mode. You can control the app through the menu bar. I like its simplicity because it just does the right thing, nothing more, nothing less.  
Link: [Caffeinated](https://apps.apple.com/ch/app/caffeinated-anti-sleep-app/id1362171212?mt=12)

**Pock**  
Don't you know what the touch bar on your MacBook is good for? Well, me neither, but this tool makes it a lot more useful. It gives you more personalization possibilities for your touch bar, like shortcuts for the apps in your dock or controlling your music app. And it doesn't switch its layout based on the app you are using, which is a big plus for me.  
Link: [pock.dev](https://pock.dev)

If I missed any tools you think are useful, write me a comment or send me directly a message, so I can check them out too!</p>