> [Content layout][content layout] is a common pattern used for page and component structures.  

```html|no-source
responsive: ['Phone', 'Tablet', 'Desktop']
---
<div class="content-layout" style="background:#edf6fb;border:#edf6fb 10px solid;">
  <div class="content-layout__main" style="background:#fff;"><p class="epsilon">Main Content</p>
    <ul><li>content-layout__main</li></ul>
  </div>
  <div class="content-layout__aside content-layout__aside--primary content-layout__aside--wide-gutter" style="background:#fff;">
    <p class="epsilon">Primary Aside</p>
    <ul><li>content-layout__aside</li><li>content-layout__aside--primary</li><li>content-layout__aside--wide-gutter</li></ul>
  </div>
  <div class="content-layout__aside content-layout__aside--secondary" style="background:#fff;"><p class="epsilon">Secondary Aside</p>
  <ul><li>content-layout__aside</li><li>content-layout__aside--secondary</li></ul></div>
</div>
```
```code|collapsed
lang:html
---
<div class="content-layout">
  <div class="content-layout__main"></div>
  <div class="content-layout__aside content-layout__aside--primary content-layout__aside--wide-gutter"></div>
  <div class="content-layout__aside content-layout__aside--secondary">/div>
</div>
```

[content layout]: https://bitbucket.org/sq360_sysadmin/yale-som-theme/src/master/scss/layout/_content-layout.scss
