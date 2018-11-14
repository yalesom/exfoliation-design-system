# Standard buttons
Button classes can be applied to anchor links OR buttons ("light", "reverse", and "large" classes also require the “button" class). In addition, the "large" and "thin" classes may be combined with other class variants.
```html|span-6,plain,light
<button>Button</button> or <a href="#" class="button">Anchor</a>
<figcaption>Default</figcaption>
```
```html|span-2,plain,light
<button class="action">Button</button> or <a href="#" class="button action">Anchor</a>
<figcaption>Action</figcaption>
```
```html|span-2,plain,light
<button class="gray">Button</button>
<figcaption>Gray</figcaption>
```
```html|span-2,plain,light
<button class="outline">Button</button> or <a href="#" class="button outline">Anchor</a>
<figcaption>Outline</figcaption>
```
```html|span-2,plain,light
<button class="reverse">Button</button> or <a href="#" class="button reverse">Anchor</a>
<figcaption>Reverse</figcaption>
```
```html|span-2,plain,light
<button class="large">Button</button> or <a href="#" class="button large">Anchor</a>
<figcaption>Large</figcaption>
```
```html|span-2,plain,light
<button class="thin">Button</button> or <a href="#" class="button thin">Anchor</a>
<figcaption>Thin</figcaption>
```

# Paragraph links
```html|plain,light
<p>This is an example of a <a href="#">text link</a> in the context of a paragraph. </p>
```
Anchor links in paragraphs will receive the "block" link style by default.

```html|plain,light
<p><a href="#" class="arrow-right">Arrow link</a></p>
```
For an extra emphasis, arrow links add a button rollover effect and work best as a separate paragraph.

```html|plain,light
<a href="#" class="teaser-continue">Continue reading “Article”</a>
```
Continue links are typically used for article teasers and contain the full name of the article.
