# FilterCriteria Object (JavaScript API for Excel)

_Excel 2016, Excel Online, Excel for iPad, Excel for Mac_

Represents the filtering criteria applied to a column.

## Properties

| Property	   | Type	|Description| Req. Set|
|:---------------|:--------|:----------|:----|
|color|string|The HTML color string used to filter cells. Used with "cellColor" and "fontColor" filtering.|1.2||
|criterion1|string|The first criterion used to filter data. Used as an operator in the case of "custom" filtering.|1.2||
|criterion2|string|The second criterion used to filter data. Only used as an operator in the case of "custom" filtering.|1.2||
|values|object[]|The set of values to be used as part of "values" filtering.|1.2||

_See property access [examples.](#property-access-examples)_

## Relationships
| Relationship | Type	|Description| Req. Set|
|:---------------|:--------|:----------|:----|
|dynamicCriteria|[DynamicFilterCriteria](dynamicfiltercriteria.md)|The dynamic criteria from the Excel.DynamicFilterCriteria set to apply on this column. Used with "dynamic" filtering.|1.2||
|filterOn|[FilterOn](filteron.md)|The property used by the filter to determine whether the values should stay visible.|1.2||
|icon|[Icon](icon.md)|The icon used to filter cells. Used with "icon" filtering.|1.2||
|operator|[FilterOperator](filteroperator.md)|The operator used to combine criterion 1 and 2 when using "custom" filtering.|1.2||

## Methods

| Method		   | Return Type	|Description| Req. Set|
|:---------------|:--------|:----------|:----|
|[load(param: object)](#loadparam-object)|void|Fills the proxy object created in JavaScript layer with property and object values specified in the parameter.|1.1|

## Method Details


### load(param: object)
Fills the proxy object created in JavaScript layer with property and object values specified in the parameter.

#### Syntax
```js
object.load(param);
```

#### Parameters
| Parameter	   | Type	|Description|
|:---------------|:--------|:----------|:---|
|param|object|Optional. Accepts parameter and relationship names as delimited string or an array. Or, provide [loadOption](loadoption.md) object.|

#### Returns
void