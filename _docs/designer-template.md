---
title: Template
permalink: /docs/designer-template/
---
<code>Template</code> is what you actually see, when open SPA Form. 
<br/>
<br/>
<b>SPA Form's [knockout component](http://knockoutjs.com/documentation/component-overview.html){:target="_blank"}</b> needs both: template and model to build functionining MVVM runtime form. However in many practical use cases, you can leave model in initial state and customize only form template.
<div class="note">
  <h5>ProTip™: Coding may not needed to build working SPA Form</h5>
  <p>
    Basic template customization doesn't require software programming. Because <code>SPA Forms 365 Designer</code> promotes <code>visual</code> form design style. Some limited knowledge of HTML markup may be needed to design professionally-looking forms.
  </p>
</div>
### Form Layout
<code>Content</code> on SPA Form is organized and structured on top of suitable <code>layout</code>. <code>HTML Template</code> of the root (or underlying) component at hierarchical structure of SPA Form project, provides <code>layout</code> for the whole project.
<br/>
<br/>
To work on form layout, Designer enables two side-by-side panels: <code>HTML Layout</code> in <code>Grid</code> mode and <code>HTML Template</code>: 
<br/>
<br/>
![Image of Layout Ribbon](/img/form-ribbon-layout.png)
<br/>
<br/>
To enable layout, <code>HTML Template</code> of the root component has <code>responsive grid</code> markup powered by <b>[Office UI Fabric](https://dev.office.com/fabric){:target="_blank"}</b>. Easiest way to configure desired form layout is <code>visual</code>, using interactive capabilities of <code>HTML Layout</code> panel, when toggled into <code>Grid</code> mode: 
<br/>
<br/>
![Image of Grid Editing](/img/form-gridediting.gif)
<div class="note">
  <h5>ProTip™: HTML Layout & Template panels are always in sync !</h5>
  <p>
    Visually composed design at <code>HTML Layout</code> form preview, immediately gets converted into source code at <code>HTML template</code>. And vice-versa: changes made with <code>HTML template</code> source code, immediately gets visialized at <code>HTML Layout</code> form preview.
  </p>
</div>

### Placing SharePoint Columns and Components on Layout {#placingcomponents}

<code>Visual design style</code> is also efficient option to place <code>SharePoint columns</code> and various components on drawing surface of the form. 
<br/>
<br/>
<code>Columns and Components Picker panel</code> can be launched from any <code>target cell</code> on layout. Then selected group of Sharepoint columns and/or Form components can be <code>placed</code> into target cell. Each placed component in the group can be re-arranged later between other cells on layout responsive grid: 
<br/>
<br/>
![Image of Placing Components](/img/form-placingcomponents2.gif)
<div class="note">
  <h5>ProTip™: Your SPA Form is powered by system library components</h5>
  <p>
    <code>SPA Forms 365 Designer</code> uses <b>[form components library](/docs/designer-syslibrary/#syscomponents)</b> to render various types of SharePoint List columns on SPA Form.
  </p>
</div>
 
### Direct HTML Template Markup Customization {#editingtemplate}

Interactive visual design style is most productive approach to draft form template quickly. Further template customizations are possible via direct HTML markup editing at <code>HTML Template</code> panel. 
<br/>
<br/>
![Image of Placing HTML](/img/form-placinghtml.gif)
<div class="note">
  <h5>ProTip™: Any HTML markup features are allowed on template !</h5>
  <p>
    You can insert static text, links, images, etc. - everything what HTML markup allows for developer. Changes made in HTML markup, are immediately passed into <code>HTML Layout</code> panel, enabling ad-hock visual feedback. 
  </p>
</div>

