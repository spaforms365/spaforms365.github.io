---
title: Basic Usage
permalink: /docs/usage/
---

Custom SPA Form project should be designed first and then published into runtime model serving end users.
<br/> 
<br/>
<code>Design</code> and <code>Runtime</code> environments are <code>fully isolated</code> from each other. 
User can safely modify design and debug SPA Form project, with no risk to affect current (in use) runtime version of SPA form model.
<br/> 
<br/>
When changes with design are completed, SPA Form project can be <code>published</code> to update runtime model serving end users. 

### Published SPA Form serving users at runtime:
Published SPA Form runtime model replaces all out-of-box list forms.
<br/> 
User can continue use any standard out-of-box SharePoint UI controls (context menus, ribbon buttons, etc) to work with SharePoint ListItems.
Any requests to out-of-box New, Display or Edit forms will be redirected to SPA Form.  
<br/>
![Image of States Demo](/img/form-states-demo.gif)
<br/> 
<br/>
SPA Form comes along with associated<code>FORM</code> ribbon tab. The ribbon tab carries set of control buttons, functionally similar to available for out-of-box list forms. 
<br/>
<br/>
Set of controls on ribbon exposes (duplicates) base functionality of <code>buttons</code> library component placed on surface of SPA Form. This component enables SPA Form state management.
<br/>
<br/>
Diagram of embedded state management <code>workflow</code> for SPA Form is illustrated below. 
<br/>
<br/>
![Image of State Machine](/img/form-statemachine.png)
<br/>
There are total six UI control buttons - <code>Submit</code>, <code>Save</code>, <code>Close</code>, <code>Cancel</code>, <code>Update</code> and <code>Delete</code> provided by <code>buttons</code> library component for interactive form state management.   

### Design SPA Form project usage:
There are two available options to start SPA Forms designer and open SPA Form project:
<ul>
<li> Select existing item on a list and use either<code>Design Item context menu</code> or <code>Design Item button</code> located at ITEMS tab on ribbon. Selected Item will stay linked to SPA Form Project at design time and column values will be accessible on form: similar to out-of-box Design or Edit forms. </li>
<li> Open LIST tab on ribbon and use out-of-box dropwown option <code>Form Web Parts</code>. This case would be more closer modeling out-of-box New form. </li>
</ul>

To start SPA Forms designer, user need to have at least <code>design</code> permission level assigned on List.  
 
<br/>
![Image of Open Design](/img/form-open-design.png)
<br/> 
To exit SPA Form designer and return back to SharePoint list view, press button <code>Close</code> on ribbon.
<br/>
![Image of Open Design](/img/form-design.png)
<br/>
### SPA Form project publishing into runtime model:
<br/> 
<br/>
![Image of Publishing](/img/form-publish.png)

