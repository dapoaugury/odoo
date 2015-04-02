Odoo Website Builder - Simple Website Menu Features to Copy and Delete Web CMS Pages
------------------------------------------------------------------------------------

To implement Page Copy and Page Delete menu options, changes have been made in following four files:

-- website/controllers/main.py
Functions: pagecopy, pagedelete

-- website/models/website.py
Functions: copy_page, delete_page

-- website/static/src/js/website.contentMenu.js
Functions: copy_page, delete_page

To create entry points (menu options in top menu bar), following XML file must be changed to include two new lines:

-- website/static/views/website_backend_navbar.xml (line 56)

```
   <li groups="base.group_website_designer"><a href="#" data-action="copy_page">Copy Page</a></li> 
   <li groups="base.group_website_designer"><a href="#" data-action="delete_page">Delete Page</a></li>
```
