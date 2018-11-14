# Striped table
Tables will use zebra stripes by default.

```html|plain,light,span-3
<table>
  <thead>
    <tr>
      <th>Header One</th>
      <th>Header Two</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Item One</td>
      <td>Item Two</td>
    </tr>
    <tr>
      <td>Item Three</td>
      <td>Item Four</td>
    </tr>
    <tr>
      <td>Item Five</td>
      <td>Item Six</td>
    </tr>
  </tbody>
  <caption>Striped table with top heading</caption>
</table>
```
```html|plain,light,span-3
<table>
  <tbody>
    <tr>
      <th scope="row">Header One</th>
      <td>Item One</td>
      <td>Item Two</td>
    </tr>
    <tr>
      <th scope="row">Header Two</th>
      <td>Item Three</td>
      <td>Item Four</td>
    </tr>
    <tr>
      <th scope="row">Header Three</th>
      <td>Item Five</td>
      <td>Item Six</td>
    </tr>
  </tbody>
  <caption>Striped table with left heading</caption>
</table>
```

# Plain table
Add `class="table--plain"` to any `<table>` to remove styling.
```html|plain,light
<table class="table--plain">
  <thead>
    <tr>
      <th>Header One</th>
      <th>Header Two</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Item One</td>
      <td>Item Two</td>
    </tr>
    <tr>
      <td>Item Three</td>
      <td>Item Four</td>
    </tr>
    <tr>
      <td>Item Five</td>
      <td>Item Six</td>
    </tr>
  </tbody>
  <caption>Plain table</caption>
</table>
```
