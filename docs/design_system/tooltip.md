> Tooltips can convey additional context without interrupting a page layout or narrative flow.

Tooltips are applied through a combination of a class (i.e., `tooltip`) and data attribute (i.e., `data-tooltip`) on a given element.

# Indirect

Indirect tooltips are automated conversions of the `tooltip` class into a question mark icon.

```html|light,plain,span-3
<div>Example text <span class="tooltip processed" data-tooltip="I am a tooltip">?</span></div>
```

# Direct

Direct tooltips are applied to the element itself. Use the class `no-process` to prevent automated styling of the tooltip.

```html|light,plain,span-3
<a href="#" class="tooltip no-process" data-tooltip="I am a tooltip">Hover over me</a>
```

```hint|span-3
The method articulated here only creates the tooltip itself. Be sure to include some indication the element is interactive.
```
