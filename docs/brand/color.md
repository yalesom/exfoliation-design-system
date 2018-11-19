# Primary colors

## Blues
```color
span: 2
name: "Dark Blue (Brand)"
value: "#000440"
```
```color
span: 2
name: "Blue"
value: "#1069a0"
```
```color
span: 1
name: "Light Blue"
value: "#4ba5d7"
```
```color
span: 1
name: "Pale Blue"
value: "#a5d2eb"
```

## Neutrals
```color
span: 2
name: "Black"
value: "#14171a"
```
```color
span: 1
name: "Gray"
value: "#77706a"
```
```color
span: 1
name: "Light Gray"
value: "#a7a6a6"
```
```color
span: 1
name: "Border"
value: "#ddd"
```
```color
span: 1
name: "Tint Gray"
value: "#f6f6f6"
```

# Accent colors
Use sparingly.
```color
span: 2
name: "Orange (default)"
value: "#b16312"
```
```color
span: 1
name: "Green"
value: "#647f35"
```
```color
span: 1
name: "Red"
value: "#942d2d"
```
```color
span: 1
name: "Yellow"
value: "#d89d29"
```
```color
span: 1
name: "Purple"
value: "#7c2c94"
```

# Accessible color patterns
Required contrast ratio for [WCAG 2.0 AA compliance](https://www.w3.org/TR/UNDERSTANDING-WCAG20/visual-audio-contrast-contrast.html) is 4.5:1. This ensures that viewers who cannot see the full color spectrum are able to read the text.

The options below offer color palette combinations that fall within the range of Section 508 compliant foreground/background color contrast ratios.

## White backgrounds
```html|plain,span-3
<div class="accessible-color">
  <span style="color:#000440">White with brand blue text</span>
</div>
```
```html|plain,span-3
<div class="accessible-color">
  <span style="color:#1069a0">White with blue text</span>
</div>
```
```html|plain,span-3
<div class="accessible-color">
  <span style="color:#14171a">White with black text</span>
</div>
```
```html|plain,span-3
<div class="accessible-color">
  <span style="color:#77706a">White with gray text</span>
</div>
```
```html|plain,span-3
<div class="accessible-color">
  <span style="color:#b16312">White with orange text</span>
</div>
```
```html|plain,span-3
<div class="accessible-color">
  <span style="color:#647f35">White with green text</span>
</div>
```
```html|plain,span-3
<div class="accessible-color">
  <span style="color:#942d2d">White with red text</span>
</div>
```
```html|plain,span-3
<div class="accessible-color">
  <span style="color:#7c2c94">Purple with green text</span>
</div>
```
## Color backgrounds, blues
```html|plain,span-3
<div style="background:#000440" class="accessible-color">
  <span style="color:#fff">Brand blue with white text</span>
</div>
```
```html|plain,span-3
<div style="background:#000440" class="accessible-color">
  <span style="color:#a5d2eb">Brand blue with pale blue text</span>
</div>
```
```html|plain,span-3
<div style="background:#000440" class="accessible-color">
  <span style="color:#4ba5d7">Brand blue with light blue text</span>
</div>
```
```html|plain,span-3
<div style="background:#000440" class="accessible-color">
  <span style="color:#f6f6f6">Brand blue with tint gray text</span>
</div>
```
```html|plain,span-3
<div style="background:#000440" class="accessible-color">
  <span style="color:#a7a6a6">Brand blue with light gray text</span>
</div>
```
```html|plain,span-3
<div style="background:#1069a0" class="accessible-color">
  <span style="color:#fff">Blue with white text</span>
</div>
```
```html|plain,span-3
<div style="background:#1069a0" class="accessible-color">
  <span style="color:#f6f6f6">Blue with tint gray text</span>
</div>
```
```html|plain,span-3
<div style="background:#4ba5d7" class="accessible-color">
  <span style="color:#14171a">Light blue with black text</span>
</div>
```
```html|plain,span-3
<div style="background:#4ba5d7" class="accessible-color">
  <span style="color:#000440">Light blue with brand blue text</span>
</div>
```
```html|plain,span-3
<div style="background:#a5d2eb" class="accessible-color">
  <span style="color:#14171a">Tint blue with black text</span>
</div>
```
```html|plain,span-3
<div style="background:#a5d2eb" class="accessible-color">
  <span style="color:#000440">Tint blue with brand blue text</span>
</div>
```
## Color backgrounds, neutrals
```html|plain,span-3
<div style="background:#14171a" class="accessible-color">
  <span style="color:#fff">Black with white text</span>
</div>
```
```html|plain,span-3
<div style="background:#14171a" class="accessible-color">
  <span style="color:#a5d2eb">Black with pale blue text</span>
</div>
```
```html|plain,span-3
<div style="background:#14171a" class="accessible-color">
  <span style="color:#4ba5d7">Black with light blue text</span>
</div>
```
```html|plain,span-3
<div style="background:#14171a" class="accessible-color">
  <span style="color:#a7a6a6">Black with tint gray text</span>
</div>
```
```html|plain,span-3
<div style="background:#14171a" class="accessible-color">
  <span style="color:#a7a6a6">Black with light gray text</span>
</div>
```
```html|plain,span-3
<div style="background:#77706a" class="accessible-color">
  <span style="color:#fff">Gray with white text</span>
</div>
```
```html|plain,span-3
<div style="background:#77706a" class="accessible-color">
  <span style="color:#f6f6f6">Gray with tint gray text</span>
</div>
```
```html|plain,span-3
<div style="background:#a7a6a6" class="accessible-color">
  <span style="color:#000440">Light gray with brand blue text</span>
</div>
```
```html|plain,span-3
<div style="background:#a7a6a6" class="accessible-color">
  <span style="color:#14171a">Light gray with black text</span>
</div>
```
```html|plain,span-3
<div style="background:#f6f6f6" class="accessible-color">
  <span style="color:#1069a0">Tint gray with blue text</span>
</div>
```
```html|plain,span-3
<div style="background:#f6f6f6" class="accessible-color">
  <span style="color:#000440">Tint gray with brand blue text</span>
</div>
```
```html|plain,span-3
<div style="background:#f6f6f6" class="accessible-color">
  <span style="color:#14171a">Tint gray with black text</span>
</div>
```
```html|plain,span-3
<div style="background:#f6f6f6" class="accessible-color">
  <span style="color:#77706a">Tint gray with gray text</span>
</div>
```
## Color backgrounds, accents
```html|plain,span-3
<div style="background:#b16312" class="accessible-color">
  <span style="color:#fff">Orange with white text</span>
</div>
```
```html|plain,span-3
<div style="background:#647f35" class="accessible-color">
  <span style="color:#fff">Green with white text</span>
</div>
```
```html|plain,span-3
<div style="background:#942d2d" class="accessible-color">
  <span style="color:#fff">Red with white text</span>
</div>
```
```html|plain,span-3
<div style="background:#7c2c94" class="accessible-color">
  <span style="color:#fff">Purple with white text</span>
</div>
```
```html|plain,span-3
<div style="background:#d89d29" class="accessible-color">
  <span style="color:#14171a">Yellow with black text</span>
</div>
```
```hint
SCSS color adjustments (e.g., darken, lighten) are permissible to create variants for :focus states. Please be sure to verify the output [colors are accessible](http://accessible-colors.com/).
```