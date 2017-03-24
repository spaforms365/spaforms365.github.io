---
title: Quick-start guide
permalink: /docs/quickstart/
---



## Ensure SPA Forms 365 Add-in is available

~SPA Forms 365 app must be added on SharePoint site before use with lists. To check if the app is available, go to <code>Site Contents</code> page on SharePoint site and verify that <code>SPA FORMS 365</code> app present. If you don't see the ![Image of AddIn](/img/logo-2x.png) app at Site Contents page, then follow [Installation](/docs/installation) instructions to deploy the app.

## Provision and configure SharePoint List

~ Create new out-of-box custom or tasks list on your SharePoint web site. You may also use existing list and/or develop your list further at this time: add custom columns, etc. 

<div class="note warning">
  <h5>Note regarding SharePoint lists hosted on Office 365</h5>
  <p>
    SPA Forms 365 UI requires ribbon feature enabled on SharePoint List. In the meantime ribbon is not available by default on newly provisioned lists at Office 365. You must explicitly enable ribbon on list with SPA Forms 365.
  </p>
  <p>
    Open <code>Settings</code> page on your list and select <code>Advanced Settings</code> section. Scroll to the bottom of page and switch your list into <code>Classic experience</code>.
  </p>
</div>

~ Provision SPA Forms 365 on your list. Open <code>LIST</code> tab on ribbon at your SharePoint list. Locate and press <code>SPA Forms 365</code> button to open SPA Forms 365 Installer dialog. Press <code>INSTALL</code> button to activate product instance on your list.
<br/>
<br/>
![Image of Installer](/img/SPSForms365Installer1.PNG)

## Design and Publish custom SPA Form

~ Unlike out-of-box SharePoint list forms, custom SPA Form must be designed and published before first use with list data. Click on SharePoint list's <code>new item</code> menu item and SPA Forms runtime will reply with warning message, that published SPA project was not found. Click on <code>Open Form Design project</code> link to open SPA Form designer.
<br/>
<br/>
![Image of Design1](/img/SPAForms365Design1.png)
<br/>
~ SPA Forms designer will show simple custom default form as a starting point for further project development. Default custom form project has one field for out-of-box Title column and standard buttons on form.
<div class="note">
  <h5>ProTip™: Quick initial design for new form project</h5>
  <p>
    SPA Forms designer can help quickly initialize newly created SPA project. There are options to start with <code>Empty Layout</code>, <code>Layout with all SharePoint List Columns</code> or <code>Layout imported from GitHub</code> initial designs.
    You should really
    <a href="../templates/#code-snippet-highlighting">check out how to
    do that</a> before you go any further.
  </p>
</div>
~ For quick start we won't proceed with any design modifications and will just publish SPA form project 'as-is' into production. Press on <code>Publish</code> button on ribbon to open <code>Form Project</code> panel and next click on <code>Publish</code> button on the panel.
<br/>
<br/>
![Image of Publishing](/img/form-publish.png)
<br/> 
<br/>
~ Wait until SPA Forms designer will publish SPA form project into single minified runtime module and press <code>Close</code> button to collapse panel. Next press <code>Close</code> button on ribbon to exit SPA Forms designer.
<br/>
<br/>
![Image of Published](/img/form-published.png)

## Good to go now: try new custom SPA Form

Click <code>new item</code> on SharePoint list and published custom SPA Form shell open now.


## Next steps

Building a Jekyll site with the default theme is just the first step. The real magic happens when you start creating blog posts, using the front matter to control templates and layouts, and taking advantage of all the awesome configuration options Jekyll makes available.
