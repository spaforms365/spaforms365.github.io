---
title: Designer Environment
permalink: /docs/designer-overview/
---

SPA Forms project is a <code>Single Page Application</code> (SPA) based on [Knockout](http://knockoutjs.com/documentation/introduction.html) <code>data model</code>.
<br/> 
SPA Forms project internally structured as <code>hierarchy</code> of a self-contained and reusable chunks: <code>components</code>.
This pattern is beneficial for large applications, because it <code>simplifies development</code> through clear organization and encapsulation, and helps to <code>improve runtime performance</code> by incrementally loading your application code as needed.
<br/>
SPA Forms 365 Designer is a multipage development environment, where <code>one page</code> surfaces a <code>single component</code> on hierarchy of SPA Form project. Each Designer page appears as an individual <code>TAB</code> on Ribbon. 
<br>
<br/>
[Knockout component](http://knockoutjs.com/documentation/component-overview.html) is a pair of HTML <code>Template</code> and Javascript <code>Model</code>. At runtime nested component receives <code>parameters</code> out of project hierarchy and dynamically binds its parts into <code>MVVM runtime model</code>. 
<br/>
To design and debug component, Designer page has 3 editors: <code>HTML Template</code>, <code>Javascript Model</code> and <code>Layout</code> represinting MVVM component model at runtime.    
<br/>
<br/>
![Image of Designer Overview](/img/form-designer3.gif)
<br/>
