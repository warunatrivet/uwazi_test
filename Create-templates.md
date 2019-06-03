Templates allow you to attribute structured, consistent metadata to your entities. Within each Template, you can assign properties:
* text 
* numeric
* select ([needs thesauri](https://github.com/huridocs/uwazi/wiki/Create-thesauri)) 
* multi-select ([needs thesauri](https://github.com/huridocs/uwazi/wiki/Create-thesauri)) 
* date, date range, multi date, multi date range
* rich text
* geolocation
* external link
* media (for video and audio embedding or self-hosting)
* image
* relationship, which allows you to use items from another template as thesauri items

For example, you may want to create a template called "Court" which will contain properties such as name, judges, location, etc. You create one template for each entity that has a distinct set of properties.

Under _Templates_, you can view, edit, and delete existing templates. 

## Follow these steps:

1. Click on the gear icon in the top right corner of the site.

![Gear icon](https://raw.githubusercontent.com/huridocs/uwazi-assets/master/wiki/screenshots/settings_link.jpg)

2. Go to _Templates_.
3. Click on _Add template_.
4. You will see two default properties: _Title_, and _Date added_. 
5. Add properties by dragging them into the designated box. 
6. Edit the Name of the property that you are adding.
7. Click _Save_.

![New template](https://raw.githubusercontent.com/huridocs/uwazi-assets/master/wiki/screenshots/new_document_entity.jpg)

Note: 

1. In case the instance should be in Arabic, the template and properties should be created in latin characters then translated into Arabic, otherwise it is going to trigger a bug. Developers are working to fix it.

2. When you add a **select** or **multi-select property** to a type, you will see a field titled _Thesauri_ in which you can select a _Thesaurus_ or a _Template_ that you have already created. See the section on [create thesauri](https://github.com/huridocs/uwazi/wiki/Create-thesauri) for more information on how to create these thesauri. 
