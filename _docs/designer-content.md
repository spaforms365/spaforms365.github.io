---
title: Placing Content
permalink: /docs/designer-content/
---

SPA Forms promotes visual form design style. Interactively made design modifications are transparently rendered into SPA form project source code.

### Placing SharePoint Columns and Components on Form {#placingcomponents}

Developer interactively picks and places SharePoint list columns, library or custom components on drawing surface of the form. Columns and Components <code>picker panel</code> is accessible right from <code>target cell</code> on responsive grid. Selected group of components are droppable in bulk on target cell and can be re-arranged later between other cells on the grid. 
<br/>
<br/>
![Image of Placing Components](/img/form-placingcomponents2.gif)
<br/>
<br/>
Interactively dropped component instance immediately gets injected into hierarchy of the SPA project. Columns and Components picker panel <code>dynamically matches</code> selected SharePoint Column properties and metadata-defined interface at Knockout component to determine <code>params values</code> needed to call <code>component instance</code>:
<br/>
<br/> 
![Image of Component HTML](/img/form-component-html.png)

<br/>
### Editing Form HTML Template {#editingtemplate}
![Image of Placing HTML](/img/form-placinghtml.gif)

