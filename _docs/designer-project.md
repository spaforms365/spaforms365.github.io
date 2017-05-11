---
title: Project
permalink: /docs/designer-project/
---
<code>SPA Form project</code> is a collection of <b>[Knockout components](http://knockoutjs.com/documentation/component-overview.html){:target="_blank"}</b>. <code>Form layout</code> normally backed by single (root) component and <code>fiels on form</code> by [usually library] components placed on top of the layout.
<br/>
At runtime, all components on project hierarchy <code>instanciates</code> their <code>template/model pairs</code> into <code>MVVM runtime models</code>. Altogether, these instances produces <code>Single Page Application</code> powering SPA Form.
<br/>

###  Published (runtime) project
<code>Published</code> SPA Form project appears as a single file <code>model.min.js</code>. 
<br/>
<br/>
When user interacts with out-of-box SharePoint List UI, <code>SPA Forms runtime</code> launches <code>model.min.js</code> to instanciate Single Pade Application powering SPA Form.
###  Design (development) project
SPA Form project at <code>design time</code> is a set of components source code files and single <code>project.js</code> file.
<br/>
<br/>
Normally at design-time all source code project files are permanently stored in your web browser's <code>local storage</code>, on your computer's hard drive. Additionally you can save source code at <code>remote repositories</code>: on SharePoint server or on GitHub.
<br/>
<br/>
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

<br/>
<code>SPA Forms 365 Designer</code> <b>[publishing](#projectpublishing)</b> operation copies all project source code  in optimized & minified format into single file, located at <code>/Form/Runtime/</code> folder under SharePoint List file structure on <code>SharePoint server</code>.


###  Project import/export {#projectmigrations}

###  Components versioning {#componentsversioning}
![Image of Form Versioning](/img/form-versioning.png)

###  Custom components management {#componentscustom}

