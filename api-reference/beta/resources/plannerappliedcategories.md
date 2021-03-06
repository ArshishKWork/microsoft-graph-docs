# plannerAppliedCategories resource type


The AppliedCategoriesCollection* resource represents the collection of categories (or labels) that have been applied to a task. It is part of the [plannerTask](plannertask.md) object.
There can be up to 6 categories applied to a task. Category names, e.g. `category0`, `category1` etc., are part of the [plan details](plannerplandetails.md) object. 

*Note that this is an Open Type.


### Properties
Properties of an Open Type can be defined by the client. In this case though, the client must provide `category0`, `category1`, `category3`, `category4` and/or `category5` as properties with their values being the `true` boolean when the corresponding categories are applied on the task. Example is shown below. When they do not apply, properties are automatically removed by setting their values to the `false` boolean. 

## JSON representation

Here is a JSON representation of the resource

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appliedCategoriesCollection"
}-->

```json
{
  "String-value": true
}
```

Example: 

```json
{
  "category0": true,
  "category3": true,
  "category5": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAppliedCategories resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->