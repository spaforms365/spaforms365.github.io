---
title: Quick-start guide
permalink: /docs/quickstart/
---

As a quick practical introduction into SPA Forms, tet's will walk though a few minutes long training exersize: we will create SPA Form functinally equivalent to out-of-box SharePoint list forms.

## Ensure SPA Forms 365 Add-In is available

Before begin working on exersize, we need to ensure that <code>SPA Forms 365 Installer</code> Add-In is avaliable on SharePoint web site. The <code>Add-In</code> is needed to install SPA Forms 365 feature on top of out-of-box SharePoint list.
<br/>
<br/>
To verify Add-In, go to <code>Site Contents</code> page on your SharePoint site and check that <code>SPA Forms 365 Installer</code> pictogram is present. If you don't see the Add-In pictogram at Site Contents page: 
<br/>
![Image of AddIn](/img/logo-96.png)
<br/>
then please stop at this point and follow [Installation](/docs/installation) instructions to deploy the Add-In.

## Provision and configure SharePoint List

Create new out-of-box <code>Custom</code> or <code>Tasks</code> list on your SharePoint web site. You may also choose existing list and/or extend list with custom columns, etc. 


Provision SPA Forms 365 on your list. Open <code>LIST</code> tab on ribbon at your SharePoint list. Locate and press <code>SPA Forms 365</code> button to open SPA Forms 365 Installer dialog. Press <code>INSTALL</code> button to activate product instance on your list.
<br/>
<br/>
![Image of Installer](/img/SPSForms365Installer1.PNG)
<div class="note warning">
  <h5>Note regarding SharePoint lists hosted on Office 365</h5>
  <p>
    SPA Forms 365 UI requires ribbon feature enabled on SharePoint List. In the meantime SharePoint Online promotes <code>modern</code> UI experience on newly provisioned lists, with no ribbon exposed. List with <code>modern</code> UI provides menu item  on list toolbar to launch <code>SPA Forms 365 Installer</code>. To enable ribbon <code>SPA Forms 365 Installer</code> will forcibly switch SharePoint list into <code>Classic experience</code> during provisioning SPA Forms on the list.
  </p>
</div>

## Design and Publish custom SPA Form

Unlike out-of-box SharePoint list forms, custom SPA Form must be designed and published before first use with list data. Click on SharePoint list's <code>new item</code> menu item and SPA Forms runtime will reply with warning message, that published SPA project was not found. Click on <code>Open Form Design project</code> link to open SPA Form designer.
<br/>
<br/>
![Image of Design1](/img/qs-exersize-1.png)
<br/>
SPA Forms designer will show simple custom default form as a starting point for further project development. Default custom form project has one field for out-of-box Title column and standard buttons on form.
<div class="note">
  <h5>ProTip™: Quick initial design for new form project</h5>
  <p>
    SPA Forms designer can help quickly initialize newly created SPA project. There are options to start with <code>Empty Layout</code>, <code>Layout with all SharePoint List Columns</code> or <code>Layout imported from GitHub</code> initial designs.
    You should really
    <a href="../templates/#code-snippet-highlighting">check out how to
    do that</a> before you go any further.
  </p>
</div>
For quick start we won't proceed with any design modifications and will just publish SPA form project 'as-is' into production. Press on <code>Publish</code> button on ribbon to open <code>Form Project</code> panel and next click on <code>Publish</code> button on the panel.
<br/> 
<br/>
![Image of Published](/img/qs-exersize-2.png)
<div class="note warning">
  <h5>Important Web Browser Compatibility Note:</h5>
  <p>
    You must use modern web browser, like <code>Google Chrome</code>, <code>Microsoft Edge</code> or <code>Firefox</code> to run project publishing. 
    <code>Microsoft IE-11</code> web browser can't support a few SPA Forms 365 UI features, including <code>Project Publishing</code>.
  </p>
</div>
Wait until SPA Forms designer will publish SPA form project into single minified runtime module and press <code>Close</code> button to collapse panel. Next press <code>Close</code> button on ribbon to exit SPA Forms designer.
<br/>
<br/>
![Image of Published](/img/qs-exersize-3.png)

## Good to go now: 

Click <code>new item</code> on SharePoint list and newly published custom SPA Form shell now open.


## Next steps

Building default SPA Form is just the first step. More to add here ...
