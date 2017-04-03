---
title: Form Model
permalink: /docs/designer-model/
---

### Example: text box bound to SharePoint 

You can now render the list of members in a template:

```html
<input type="text" data-bind="textInput: mytitle"> 
{% raw %}
<ul>
{% for member in site.data.members %}
  <li>
    <a href="https://github.com/{{ member.github }}">
      {{ member.name }}
    </a>
  </li>
{% endfor %}
</ul>
{% endraw %}
```
