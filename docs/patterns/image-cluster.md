> An image cluster is a list of images that self adjust their size to maintain a single row.

```image|span-4,light
src: "yalesom/assets/patterns/2016-09-02-04.51.27-pm.png"
description: "Rendered example"
```
## Sample markup
```html|plain,light
responsive: ['Phone', 'Tablet', 'Desktop']
---
<ul class="image--cluster auto">
  <li><img alt=“Image description" src="/yalesom/assets/core/image-600x300.gif" /></li>
  <li><img alt=“Image description" src="/yalesom/assets/core/image-300x600.gif" /></li>
  <li><img alt=“Image description" src="/yalesom/assets/core/image-300x300.gif" /></li>
  </ul>
```
