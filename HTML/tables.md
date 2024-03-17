### Rows - `<tr>`

### Headers (aka Columns) - `<th>`

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

- #### `<caption>` - gives the table a title; must be inserted immediately after the `<table>` tag.
- #### `<colgroup>` - specifies a group of one or more columns; useful for applying styles to entire columns. must be a **child** of a `<table>` element (AFTER any `<caption>` elements!)
    - ##### `<col>` - specifies properties for each column within a `<colgroup>` element; useful for applying styles to entire columns.
##### the following specify the parts of a `<table>` (header, body, footer)v and:
    + will not affect the table's layout (by default).
    + enable scrolling of the table body independently of the header and footer.  
- #### `<thead>` - groups the header content; must include 1 or more `<tr>` tags inside and be used as a **child** of a `<table>` element (AFTER any `<caption>` and `<colgroup>` elements!)
- #### `<tbody>` - groups the body content;
- #### `<tfoot>` - groups the footer content in a table