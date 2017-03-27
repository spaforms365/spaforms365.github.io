---
title: Basic Usage
permalink: /docs/usage/
---

Custom SPA Form project should be designed first and then published into runtime model runned by end users.
<br/> 
<br/>
<code>Design</code> and <code>Runtime</code> environments are <code>fully isolated</code> from each other. 
User can safely modify design and debug SPA Form project, with no risk to affect current in use runtime version of SPA form model.
<br/> 
<br/>
When changes with design are completed, SPA Form project can be <code>published</code> to update runtime model for end users. 

### Use SPA Form runtime model:
Published SPA Form runtime model substitutes all out-of-box list forms.
<br/> 
User can continue use any standard out-of-box SharePoint UI controls (context menus, ribbon buttons, etc) to manipulate with SharePoint List Items.
Any requests to out-of-box New, Display or Edit forms will be redirected to SPA Form.  
<br/>
![Image of States Demo](/img/form-states-demo.gif)
<br/> 
<br/>
SPA Form comes along with associated<code>FORM</code> ribbon tab. The ribbon tab carries set of control buttons, similar to out-of-box SharePoint form. 
<br/>
Set of controls on ribbon duplicates functionality of <code>buttons library component</code> placed on SPA Form surface and enabling the form state management.
<br/>
Embedded <code>workflow managing state</code> of SPA Form is illustrated below. 
<br/>
<br/>
![Image of State Machine](/img/form-statemachine.png)
<br/>
There are total 6 control buttons - <code>Submit</code>, <code>Save</code>, <code>Close</code>, <code>Cancel</code>, <code>Update</code> and <code>Delete</code>, available for user and provided via <code>buttons</code> library component.   

### Design SPA Form project usage:
There are two available options to start SPA Forms designer and open SPA Form project:
* Select existing item on a list and use either<code>Design Item context menu</code> or <code>Design Item button</code> located at ITEMS tab on ribbon. Selected Item will be linked to SPA Form Project and column values will be available during design time. 
* Open LIST tab on ribbon and use out-of-box dropwown option <code>Form Web Parts</code>.
<br/>
To start SPA Forms designer, user need to have at least <code>design</code> permission level assigned on List.  
<br/> 
<br/>
![Image of Open Design](/img/form-open-design.png)
<br/> 
<br/>
![Image of Open Design](/img/form-design.png)
<br/>
### SPA Form project publishing into runtime model:
<br/> 
<br/>
![Image of Publishing](/img/form-publish.png)

