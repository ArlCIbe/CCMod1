### Rows - enclosed with `<tr>` tags.

### Headers (aka Columns) - enclosed with `<th>` tags, each representing an actual table cell.
 ##### `<colgroup>` - used as a container for the column specifications (i.e. applying styles to the entire column); must be a **child** of a `<table>` element (AFTER any `<caption>` elements!)
  ##### `<col>` - specifies properties for each column within a `<colgroup>` element; useful for applying styles to entire columns.
  ###### NOTE: only **width**, **visibility**, **background**, and **border** properties can be used inside a `<colgroup>`
   ```
    <table style="width: 100%;">
    <colgroup>
    <col span="2" style="background-color: #D6EEEE">
    <col span="3">
    <col span="1" style="background-color: #D6EEEE">
    </colgroup>
    <tr>
    <th>MON</th>
    <th>TUE</th>
    <th>WED</th>
    <th>THU</th>
    <th>FRI</th>
    <th>SAT</th>
    <th>SUN</th>
    </tr>
    <tr>
    <td>1</td>
    <td>2</td>
    <td>3</td>
    <td>4</td>
    <td>5</td>
    <td>6</td>
    <td>7</td>
    </tr>
    <tr>
    <td>8</td>
    <td>9</td>
    <td>10</td>
    <td>11</td>
    <td>12</td>
    <td>13</td>
    <td>14</td>
    </tr>
    </table>
   ```
### Cells - enclosed with `<td>` tags.
```
<table>
  <thead>
    <tr>
      <th>Month</th>
      <th>Savings</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>January</td>
      <td>$100</td>
    </tr>
    <tr>
      <td>February</td>
      <td>$80</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td>Sum</td>
      <td>$180</td>
    </tr>
  </tfoot>
</table>
```

### Other Table Tags

 #### `<caption>` - gives the table a title; must be inserted immediately after the `<table>` tag.

##### the following specify the parts of a `<table>` (header, body, footer) and:
    + will not affect the table's layout (by default).
    + enable scrolling of the table body independently of the header and footer.  
 #### `<thead>` - groups the header content; must include 1 or more `<tr>` tags inside and be used as a **child** of a `<table>` element (AFTER any `<caption>` and `<colgroup>` elements!)
 #### `<tbody>` - groups the body content; must include 1 or more `<tr>` tags inside and be used as a **child** of a `<table>` element (AFTER any `<caption>`, `<colgroup>`, and `<thead>` elements!)
 #### `<tfoot>` - groups the footer content in a table; must include 1 or more `<tr>` tags inside and be used as a **child** of a `<table>` element (AFTER any `<caption>`, `<colgroup>`, `<thead>`, and `<tbody>` elements!)

### Styling A Table

#### Add Borders to Tables - use the CSS **border** property on `<table>`, `<th>`, and `<td>` elements
##### NOTE: use **border-collapse: collapse** to get rid of the double borders

#### Horizontal Table Headers
```
<table>
  <tr>
    <th>Firstname</th>
    <th>Lastname</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>Jill</td>
    <td>Smith</td>
    <td>50</td>
  </tr>
</table>
```

#### Vertical Table Headers
```
<table>
  <tr>
    <th>Firstname</th>
    <td>Jill</td>
    <td>Eve</td>
  </tr>
  <tr>
    <th>Lastname</th>
    <td>Smith</td>
    <td>Jackson</td>
  </tr>
</table>
```

#### Make a Cell Span Over Multiple Columns/Rows 
 ##### use **colspan** attribute for columns
```
<table>
  <tr>
    <th colspan="2">Name</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>Jill</td>
    <td>Smith</td>
    <td>50</td>
  </tr>
  <tr>
    <td>Eve</td>
    <td>Jackson</td>
    <td>94</td>
  </tr>
</table>
```

- ##### use **row** attribute for rows
```
<table>
  <tr>
    <th>Name</th>
    <td>Jill</td>
  </tr>
  <tr>
    <th rowspan="2">Phone</th>
    <td>555-1234</td>
  </tr>
  <tr>
    <td>555-8745</td>
</tr>
</table>
```

#### Change Spacing Between Cells - use the CSS **border-spacing** property on the `<table>` element

#### Styling Columns in the Middle of a Table -  insert a empty (no styles) `<col>` element for the columns before

#### Hiding Columns - use **visibility: collapse** property






