---
title: Template
permalink: /docs/designer-template/
---
<code>SPA Forms 365 Designer</code> promotes <code>visual</code> form design style. 
<br/>
<br/>

### Form Layout
<code>Content</code> on SPA Form organized and structured on top of suitable <code>layout</code>. <code>HTML Template</code> of the root (or underlying) component at hierarchical structure of SPA Form project, provides <code>layout</code> for the whole project.
<br/>
<br/>
To work on form layout, Designer enables two side-by-side panels: <code>HTML Layout</code> in <code>Grid</code> mode and <code>HTML Template</code>: 
<br/>
<br/>
![Image of Layout Ribbon](/img/form-ribbon-layout.png)
<br/>
To enable layout, <code>HTML Template</code> of the root component has <code>responsive grid</code> markup powered by <b>[Office UI Fabric](https://dev.office.com/fabric){:target="_blank"}</b>. Easiest way to configure desired form layout is <code>visual</code>, using interactive capabilities of <code>HTML Layout</code> panel, when toggled into <code>Grid</code> mode: 
<br/>
<br/>
![Image of Grid Editing](/img/form-gridediting.gif)
<br/>
Visually composed design at <code>HTML Layout</code> form preview, immediately gets converted into source code at <code>HTML template</code>. And vice-versa: changes made with <code>HTML template</code> source code, immediately gets visialized at <code>HTML Layout</code> form preview.

### Placing SharePoint columns and components on layout {#placingcomponents}

<code>Visual design style</code> is also convenient to place SharePoint columns and various other components on drawing surface of the form. <code>Columns and Components picker panel</code> can be accessed from any <code>target cell</code> on layout. Developer can select group of Sharepoint columns and/or components on picker panel and drop it into target cell. Each dropped component can be re-arranged later between other cells on layout responsive grid: 
<br/>
<br/>
![Image of Placing Components](/img/form-placingcomponents2.gif)
<br/>
<br/>
SPA Forms 365 uses <b>[library](/docs/designer-syslibrary/#syscomponents)</b> of form components to render various types of SharePoint List columns on form layout.
<br/>
<br/> 
![Image of Component HTML](/img/form-component-html.png)
 
### Freestyle Editing HTML Template {#editingtemplate}
Interactive visual design is good to quickly compose initial draft for template rendered by SPA Form component. HTML Template editor is convenient tool for further HTML template source code development. Changes made in code immediately gets visualized on HTML Layout: 
<br/>
<br/>
![Image of Placing HTML](/img/form-placinghtml.gif)

