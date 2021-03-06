---
title: Installation
permalink: /docs/installation/
---

Full installation process for SPA Forms 365 Add-in is related to 3 various areas on SharePoint landscape:
* [Step 1:](#step1) Upload software distributive file <code>spaforms365.app</code> into <code>SharePoint Apps Catalog</code>. Normally this step is executed by SharePoint tenant or farm administrator to enable access to <code>SPA Forms 365 Installer App</code> for all other users.  
* [Step 2:](#step2) Add <code>SPA Forms 365 Installer App</code> on desired <code>SharePoint Web Site</code>. The Installer App should reside on web site, where target SharePoint List is located. The Installer App enables activation or removal of SPA Forms instances on any number of SharePoint Lists residing at the web site. Normally SharePoint user with Full Control level of access on web site can add Installer App on web site.  
* [Step 3:](#step3) Activate <code>SPA Forms feature</code> on desired <code>SharePoint List</code>. To substitute out-of-box forms with SPA Form on SharePoint list, an instance of SPA Forms application should be activated on that list. A SharePoint user with Design level of access or higher can activate or deactivate SPA Forms instances. 

### Requirements & Compatibility

* SharePoint: SPA Forms 365 software has been tested to run with on-premise versions of <code>SharePoint 2013 & 2016</code> and with <code>SharePoint Online on Office 365<code>.
* Web Browsers: SPA Forms 365 software has been tested for compatibility with <code>Google Chrome</code> and <code>Microsoft IE-11</code>. 

### Step 1: Apps Catalog {#step1}
In order to upload SPA Forms 365 distributive file <code>spaforms365.app</code> into <code>SharePoint Apps Catalog</code>, SharePoint Administartor need to choose and follow one of a few various procedures, depends on target SharePoint environment:
* <b>Office Apps Catalog:</b> No action needed: planned to be placed in a nearest future. 
* <b>App Catalog at SharePoint Online:</b> download software distributive file [spaforms365.app](https://github.com/spaforms365/addin/releases/download/1.0.7.3/SPAFORMS365.zip) and follow guidelines outlined at [Microsoft Office Support Article](https://support.office.com/en-us/article/Use-the-App-Catalog-to-make-custom-business-apps-available-for-your-SharePoint-Online-environment-0b6ab336-8b83-423f-a06b-bcc52861cba0){:target="_blank"} to upload distributive file to the App Catalog.
* <b>App Catalog at on premise SharePoint Farm:</b> download software distributive file [spaforms365.app](https://github.com/spaforms365/addin/releases/download/1.0.7.3/SPAFORMS365.zip) and follow guidelines outlined at [Microsoft Technet Article](https://technet.microsoft.com/en-us/library/fp161234.aspx#AddApps){:target="_blank"} to upload distributive file to the App Catalog.

### Step 2: Add SPA Forms 365 Installer App on SharePoint Site {#step2}
SPA Forms 365 Installer App must be added on <code>SharePoint Web Site</code> to enable <code>SPA Form feature</code> management on <code>Custom</code> and <code>Tasks</code> Lists. 
LIST tab on Ribbon for any List of these two types, exposes new <code>SPA Forms 365</code> button, provided by installed SPA Forms Installer App.
<br/>
<br/>
![Image of Add Installer](/img/form-addinstaller.png)
<div class="note info">
  <h5> No need to keep Installer App on Site all the time</h5>
  <p>
    <code>SPA Forms Installer App</code> is needed only at a time of <code>SPA Forms feature</code> activation or removal. 
    Being activated, <code>instance of SPA Forms feature</code> on SharePoint list is self-sufficient and independent. 
  </p>
  <p>
    You may safely remove SPA Forms Installer App off the SharePoint Site at any time. As a result the <code>SPA Forms 365</code> button will not show up on LIST tab on Ribbon at <code>Custom</code> and <code>Tasks</code> lists on site.  
  </p>
</div>
### Step 3: Activate SPA Forms feature on SharePoint List {#step3}
* To activate <code>instance</code> of SPA Forms on SharePoint List: open <code>LIST</code> tab on ribbon at the list and press <code>SPA Forms 365</code> button to open SPA Forms 365 Installer dialog. Press <code>INSTALL</code> button to activate product instance on the list. Upon completion of istallation process you are good to go to start using SPA Forms with the list.
<br/>
![Image of Activate Instance](/img/SPSForms365Installer1.PNG)
<div class="note warning">
  <h5>Only Custom or Tasks Lists are supported for SPA Forms feature.</h5>
  <p>
    Currently only <code>Custom</code> or <code>Tasks</code> SharePoint Lists are compatible with <code>SPA Forms feature</code>. SPA Forms Installer App injects custom <code>SPA Forms 365 button</code> into <code>ribbon</code> for these two list types. 
  </p>
</div>
* To remove <code>instance</code> of SPA Forms off the SharePoint list: open <code>LIST</code> tab on ribbon at the list and press <code>SPA Forms 365</code> button to open SPA Forms 365 Installer dialog. Press <code>REMOVE</code> button to remove product instance off the list. Upon completion of removal process out-of-box forms functionality will be restored on the list.
<br/>
![Image of Remove Instance](/img/form-remove.PNG)
<div class="note">
  <h5>ProTip™: Preserve SPA Form project source code prior SPA Forms removal</h5>
  <p>
    SPA Form instance removal will delete everything: runtime code and any customizations made within source code for SPA Form project. To avoid loss of source code, you may need to preserve custom SPA Form project prior removal and save it into remote GitHub repository.   
  </p>
</div>
<div class="note">
  <h5>ProTip™: SharePoint List deletion use case.</h5>
  <p>
    The whole SharePoint List can be deleted at any time. Such deletion will also effectively remove SPA Forms instance, including source code for SPA Form project. To avoid loss of source code, you may need to preserve custom SPA Form project prior removal and save it into remote GitHub repository. 
  </p>
</div>


#### Now that you’ve got everything up-to-date and installed, let’s get to work!
