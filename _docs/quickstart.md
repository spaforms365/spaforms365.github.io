---
title: Quick-start guide
permalink: /docs/quickstart/
---

To get quick practical introduction into SPA Forms, let's will walk through a few minutes long training exersize, to create <code>custom SPA Form</code>, functionally equivalent to out-of-box SharePoint list forms.

## Ensure SPA Forms 365 Add-In is available

Before begin working on training exersize, we need to ensure that <code>SPA Forms 365 Installer Add-In</code> is avaliable on SharePoint web site. <code>Add-In</code> is neccessary to provision SPA Forms 365 feature on top of out-of-box SharePoint list. 
<table>
  <tr>
    <td>
      <img src="/img/logo-96.png"/>
    </td>
    <td>
      <p>
To verify Add-In, go to <code>Site Contents</code> page on your SharePoint site and check that <code>SPA Forms 365 Installer</code> pictogram is present.  
      </p>
    </td>
  </tr>
</table>
If you don't see the Add-In pictogram at Site Contents page, then please stop at this point and follow [Installation](/docs/installation) instructions to deploy the Add-In.

## Provision and configure SharePoint List

Create new out-of-box <code>Custom</code> or <code>Tasks</code> list on your SharePoint web site. You may also choose existing list and/or extend list with custom columns, etc. 
<br/>
<br/>
Having SharePoint list available, next step is to <code>provision</code> SPA Forms 365 feature on the list, as illustrated on the screenshot below:  
<br/>
![Image of Installer](/img/SPSForms365Installer1.PNG)
<br/>
Open <code>LIST</code> tab on ribbon at SharePoint list. Locate and press <code>SPA Forms 365</code> button to open SPA Forms 365 Installer dialog. Press <code>INSTALL</code> button to activate SPA Form 365 product instance on the list.
<div class="note warning">
  <h5>Note regarding SharePoint lists hosted on Office 365</h5>
  <p>
    SPA Forms 365 UI requires ribbon feature enabled on SharePoint List. In the meantime SharePoint Online promotes <code>modern</code> UI experience on newly provisioned lists, with no ribbon exposed. List with <code>modern</code> UI provides menu item  on list toolbar to launch <code>SPA Forms 365 Installer</code>. To enable ribbon <code>SPA Forms 365 Installer</code> will forcibly switch SharePoint list into <code>Classic experience</code> during provisioning SPA Forms on the list.
  </p>
</div>
![Image of Modern](/img/form-deploy-modern.png)

## Design and Publish custom SPA Form

Unlike out-of-box SharePoint list forms, custom SPA Form must be designed and published before first use with list data. Upon activation SPA Form 365 feature on list, there is no ready to use SPA Form available yet. 
<br/>
<br/>
You can simply start by click on SharePoint list's <code>new item</code> menu item and SPA Forms will walk you through easy few-steps workflow to let you begin with form design:
<br/>
<br/>
![Image of Design1](/img/qs-exersize-1.png)
<br/>
Steps shown on 3-pages screenshot above, moves you from out-of-box <code>List View</code> page, through unavailable yet <code>SFA Form at runtime</code> page, to open <code>SPA Form in Designer</code> page.
<br/>
<br/>
Since we still don't have any SPA Form project setup yet, let's will use convinience hyperlink shown on <code>SPA Forms Designer</code> page to <code>create new project</code>, and move us forward: to the next screenshot below.
<div class="note">
  <h5>ProTip™: Quick initial design for new form project</h5>
  <p>
    SPA Forms designer can help quickly initialize newly created SPA project. Use <code>Open</code> button on ribbon to explore a few options to start with: <code>Empty Layout</code>, <code>Layout with all SharePoint List Columns</code> or <code>Layout imported from GitHub</code> initial designs.
  </p>
</div>
For quick start, we will initialize SPA Form project with <code> All SharePoint List Columns Layout</code> and publish it into runtime without any further customizations. To complete this task, just follow graphical guidance (arrows) on the 3-pages screenshot, and finally press <code>Publish</code> button to complete:
<br/> 
<br/>
![Image of Published](/img/qs-exersize-2.png)
<br/>
<div class="note warning">
  <h5>Important Web Browser Compatibility Note:</h5>
  <p>
    You must use modern web browser, like <code>Google Chrome</code>, <code>Microsoft Edge</code> or <code>Firefox</code> to run project publishing. 
    <code>Microsoft IE-11</code> web browser can't support a few SPA Forms 365 UI features, including <code>Project Publishing</code>.
  </p>
</div>
Wait until SPA Forms designer will publish SPA form project into single minified runtime module and show <code>Completed</code> message. 
<br/>
<br/>
Now we are good to go and start using newly created SPA Form. You can follow a few steps illustrated below, to open newly created form in runtime:
<br/>
<br/>
![Image of Published](/img/qs-exersize-3.png)
<br/>

## Next steps

Building default SPA Form is just the first step. More to add here ...
