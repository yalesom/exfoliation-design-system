> Headings are important to maintain a proper semantic structure independant of a desired style

Screen readers and assistive technologies rely on heading tags (`<h1> ` through `<h6>`) to identify headings. In most instances, the semantics and style of a heading will correlate. For instances where the desired presentation diverges, adding a [type-style class](#text-styles) (i.e., `beta`) to a heading will change the style and maintain the heirarchtical structure of the content.

```hint|warning
**Important:** Do NOT use heading tags for presentation style or skip tag levels in — such as jumping from `<h2>` to `<h5>` — to achieve a page design. Mixing heading levels is confusing for screen readers and other assistive technologies that skip from heading to heading.
```

# Heading tags

```html|span-3,showSource,plain,light
<h1>Heading 1</h1>
```

```html|span-3,showSource,plain,light
<h2>Heading 2</h2>
```

```html|span-3,showSource,plain,light
<h3>Heading 3</h3>
```

```html|span-3,showSource,plain,light
<h4>Heading 4</h4>
```

```html|span-3,showSource,plain,light
<h5>Heading 5</h5>
```

```html|span-3,showSource,plain,light
<h6>Heading 6</h6>
```

## Variant styles

```html|span-3,showSource,plain,light
<h2 class="sub-title">Page subtitle</h2>
```

```html|span-3,showSource,plain,light
<h2 class="intro">Page introduction</h2>
```

# Text styles

```html|span-3,showSource,plain,light
<h2 class="alpha">Alpha</h2>
```

```html|span-3,showSource,plain,light
<h2 class="beta">Beta</h2>
```

```html|span-3,showSource,plain,light
<h2 class="gamma">Gamma</h2>
```

```html|span-3,showSource,plain,light
<h2 class="delta">Delta</h2>
```

```html|span-3,showSource,plain,light
<h2 class="epsilon">Epsilon</h2>
```

```html|span-3,showSource,plain,light
<h2 class="zeta">Zeta</h2>
```
