Uwazi supports connecting data in unstructured ways, meaning you don't need to follow a particular data structure or predefine a relational model upfront. Both entities and documents can be connected to each other in one-to-one or one-to-many relations arbitrarily:

![](https://github.com/huridocs/uwazi-assets/blob/master/wiki/screenshots/relationships-overview.png)

## Information hubs

Uwazi relationships support information hubs, that is, a concentrator that holds together a series of documents or entities. Hubs are useful for telling apart mixed information. Ie. a person may be related to two different legal cases but you want that information segregated:

![](https://github.com/huridocs/uwazi-assets/blob/master/wiki/screenshots/relationships-hubs-example.png)

A hub denotes relationships that, not only make sense to have grouped, but that would INFER A RELATIONSHIP BETWEEN ALL ITS CHILDREN.

So, if document A has a hub with documents B and C, then a relationship would be inferred between B and C also. Not only inferred but it actually exists. On the other hand, if you have document A with one hub to B and another hub to C, then B and C will have NO relationship between each other.

## Creating connections

You can create and edit relationships by clicking on the "Edit" button at the bottom of the page. After adding, removing or renaming the connected entities or documents, click on save to store your changes:

![](https://github.com/huridocs/uwazi-assets/blob/master/wiki/screenshots/relationships-edition.png)

## Relationship fields in templates

Former select and multiselect fields that used an entity template as options, have been replaced with a relationship field. This is a preconfigured relationship type with some advantages:

- The allowed targed entities (select list) can be used to force connecting only to one type of template. Ie. If we have a type "Country" and we want to add that property to another type (ie. Person). Specifying the select list "Country" will force users to use only countries for this field.
- A relationship type can be defined as well.

![](https://github.com/huridocs/uwazi-assets/blob/master/wiki/screenshots/relationships-field-config.png)

This means, a Relationship field will behave as a regular multiselect, and at the same time, create a relationship of a particular type that will be displayed in the relationships tree view:

![](https://github.com/huridocs/uwazi-assets/blob/master/wiki/screenshots/relationship-field-tree.png)

Likewise, configuring a Relationship field for a set of connections that already exist, will display these connections as a multiselect field. Ie. we added some connections as signers of a document:

![](https://github.com/huridocs/uwazi-assets/blob/master/wiki/screenshots/relationships-example-1.png)

And we configure a Relationship field with "Judges" as the target entity and "Signers" as the relationship type, it will be presented in the metadata as:

![](https://github.com/huridocs/uwazi-assets/blob/master/wiki/screenshots/relationships-as-metadata-1.png)

Moreover, this field can be used for filtering as a regular multiselect:

![](https://github.com/huridocs/uwazi-assets/blob/master/wiki/screenshots/relationships-as-filter.png)

Also, you can configure this field as the rest of the metadata fields:

![](https://github.com/huridocs/uwazi-assets/blob/master/wiki/screenshots/relationship-field-config-2.png)

- Required: will force a particular entity of document to have at least one relationship of a particular type. Ie, all documents must have a country.
- Show in cards: will display the relationships as metadata en the grid cards.
- Use as filter: this relationship can be filtered in the library.
- Default filter: this filter will be shown regardless of document and entity types being selected.




