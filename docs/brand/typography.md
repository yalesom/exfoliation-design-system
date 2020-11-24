# Typeface

## Neue Haas Unica Pro

Neue Haas Unica Pro is primarily used for headings, navigational elements and metadata. Italics are available, but rarely used.

```type|span-3,kern
{
  "headings": [
   { "label": "Normal", "value": 24},
  ],
  "background":"#f6f6f6",
  "font": "'NeueHaasUnicaPro', clean, sans-serif",
  "style": "normal",
  "weight":"300"
}
```

```type|span-3,kern
{
  "headings": [
   { "label": "Bold", "value": 24},
  ],
  "background":"#f6f6f6",
  "font": "'NeueHaasUnicaPro', clean, sans-serif",
  "style": "normal",
  "weight":"700"
}
```

## Yale Design

Yale's custom font is used for large spans of text, commonly paragraphs.

```type|span-3,kern
{
  "headings": [
   { "label": "Normal", "value": 24},
  ],
  "background":"#f6f6f6",
  "font": "'Yale', serif",
  "style": "normal",
  "weight":"300"
}
```

```type|span-3,kern
{
  "headings": [
   { "label": "Italic", "value": 24},
  ],
  "background":"#f6f6f6",
  "font": "'Yale', serif",
  "style": "italic",
  "weight":"300"
}
```

```type|span-3,kern
{
  "headings": [
   { "label": "Bold", "value": 24},
  ],
  "background":"#f6f6f6",
  "font": "'Yale', serif",
  "style": "normal",
  "weight":"700"
}
```

```type|span-3,kern
{
  "headings": [
   { "label": "Bold Italic", "value": 24},
  ],
  "background":"#f6f6f6",
  "font": "'Yale', serif",
  "style": "italic",
  "weight":"700"
}
```

# Sizes

Font sizes use a Greek symbol for basic sizes and metric prefixes at the extremes. See the [font-size variables][size] for reference.

```type|single
{
  "headings": [
   { "label": "Giga", "value": 96 },
   { "label": "Mega", "value": 85 },
   { "label": "Kilo", "value": 60 },
   { "label": "Alpha (H1)", "value": 38 },
   { "label": "Beta (H2)", "value": 30 },
   { "label": "Gamma (H3)", "value": 24 },
   { "label": "Delta (H4)", "value": 20 },
   { "label": "Epsilon (H5)", "value": 18 },
   { "label": "Zeta (H6)", "value": 16 },
   { "label": "Deci", "value": 14 },
   { "label": "Centi", "value": 13 },
   { "label": "Milli", "value": 12 },
   { "label": "Micro", "value": 11 },
   { "label": "Nano", "value": 10 }
  ],
  "background":"#000440",
  "color":"#fff",
  "font": "'NeueHaasUnicaPro', clean, sans-serif",
  "weight":"700"
}
```

```type|kafka
{
  "paragraphs": [
    { "label": "Paragraph", "value": "18/27" }
  ],
  "font": "'Yale', serif"
}
```

## Font scaling

Exfoliation uses [font scaling][scaling] to adjust a base font size relative to the screen width (i.e., breakpoint). Different breakpoints may use different size/scale relationships.

```hint|warning
Font scaling should **only** be used for larger headlines.
```

#### Font size calculator by breakpoint

```react|plain,light,no-source
state: {value: 38, scale: 1, breakpoint: 375}
---
<div>
<div class="form_page">
<div class="form_text">
  <label for="base_size">Base size</label>
  <input type="number" size="20" id="base_size" defaultValue={state.value} placeholder="Enter a base size" min="16" onChange={(e) => setState({value: e.target.value })}/>
</div>
<div class="form_text">
  <label for="scale_size">Scale</label>
  <input type="number" size="20" id="scale_size" defaultValue={state.scale} placeholder="Enter a scale" min="1" onChange={(e) => setState({scale: e.target.value })}/>
</div>
<div class="form_select">
  <label for="breakpoint">Base size</label>
  <select id="breakpoint" onChange={(e) => setState({breakpoint: e.target.value })} >
    <option value="375">Phone portrait</option>
    <option value="480">Phone landscape</option>
    <option value="720">Tablet portrait</option>
    <option value="800">Tablet landscape</option>
    <option value="1024">Desktop</option>
    <option value="1280">Big desktop</option>
  </select>
</div>
</div>
<p class="delta">
<span class="eta">( ( ({state.value}px / 16 ) - 0.875) * 16) + ( ({state.scale} / 100) * {state.breakpoint}px ) = </span><br/>
Approximately <strong>{Math.round( (((parseInt(state.value) / 16) - 0.875) * 16) + ((parseInt(state.scale)/100) * parseInt(state.breakpoint)) )}</strong> px</p>

</div>
```

[size]: https://bitbucket.org/sq360_sysadmin/yale-som-theme/src/master/scss/core/_fonts.scss
[scaling]: https://bitbucket.org/sq360_sysadmin/s360-fundamental-toolkit/src/master/scss/core/functions/_scale-font.scss
