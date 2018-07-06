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
Will inject the data from the default library query so its available to be used as data source for the components.

```
<MarkdownLink url="https://your_uwazi_url/en/library/?q=(filters:(type_of_case:(values:!(%27931c8ec2-848d-4e70-a10a-5f8517d08db8%27))),order:desc,sort:creationDate,types:!(%2759d25a6fd841d62ab685815d%27))">
```
Will create a link to the library with a particular subselection of data.

```
 <Counter property="type_of_case" value="931c8ec2-848d-4e70-a10a-5f8517d08db8" />
```
Will display the total for a particular option from a library filter (or aggregation). In this case for the property "type_of_case" and the value "931c8ec2-848d-4e70-a10a-5f8517d08db8" (Financial crime case). This requires knowledge of which value represents each database id. This information can be obtained by accessing https://your_uwazi_url/api. 

The rest of the code is regular HTML than can be tweaked via [CSS customization](https://github.com/huridocs/uwazi/wiki/Customize-the-interface)
