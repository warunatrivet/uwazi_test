You can add graphs and other data visualization elements to pages and rich text fields.

## Search Box

This code snippet added to any page or rich text field, will render a search box that will run queries on your collections of documents:

```
<SearchBox placeholder="Search corruption cases..." />
```

Such as:
![Component search box](https://github.com/huridocs/uwazi-assets/blob/master/wiki/screenshots/component-search-box.png)

## Counter
```
<Dataset />
<div className="home-bullet">
    <MarkdownLink url="https://your_uwazi_url/en/library/?q=(filters:(type_of_case:(values:!(%27931c8ec2-848d-4e70-a10a-5f8517d08db8%27))),order:desc,sort:creationDate,types:!(%2759d25a6fd841d62ab685815d%27))">
      <div className="big-bullet">
        <Counter property="type_of_case" value="931c8ec2-848d-4e70-a10a-5f8517d08db8" />
      </div>
      <span>Financial Crime Case</span>
    </MarkdownLink>
  </div>
```
Will render a total counter such as:

![Total counter](https://github.com/huridocs/uwazi-assets/blob/master/wiki/screenshots/component-total-counter.png)

Explained:

```
<Dataset />
```
Will inject the data from the default library query so its available to be used as data source for the components. This includes all aggregations for all filters.

You can create other datasets based on library queries that will provide different aggregations for your charts and graphs:

```
<Dataset name='a_name_to_refer_this_dataset' url='http://localhost:3000/?q=(filters:(super_powers:(values:!(ecff0687-19c0-459c-bcbe-0e8d78e1a919))),order:desc,sort:creationDate,types:!(%2758ad7d240d44252fee4e61fd%27))' />
```

```
<MarkdownLink url="https://your_uwazi_url/en/library/?q=(filters:(type_of_case:(values:!(%27931c8ec2-848d-4e70-a10a-5f8517d08db8%27))),order:desc,sort:creationDate,types:!(%2759d25a6fd841d62ab685815d%27))">
```
Will create a link to the library with a particular subselection of data.

```
 <Counter property="type_of_case" value="931c8ec2-848d-4e70-a10a-5f8517d08db8" />
```
Will display the total for a particular option from a library filter (or aggregation). In this case for the property "type_of_case" and the value "931c8ec2-848d-4e70-a10a-5f8517d08db8" (Financial crime case). You can pass a comma separated list of values to the "value" property to add multiple values of the same property together (useful for reporting combined number of documents of different templates, for example).

Obtaining the actual value id requires knowledge of which value represents each database id. This information can be obtained by accessing https://your_uwazi_url/api/templates.

The rest of the code is regular HTML than can be tweaked via [CSS customization](https://github.com/huridocs/uwazi/wiki/Customize-the-interface)

## Bar chart
```
<BarChart property="nigerian_state" context="59d25ff4d841d62ab6858184" />
```

Will render:

![Bar chart](https://github.com/huridocs/uwazi-assets/blob/master/wiki/screenshots/component-graph-bar.png)

Context is used for pulling out translations for the labels. This value is the id of the thesaurus, if labels are coming from a thesaurus and the id of the entity template, if its coming from using templates as select options.

You can find these values via the api: https://your_uwazi_url/api/templates. ie, for a thesauri based property (selects and multiselects), it looks like: (Depending on your browser, you may need to install a JSON viewer extension) 

```
id	"cb273227-0e0b-44e1-98e5-6c88fb0e7ed1"
name	"property_name"
filter	true
showInCard	true
content	"58cf1c10f53d6d50ab7494d3"
type	"multiselect"
label	"Property name"
_id	"58d070f2f53d6d50ab749607"
nestedProperties	[]
```
In this case, the context we are looking for is "58cf1c10f53d6d50ab7494d3" (content).

## Pie chart
```
<PieChart property="type_of_court" context="59d259f4d841d62ab6858157" />
```

Will render:

![Pie chart](https://github.com/huridocs/uwazi-assets/blob/master/wiki/screenshots/component-pie-chart.png)

## Card list

```
{list}(https://your_uwazi_url/en/library/?q=(order:desc,sort:creationDate))(limit:3)
```
Renders:
![Card list](https://github.com/huridocs/uwazi-assets/blob/master/wiki/screenshots/component-card-list.png)

This syntax will display an arbitrary number of cards, defined by the param "limit", based on a library query URL.

## Map

```
<Dataset geolocation="true" />
<Map />
```
Renders:
![Map](https://github.com/huridocs/uwazi-assets/blob/master/wiki/screenshots/component-map.png)


The map component requires a dataset with geolocation data in order to work properly, and the `geolocation` attribute of the `Dataset` component should be activated (`geolocation="true"`).

Clicking on individual or cluster markers in the map will open a side panel with more information about the selected items.

## EntityInfo

```
<EntityInfo entity="entitySharedId" tag="div" classname="classes">More Info</EntityInfo>
```

Creates an HTML element of the type described in tag ("div" is default and can be omitted) bound to a "click" event that will load and display, on the a side panel, the info of the entity described in the "entity" property.  The element allows further HTML structure inside, so you can tailor the 'button' look however you want.