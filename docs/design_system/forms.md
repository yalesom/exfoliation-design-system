# Default form elements
Standard form elements do have basic styles applied, however, **wrapped form elements** should be used wherever possible.
```html|plain,light,no-source
    <label class="form_label" for="form_input">Email Address</label>
    <input type="email" placeholder="your@email.com" id="form_input" name="form_input" value="" autocomplete="off" autocapitalize="off" spellcheck="false">
```
```html|plain,light,no-source
    <label class="form_label" for="form_select">Country</label>
    <select id="form_select" name="form_select" autocomplete="off" aria-required="true">
    <option value="UK">United Kingdom</option><option value="US">United States</option><option value="UY">Uruguay</option><option value="UZ">Uzbekistan</option><option value="NH">Vanuatu</option><option value="VT">Vatican City</option><option value="VE">Venezuela</option><option value="VM">Vietnam</option><option value="WF">Wallis and Futuna Islands</option><option value="WI">Western Sahara</option><option value="YM">Yemen</option><option value="ZA">Zambia</option><option value="ZI">Zimbabwe</option></select>
```

# Wrapped form elements
Wrapped form styles are defined by the label being visually contained in the form "element" and better :focus styles. This affect is achieved via class attached to the parent element.
## Text input
```html|plain,light
  <div class="form_text">
    <label class="form_label" for="form_input_wrapped">Email Address</label>
    <input type="email" placeholder="your@email.com" id="form_input_wrapped" name="form_input_wrapped" value="" autocomplete="off" autocapitalize="off" spellcheck="false">
  </div>
  <div class="form_text disabled">
    <label class="form_label" for="form_input_wrapped2">Email Address (disabled)</label>
    <input type="email" placeholder="your@email.com" id="form_input_wrapped2" name="form_input_wrapped2" value="" autocomplete="off" autocapitalize="off" spellcheck="false">
  </div>
```
Add `class="form_text"`

## Select
```html|plain,light
  <div class="form_select">
    <label class="form_label" for="form_select_wrapped">Country</label>
    <select id="form_select_wrapped" name="form_select_wrapped" autocomplete="off" aria-required="true">
    <option value="UK">United Kingdom</option><option value="US">United States</option><option value="UY">Uruguay</option><option value="UZ">Uzbekistan</option><option value="NH">Vanuatu</option><option value="VT">Vatican City</option><option value="VE">Venezuela</option><option value="VM">Vietnam</option><option value="WF">Wallis and Futuna Islands</option><option value="WI">Western Sahara</option><option value="YM">Yemen</option><option value="ZA">Zambia</option><option value="ZI">Zimbabwe</option></select>
  </div>
  <div class="form_select disabled">
    <label class="form_label" for="form_select_wrapped2">Country (disabled)</label>
    <select id="form_select_wrapped2" name="form_select_wrapped2" autocomplete="off" aria-required="true" disabled>
    <option value="UK">United Kingdom</option><option value="US">United States</option><option value="UY">Uruguay</option><option value="UZ">Uzbekistan</option><option value="NH">Vanuatu</option><option value="VT">Vatican City</option><option value="VE">Venezuela</option><option value="VM">Vietnam</option><option value="WF">Wallis and Futuna Islands</option><option value="WI">Western Sahara</option><option value="YM">Yemen</option><option value="ZA">Zambia</option><option value="ZI">Zimbabwe</option></select>
  </div>
```
Add `class="form_select"`

# Radios and checkboxes
Radio and checkbox inputs automatically receive style.
```hint|neutral
NOTE: `<label>` elements _must_ appear directly after `<input>` elements for the style to apply correctly.
```
```html|span-3,plain,light
<input id="form_radio" type="radio" data-text="Radio" name="form_radio" value="Radio" autocomplete="off" aria-required="true" data-handler-change="1"><label for="form_radio">Radio input</label>
<input id="form_radio2" type="radio" data-text="Radio" name="form_radio" value="Radio" autocomplete="off" aria-required="true" data-handler-change="1"><label for="form_radio2">Radio input</label>
```
```html|span-3,plain,light
<input id="form_checkbox" type="checkbox" data-text="Checkbox" name="form_checkbox" value="Checkbox" autocomplete="off" aria-required="true" data-handler-change="1"><label for="form_checkbox">Checkbox input</label>
<input id="form_checkbox2" type="checkbox" data-text="Checkbox" name="form_checkbox2" value="Checkbox2" autocomplete="off" aria-required="true" data-handler-change="1"><label for="form_checkbox2">Checkbox input</label>
```

# Form layout
Forms should be wrapped in a container with `class="form_page"` to render the form items with flexbox. Children of a flexbox layout will assume the same height of another item on the same row. Separate form elements into different `<fieldset>`s  to group related field types.
```hint
IMPORTANT: Because of a [Chrome bug](https://officereplacementparts.com/knoll-rpm-task-chair-arm-assemblies/), it is not possible to use `<fieldset>` with flexbox. Use `<div>` element for `form_page` instead.
```
```html|plain,light
<form>
  <div class="form_page">
    <div class="form_text">
      <label class="form_label" for="form_input_wrapped-1">First name</label>
      <input type="text" placeholder="Bill" id="form_input_wrapped" size="30" name="form_input_wrapped-1" value="" autocomplete="off" autocapitalize="off" spellcheck="false">
    </div>
    <div class="form_text">
      <label class="form_label" for="form_input_wrapped-2">M.I.</label>
      <input type="text" placeholder="S" id="form_input_wrapped-2" name="form_input_wrapped-2" size="1" value="" autocomplete="off" autocapitalize="off" spellcheck="false">
    </div>
    <div class="form_text">
      <label class="form_label" for="form_input_wrapped-3">Last name</label>
      <input type="text" placeholder="Preston" id="form_input_wrapped-3" name="form_input_wrapped-3" size="30" value="" autocomplete="off" autocapitalize="off" spellcheck="false">
    </div>
    <div class="form_text">
      <label class="form_label" for="form_input_wrapped-4">Suffix</label>
      <input type="text" placeholder="Esq." id="form_input_wrapped-4" name="form_input_wrapped-4" size="1" value="" autocomplete="off" autocapitalize="off" spellcheck="false">
    </div>
    <div class="form_text">
      <label class="form_label" for="form_input_wrapped-5">Email Address</label>
      <input type="email" placeholder="your@email.com" id="form_input_wrapped-5" name="form_input_wrapped-6" size="100" value="" autocomplete="off" autocapitalize="off" spellcheck="false">
    </div>
    <div class="form_select">
      <label class="form_label" for="form_select_wrapped-1">Country</label>
      <select id="form_select_wrapped-1" name="form_select_wrapped-1" size="1" autocomplete="off" aria-required="true">
      <option value="UK">United Kingdom</option><option value="US">United States</option><option value="UY">Uruguay</option><option value="UZ">Uzbekistan</option><option value="NH">Vanuatu</option><option value="VT">Vatican City</option><option value="VE">Venezuela</option><option value="VM">Vietnam</option><option value="WF">Wallis and Futuna Islands</option><option value="WI">Western Sahara</option><option value="YM">Yemen</option><option value="ZA">Zambia</option><option value="ZI">Zimbabwe</option></select>
    </div>
  </div>
  <fieldset>
    <legend>Is this form layout:</legend>
    <div class="form-radios">
      <input id="form_radio-1" type="radio" data-text="Radio" name="form_radio-1" value="Radio" autocomplete="off" aria-required="true" data-handler-change="1"><label for="form_radio-1">A great form</label>
      <input id="form_radio-2" type="radio" data-text="Radio" name="form_radio-1" value="Radio" autocomplete="off" aria-required="true" data-handler-change="1"><label for="form_radio-2">The greatest form</label>
    </div>
  </fieldset>
  <div class="form-actions">
    <button>Submit</button>
    <button class="reverse">Cancel</button>
  </div>
</form>
```
