---
title: Quick-start guide
permalink: /docs/quickstart/
---



## Ensure SPA Forms 365 Add-in is available

~SPA Forms 365 app must be added on SharePoint site before use with lists. To check if the app is available, go to <code>Site Contents</code> page on SharePoint site and verify that <code>SPA FORMS 365</code> app present. If you don't see the ![Image of AddIn](/img/365x32x32.PNG) app at Site Contents page, then follow [Installation](/docs/installation) instructions to deploy the app.

## Provision and configure SharePoint List

~ Create new out-of-box custom or tasks list on your SharePoint web site. You may also use existing list and/or develop your list further at this time: add custom columns, etc. 

<div class="note warning">
  <h5>For lists provisioned on Office 365</h5>
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


## Next steps

Building a Jekyll site with the default theme is just the first step. The real magic happens when you start creating blog posts, using the front matter to control templates and layouts, and taking advantage of all the awesome configuration options Jekyll makes available.
