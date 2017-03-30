---
title: Designer Environment
permalink: /docs/designer-overview/
---

SPA Forms project is a <code>Single Page Application</code> (SPA) based on [Knockout](http://knockoutjs.com/documentation/introduction.html){:target="_blank"} data model.
<br/> 
SPA Forms project internally structured as <code>hierarchy</code> of a self-contained and reusable chunks: <code>components</code>.
This pattern is beneficial for large applications, because it <i>simplifies development</i> through clear organization and encapsulation, and helps to <i>improve runtime performance</i> by incrementally loading your application code as needed.
<br/>
<br/>
SPA Forms 365 Designer is a multipage development environment, where <code>one page</code> surfaces a <code>single component</code> on hierarchy of SPA Form project. Each Designer page appears as an individual <code>TAB</code> on Ribbon. 
<br>
<br/>
[Knockout component](http://knockoutjs.com/documentation/component-overview.html){:target="_blank"} is a pair of HTML <code>Template</code> and Javascript <code>Model</code>. At runtime nested component receives <code>parameters</code> out of project hierarchy and dynamically binds its parts into <code>MVVM runtime model</code>. 
<br/>
<br/>
To design and debug component, developer can use Ribbon to toggle up to 3 editors: <code>HTML Template</code>, <code>Javascript Model</code> and <code>HTML Layout</code>, visualizing MVVM model at runtime.    
<br/>
![Image of Designer Overview](/img/form-designer3.gif)
<br/>
<code>HTML Layout</code> editor additionally provides developer with complimentary visual editing option for HTML Template. Use <code>Grid</code> button on Ribbon to toggle <code>HTML Layout</code> editor between graphical design and visualization modes. 