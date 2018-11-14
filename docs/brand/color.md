# Primary colors

## Blues
```color
span: 3
name: "Dark Blue (Brand)"
value: "#000440"
```
```color
span: 2
name: "Blue"
value: "#1069A0"
```
```color
span: 1
name: "Light Blue"
value: "#4BA5D7"
```

## Neutrals
```color
span: 2
name: "Black"
value: "#14171A"
```
```color
span: 1
name: "Gray"
value: "#7c756e"
```
```color
span: 1
name: "Light Gray"
value: "#A7A6A6"
```
```color
span: 1
name: "White"
value: "#FFF"
```
```color
span: 1
name: "Border"
value: "#DDD"
```

# Accent colors
Use sparingly.
```color
span: 1
name: "Orange (default)"
value: "#C46D14"
```
```color
span: 1
name: "Green"
value: "#6C8A3A"
```
```color
span: 1
name: "Red"
value: "#942d2d"
```
```color
span: 1
name: "Yellow"
value: "#D89D29"
```
```color
span: 1
name: "Purple"
value: "#7C2C94"
```

# Tints and variants
Color variants are made programmatically in code via the [color function](https://bitbucket.org/sq360_sysadmin/yale-som-theme/src/master/scss/core/functions/_color.scss). Color variants include:
- tint: *lightens color by 90%*
- pale: *lightens color by 50%*
- fade: *add 10% white*
- dark: *add 10% black*
- shade: *darkens color by 10%*

In general, variants are used when the original color would create legibility issues or the original color does not sufficiently meet a use case. Gray and blue tints are commonly used for box style backgrounds.
```hint
Not all of these colors meet compliance with WCAG 2.0 contrast ratios. Be conscious of accessibility when selecting a variant.
```

## Examples
### Neutrals
```color-palette|horizontal
colors:
   - {name: "Tint",value: "#e8e8e8"}
   - {name: "Pale",value: "#8a8b8d"}
   - {name: "Fade",value: "#2a3137"}
   - {name: "Black (normal)",value: "#14171a"}
   - {name: "Shade",value: "#121517"}
   - {name: "Dark",value: "#000"}
```
```color-palette|horizontal
colors:
   - {name: "Tint",value: "#f2f1f1"}
   - {name: "Pale",value: "#bebab7"}
   - {name: "Fade",value: "#958f88"}
   - {name: "Gray (normal)",value: "#7c756e"}
   - {name: "Shade",value: "#706963"}
   - {name: "Dark",value: "#615c56"}
```
```color-palette|horizontal
colors:
   - {name: "Tint",value: "#f6f6f6"}
   - {name: "Pale",value: "#d3d3d3"}
   - {name: "Fade",value: "#c0c0c0"}
   - {name: "Light Gray (normal)",value: "#a7a6a6"}
   - {name: "Shade",value: "#969595"}
   - {name: "Dark",value: "#8e8c8c"}
```
### Blues
```color-palette|horizontal
colors:
   - {name: "Tint",value: "#e7f0f6"}
   - {name: "Pale",value: "#88b4d0"}
   - {name: "Fade",value: "#1587ce"}
   - {name: "Blue (normal)",value: "#1069a0"}
   - {name: "Shade",value: "#0e5f90"}
   - {name: "Dark",value: "#0b4b72"}
```
```color-palette|horizontal
colors:
   - {name: "Tint",value: "#edf6fb"}
   - {name: "Pale",value: "#a5d2eb"}
   - {name: "Fade",value: "#75bae0"}
   - {name: "Light Blue (normal)",value: "#4ba5d7"}
   - {name: "Shade",value: "#2b8dc4"}
   - {name: "Dark",value: "#4495c2"}
```

[Codepen](https://codepen.io/anon/pen/XBLZxW)
