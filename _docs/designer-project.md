---
title: Project
permalink: /docs/designer-project/
---
<code>SPA Form project</code> is a collection of <b>[Knockout components](http://knockoutjs.com/documentation/component-overview.html){:target="_blank"}</b>. <code>Form layout</code> normally backed by single (root) component and <code>form fields</code> by [library] components placed on top of the layout.
<br/>
<br/>
At runtime, all components on project hierarchy <code>instanciates</code> their <code>template/model pairs</code> into <code>MVVM runtime models</code>. Altogether, these instances produces <code>Single Page Application</code> powering SPA Form.
<br/>

###  Published (runtime) project
<code>Published</code> SPA Form project appears as a single file <code>model.min.js</code>. 
<br/>
<br/>
When user interacts with out-of-box SharePoint List UI, <code>SPA Forms runtime</code> launches <code>model.min.js</code> to instanciate Single Pade Application powering SPA Form.
###  Design (development) project
SPA Form project at <code>design time</code> is a set of component's source code files and <code>project.js</code> file. Important information needed to make SPA Form project <code>portable</code> is contained in <code>project.js</code>. 
<br/>
<br/>
Normally at design-time all project's source code files are permanently stored in your web browser's <code>local storage</code>, on your computer's <code>hard drive</code>. Additionally you can copy source code to <code>remote repositories</code>: on SharePoint server or GitHub.
<br/>
<br/>
There are two groups of controls available on Designer Page's ribbon for overall <code>SPA Form project</code> management. These two groups outlined on screenshot below under <code class="project">red border</code>. Controls at <code>Project</code> group are to manage project inside of <code>local storage</code> and controls at <code>Source Code</code> group are to communicate with <code>remote repositories</code>.
<br/>
<br/>
![Image of Ribbon-project](/img/Ribbon-project.png)
<br/>
<br/>

SPA Forms Designer environment supports various aspects of SPA project management, such as initial setup, dependencies tracking, version control, import/export, etc.

###  Quick setup options for new SPA Form project {#projectinit}
![Image of Setup Option](/img/form-setup-options.png)

###  Publishing {#projectpublishing}

<br/>
<code>SPA Forms 365 Designer</code> <b>[publishing](#projectpublishing)</b> operation copies all project source code  in optimized & minified format into single file, located at <code>/Form/Runtime/</code> folder under SharePoint List file structure on <code>SharePoint server</code>.


###  Project import/export {#projectmigrations}

###  Components versioning {#componentsversioning}
![Image of Form Versioning](/img/form-versions.png)

###  Custom components management {#componentscustom}

