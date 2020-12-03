> [Content layout][content layout] is a common pattern used for page and component structures.

Layouts come in both **CSS grid** and **flexbox** flavors, depending on the requirements of the layout. Both versions use similar interior structures and class names.

# CSS Grid

Use for complex template layouts with defined regions. Additional classes are required on the container to correctly position the main content.

```html|
responsive: ['Phone', 'Tablet', 'Desktop']
---
<div class="content-layout content-layout--grid  content-layout--grid--has-navigation  content-layout--grid--has-aside">
  <article class="content-layout__main"><p class="epsilon">Main Content</p>
    <p>First element in DOM order, presentation order controlled by CSS. Use for primary page content, body field, etc.</p>
  </article>
  <div class="content-layout__main--extended"><p class="epsilon">Extended Content</p>
    <p>Second element in DOM order. Intended for additional narrative elements related to the main content that require more page width. </p>
    <div class="content-layout__main--extended--item">An standard region item, single column margin on both sides</div>
    <div class="content-layout__main--extended--item-wide">An full width region item, no margin on sides</div>
    <div class="content-layout__main--extended--item-edge">An edge-to-edge region item, negative margin to extend full browser width</div>
  </div>
  <aside class="content-layout__aside content-layout__aside--secondary"><p class="epsilon">Secondary Aside</p>
  <p>Use for relational page content.</p></aside>
  <div class="content-layout__aside content-layout__aside--primary content-layout__aside--wide-gutter">
    <p class="epsilon">Primary Aside</p>
    <p>Last element in DOM order. Primarily used for secondary page navigation, but may contain a limited number of content items. Optional CSS for a wide gutter <code>content-layout__aside--wide-gutter</code> to separate content from navigation </p>
  </div>
</div>
```

# Flexbox

Use for simpler, column-only layouts

```html|
responsive: ['Phone', 'Tablet', 'Desktop']
---
<div class="content-layout content-layout--flex">
  <article class="content-layout__main"><p class="epsilon">Main Content</p>
    <p>First element in DOM order, presentation order controlled by CSS. Use for primary page content, body field, etc.</p>
  </article>
  <aside class="content-layout__aside content-layout__aside--secondary"><p class="epsilon">Secondary Aside</p>
  <p>Use for relational page content.</p></aside>
  <div class="content-layout__aside content-layout__aside--primary content-layout__aside--wide-gutter">
    <p class="epsilon">Primary Aside</p>
    <p>Last element in DOM order. Primarily used for secondary page navigation, but may contain a limited number of content items. Optional CSS for a wide gutter <code>content-layout__aside--wide-gutter</code> to separate content from navigation </p>
  </div>
</div>
```

[content layout]: https://bitbucket.org/sq360_sysadmin/yale-som-theme/src/master/scss/components/_content-layout.scss
