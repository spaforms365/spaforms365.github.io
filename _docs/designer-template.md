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
To conveniently design form layout we may open side-by-side two panels on Designer page: <code>HTML Layout</code> in <code>Grid</code> mode and <code>HTML Template</code>: 
<br/>
<br/>
![Image of Layout Ribbon](/img/form-ribbon-layout.png)
<br/>
To implement layout, <code>HTML Template</code> of the root component contains markup for <code>responsive grid</code> powered by Office UI Fabric. It is easy to visually compose desired form layout using interactive builder on <code>HTML Layout</code> panel, when toggled into <code>Grid</code> mode: 
<br/>
<br/>
![Image of Grid Editing](/img/form-gridediting.gif)
<br/>
Visually composed design at <code>HTML Layout</code> form preview, immediately gets converted into source code at <code>HTML template</code>. And vice-versa: changes made with <code>HTML template</code> source code, immediately gets visialized at <code>HTML Layout</code> form preview.

### Placing Content {#placingcomponents}

Designer can interactively pick and place SharePoint list columns, library or custom components on drawing surface of the form. Columns and Components <code>picker panel</code> is accessible right from <code>target cell</code> on responsive grid. Selected group of components are droppable in bulk on target cell and can be re-arranged later between other cells on the grid. 
<br/>
<br/>
![Image of Placing Components](/img/form-placingcomponents2.gif)
<br/>
<br/>
Interactively dropped component instance immediately gets injected into hierarchy of the SPA project. Columns and Components picker panel <code>dynamically matches</code> selected SharePoint Column properties and metadata-defined interface at Knockout component to determine <code>params values</code> needed to call <code>component instance</code>:
<br/>
<br/> 
![Image of Component HTML](/img/form-component-html.png)
 
### Freestyle Editing HTML Template {#editingtemplate}
Interactive visual design is good to quickly compose initial draft for template rendered by SPA Form component. HTML Template editor is convenient tool for further HTML template source code development. Changes made in code immediately gets visualized on HTML Layout: 
<br/>
<br/>
![Image of Placing HTML](/img/form-placinghtml.gif)

