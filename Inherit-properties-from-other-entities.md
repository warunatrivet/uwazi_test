There are times when it is useful to display a property on more than one entity. 

For example, if your data model includes an entity type that captures information about prisoners, and an entity type that captures information about the jail in which they detained, you may want to be able to display the location of the prisoners on a map via the location of the jails. 

Instead of duplicating the geolocation property and collecting the same data twice (once in the **prisoner** entity template, and again in the **jail** template), Uwazi supports the ability to inherit a property from one entity type to another, via a relationship. 

The first step is to create the property for which you want to be inherited. To use the example above, you will create the geolocation property on the **jail** entity template. This will serve as the one place to capture the geolocation of the jails. 

The next step is to [create a relationship](https://github.com/huridocs/uwazi/wiki/Create-Different-Relationships) that will represent the relationship between the **jail** and the **prisoner**. You may want to call this something like "location" or "jail". For this example, we'll use the name "jail".  

The next step is to create a relationship property _from_ the entity template that you want to inherit a property, _to_ the entity type that has the property you want to inherit. To use the example above, you will edit the **prisoner** entity template to add a relationship property. The name of this relationship property is whatever you named the relationship in the previous step ("jail"). As you are creating this relationship property, you will be asked to select which entity type you want the relationship to include and you will select "Jail" because that is the entity type that has the geolocation property you want to inherit. Then you will be asked if you want to inherit a property from the "Jail" entity template. Here is where you can select the geolocation property. 

![Inherit property](https://github.com/huridocs/uwazi-assets/blob/master/wiki/screenshots/inherit-property.png)

Now that these two entity types have this relationship established and the inherited property, when you create a relationship between prisoner X and jail Y, the prisoner X entity will inherit the geolocation of jail Y, allowing you to show the location of the prisoner (or prisoners) on a map. 

![Map via inherited properties](https://github.com/huridocs/uwazi-assets/blob/master/wiki/screenshots/inherited-properties-map.png)

This is the equivalent to a foreign key in a relation database that gets resolved to a particular property of the linked record. 