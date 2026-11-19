# Day 4: HTML Tables

## What Tables Are For

HTML tables organize **tabular data** into rows and columns. Do not use them for webpage layout.

## Essential Elements

|Tag|Purpose|
|---|---|
|`<table>`|Table container|
|`<tr>`|Table row|
|`<th>`|Header cell|
|`<td>`|Data cell|
|`<caption>`|Table title or description|

```html
<table>
  <caption>Weekly Study Hours</caption>
  <tr>
    <th>Day</th>
    <th>Hours</th>
  </tr>
  <tr>
    <td>Monday</td>
    <td>2</td>
  </tr>
</table>
```

## Table Sections

|Tag|Holds|
|---|---|
|`<thead>`|Header rows|
|`<tbody>`|Main data rows|
|`<tfoot>`|Footer or summary rows|

```html
<table>
  <caption>Weekly Study Hours</caption>
  <thead>
    <tr><th>Day</th><th>Hours</th></tr>
  </thead>
  <tbody>
    <tr><td>Monday</td><td>2</td></tr>
    <tr><td>Tuesday</td><td>3</td></tr>
  </tbody>
  <tfoot>
    <tr><th>Total</th><td>5</td></tr>
  </tfoot>
</table>
```

## Header Accessibility

Use `scope` on `<th>` so screen readers know what the header applies to.

|Attribute|Meaning|
|---|---|
|`scope="col"`|Header for a column|
|`scope="row"`|Header for a row|

```html
<tr>
  <th scope="col">Day</th>
  <th scope="col">Hours</th>
</tr>
<tr>
  <th scope="row">Monday</th>
  <td>2</td>
</tr>
```

## Spanning Cells

|Attribute|Effect|
|---|---|
|`colspan="2"`|Cell spans two columns|
|`rowspan="2"`|Cell spans two rows|

```html
<tr>
  <th colspan="2">Week 1</th>
</tr>
<tr>
  <td rowspan="2">Morning</td>
  <td>HTML</td>
</tr>
```
