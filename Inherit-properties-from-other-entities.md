There are times when it is useful to display a property on more than one entity. 

For example, if your data model includes an entity type that captures information about prisoners, and an entity type that captures information about the jail in which they detained, you may want to be able to display the location of the prisoners on a map via the location of the jails. 

Instead of duplicating the geolocation property and collecting the same data twice (once in the **prisoner** entity template, and again in the **jail** template), Uwazi supports the ability to inherit a property from one entity type to another, via a relationship. 

The first step is to create the property for which you want to be inherited. To use the example above, you will create the geolocation property on the **jail** entity template. This will serve as the one place to capture the geolocation of the jails. 

The next step is to create a relationship that will represent the relationship between the **jail** and the **prisoner**. You may want to call this something like "location" or "jail".  

The next step is to create a relationship _from_ the entity template that you want to inherit a property, _to_ the entity type that has the property you want to inherit. To use the example above, you will edit the **prisoner** entity template to add a relationship property. 



Inherit properties. When modeling your data, sometimes a particular metadata piece is ambiguous and can be placed in one or more templates. With this solution, administrators can configure a metadata property as inherited from another entity. This is the equivalent to a foreign key in a relation database that gets resolved to a particular property of the linked record. Ie. Imagine you have products and warehouses and you want to geolocate both the products and the ware houses. A solution is to have a geolocation property in each template but this leads to duplication of information. Since products also come with the property of which warehouse they are stored in, with inherited properties the geolocation can be added only to the warehouse and the product will inherit that property from the warehouse.