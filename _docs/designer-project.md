---
title: Project
permalink: /docs/designer-project/
---
<code>SPA Form project</code> is a collection of <b>[Knockout components](http://knockoutjs.com/documentation/component-overview.html){:target="_blank"}</b>. Inside of the project, components are organized into hierarchcal structures.
<br/>
At runtime each component in project hierarchy instanciates its Template/Model pair into <code>MVVM runtime model</code>. Altogether, these instances produces <code>Single Page Application</code> powering SPA Form.
<br/>

###  Runtime (published) project
In <code>production</code> SPA Form project is a single file <code>model.min.js</code>, residing at <code>/Form/Runtime</code> folder under SharePoint List file structure on server. Designer <b>[published](#projectpublishing)</b>all project source code into that single file in optimized & minified format. If end user interacts with out-of-box SharePoint List UI, the <code>SPA Forms runtime</code> launches <code>model.min.js</code> to create instance of Single Pade Application powering SPA Form.
###  Design (development) project
![Image of Ribbon-project](/img/Ribbon-project.png)
<br/>
<br/>
<code>Development</code> version of SPA Form project is a set of source code files, residing in <code>Design</code> folder on SharePoint server. To remotely open Design folder with Windows Explorer on your local computer use <code>Explore Files</code> button on Ribbon.
<br/>
<br/>
Newly created SPA Form project contains the following 3 files in Design folder: 
* <code>project.js</code> - automatically managed by SPA Forms Designer. The file contains registration info for custom components and project external dependencies - like SharePoint columns or workflow definitions.
* <code>viewmodel.html</code> - HTML <code>template</code> for Knockout root component at SPA Form project hierarchy.
* <code>viewmodel.js</code> - Javascript <code>model</code> for Knockout root component.

SPA Forms Designer environment supports various aspects of SPA project management, such as initial setup, dependencies tracking, version control, import/export, etc.

###  Quick setup options for new SPA Form project {#projectinit}
![Image of Setup Option](/img/form-setup-options.png)

###  Publishing {#projectpublishing}

###  Project import/export {#projectmigrations}

###  Components versioning {#componentsversioning}
![Image of Form Versioning](/img/form-versioning.png)

###  Custom components management {#componentscustom}

