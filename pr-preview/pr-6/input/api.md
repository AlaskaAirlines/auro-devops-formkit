<!-- AURO-GENERATED-CONTENT:START (FILE:src=../docs/api.md) -->
<!-- The below content is automatically added from ../docs/api.md -->

# auro-input

Generate unique names for dependency components.

## Properties

| Property                           | Attribute                         | Modifiers | Type                                             | Default     | Description                                      |
|------------------------------------|-----------------------------------|-----------|--------------------------------------------------|-------------|--------------------------------------------------|
| `a11yControls`                     | `a11yControls`                    |           | `string`                                         |             | The value for the aria-controls attribute.       |
| `a11yExpanded`                     | `a11yExpanded`                    |           | `boolean`                                        |             | The value for the aria-expanded attribute.       |
| `a11yRole`                         | `a11yRole`                        |           | `string`                                         |             | The value for the role attribute.                |
| [activeLabel](#activeLabel)                      | `activeLabel`                     |           | `boolean`                                        | false       | If set, the label will remain fixed in the active position. |
| [appearance](#appearance)                       | `appearance`                      |           | `string`                                         | "'default'" | Defines whether the component will be on lighter or darker backgrounds. |
| [autocapitalize](#autocapitalize)                   | `autocapitalize`                  |           | `string`                                         |             | An enumerated attribute that controls whether and how text input is automatically capitalized as it is entered/edited by the user. [off/none, on/sentences, words, characters]. |
| [autocomplete](#autocomplete)                     | `autocomplete`                    |           | `string`                                         |             | An enumerated attribute that defines what the user agent can suggest for autofill. At this time, only `autocomplete="off"` is supported. |
| [autocorrect](#autocorrect)                      | `autocorrect`                     |           | `string`                                         |             | When set to `off`, stops iOS from auto-correcting words when typed into a text box. |
| [commonDisplayValueWrapperClasses](#commonDisplayValueWrapperClasses) |                                   | readonly  | `{ [x: string]: boolean; displayValueWrapper: boolean; }` |             |                                                  |
| [customValidityTypeEmail](#customValidityTypeEmail)          | `customValidityTypeEmail`         |           | `string`                                         |             | Custom help text message for email type validity. |
| [disabled](#disabled)                         | `disabled`                        |           | `boolean`                                        | false       | If set, disables the input.                      |
| [dvInputOnly](#dvInputOnly)                      | `dvInputOnly`                     |           | `boolean`                                        | false       | If defined, the display value slot content will only mask the HTML5 input element. The input's label will not be masked. |
| [error](#error)                            | `error`                           |           | `string`                                         |             | When defined, sets persistent validity to `customError` and sets `setCustomValidity` = attribute value. |
| [errorMessage](#errorMessage)                     | `errorMessage`                    |           | `string`                                         |             | Contains the help text message for the current validity error. |
| [format](#format)                           | `format`                          |           | `string`                                         |             | Specifies the input mask format.                 |
| [icon](#icon)                             | `icon`                            |           | `boolean`                                        | false       | If set, will render an icon inside the input to the left of the value. Support is limited to auro-input instances with credit card format. |
| [id](#id)                               | `id`                              |           | `string`                                         |             | The id global attribute defines an identifier (ID) which must be unique in the whole document. |
| [inputmode](#inputmode)                        | `inputmode`                       |           | `string`                                         |             | Exposes inputmode attribute for input.           |
| [lang](#lang)                             | `lang`                            |           | `string`                                         |             | Defines the language of an element.              |
| [max](#max)                              | `max`                             |           | `string`                                         | "undefined" | The maximum value allowed. This only applies for inputs with a type of `number` and all date formats. |
| [maxLength](#maxLength)                        | `maxLength`                       |           | `number`                                         | "undefined" | The maximum number of characters the user can enter into the text input. This must be an integer value `0` or higher. |
| [min](#min)                              | `min`                             |           | `string`                                         | "undefined" | The minimum value allowed. This only applies for inputs with a type of `number` and all date formats. |
| [minLength](#minLength)                        | `minLength`                       |           | `number`                                         | "undefined" | The minimum number of characters the user can enter into the text input. This must be a non-negative integer value smaller than or equal to the value specified by `maxlength`. |
| [name](#name)                             | `name`                            |           | `string`                                         |             | Populates the `name` attribute on the input.     |
| [nested](#nested)                           | `nested`                          |           | `boolean`                                        |             | Sets styles for nested operation - removes borders, hides help + error text, and<br />hides accents. |
| [noValidate](#noValidate)                       | `noValidate`                      |           | `boolean`                                        | false       | If set, disables auto-validation on blur.        |
| [onDark](#onDark)                           | `onDark`                          |           | `boolean`                                        | false       | DEPRECATED - use `appearance` instead.           |
| [pattern](#pattern)                          | `pattern`                         |           | `string`                                         |             | Specifies a regular expression the form control's value should match. |
| [placeholder](#placeholder)                      | `placeholder`                     |           | `string`                                         |             | Define custom placeholder text.                  |
| [readonly](#readonly)                         | `readonly`                        |           | `boolean`                                        |             | Makes the input read-only, but can be set programmatically. |
| [required](#required)                         | `required`                        |           | `boolean`                                        | false       | Populates the `required` attribute on the input. Used for client-side validation. |
| [setCustomValidity](#setCustomValidity)                | `setCustomValidity`               |           | `string`                                         |             | Sets a custom help text message to display for all validityStates. |
| [setCustomValidityBadInput](#setCustomValidityBadInput)        | `setCustomValidityBadInput`       |           | `string`                                         |             | Custom help text message to display when validity = `badInput`. |
| [setCustomValidityCustomError](#setCustomValidityCustomError)     | `setCustomValidityCustomError`    |           | `string`                                         |             | Custom help text message to display when validity = `customError`. |
| [setCustomValidityForType](#setCustomValidityForType)         | `setCustomValidityForType`        |           | `string`                                         | "undefined" | Custom help text message to display for the declared element `type` and type validity fails. |
| [setCustomValidityRangeOverflow](#setCustomValidityRangeOverflow)   | `setCustomValidityRangeOverflow`  |           | `string`                                         |             | Custom help text message to display when validity = `rangeOverflow`. |
| [setCustomValidityRangeUnderflow](#setCustomValidityRangeUnderflow)  | `setCustomValidityRangeUnderflow` |           | `string`                                         |             | Custom help text message to display when validity = `rangeUnderflow`. |
| [setCustomValidityTooLong](#setCustomValidityTooLong)         | `setCustomValidityTooLong`        |           | `string`                                         |             | Custom help text message to display when validity = `tooLong`. |
| [setCustomValidityTooShort](#setCustomValidityTooShort)        | `setCustomValidityTooShort`       |           | `string`                                         |             | Custom help text message to display when validity = `tooShort`. |
| [setCustomValidityValueMissing](#setCustomValidityValueMissing)    | `setCustomValidityValueMissing`   |           | `string`                                         |             | Custom help text message to display when validity = `valueMissing`. |
| [simple](#simple)                           | `simple`                          |           | `boolean`                                        |             | Simple makes the input render without a border.  |
| [spellcheck](#spellcheck)                       | `spellcheck`                      |           | `string`                                         |             | An enumerated attribute defines whether the element may be checked for spelling errors. [true, false]. When set to `false` the attribute `autocorrect` is set to `off` and `autocapitalize` is set to `none`. |
| [type](#type)                             | `type`                            |           | `string`                                         |             | Populates the `type` attribute on the input. Allowed values are `password`, `email`, `credit-card`, `date`, `tel` or `text`. If given value is not allowed or set, defaults to `text`. |
| [validateOnInput](#validateOnInput)                  | `validateOnInput`                 |           | `boolean`                                        |             | Sets validation mode to re-eval with each input. |
| [validity](#validity)                         | `validity`                        |           | `string`                                         |             | Specifies the `validityState` this element is in. |
| [value](#value)                            | `value`                           |           | `string`                                         |             | Populates the `value` attribute on the input. Can also be read to retrieve the current value of the input. |

## Methods

| Method     | Type                                   | Description                                      |
|------------|----------------------------------------|--------------------------------------------------|
| [clear](#clear)    | `(): void`                             | Clears the input value.                          |
| [focus](#focus)    | `(): void`                             | Function to set element focus.                   |
| [reset](#reset)    | `(): void`                             | Resets component to initial state, including resetting the touched state and validity. |
| [validate](#validate) | `(force?: boolean \| undefined): void` | Validates value.<br /><br />**force**: Whether to force validation. |

## Events

| Event                       | Type               | Description                                      |
|-----------------------------|--------------------|--------------------------------------------------|
| `auroFormElement-validated` |                    | Notifies that the `validity` and `errorMessage` value has changed. |
| `auroInput-validityChange`  | `CustomEvent<any>` |                                                  |
| [input](#input)                     | `InputEvent`       | Event fires when the value of an `auro-input` has been changed. |

## Slots

| Name                      | Description                                      |
|---------------------------|--------------------------------------------------|
| `ariaLabel.clear`         | Sets aria-label on clear button for screen reader to read |
| `ariaLabel.password.hide` | Sets aria-label on password button to toggle off showing password |
| `ariaLabel.password.show` | Sets aria-label on password button to toggle on showing password |
| [displayValue](#displayValue)            | Allows custom HTML content to display in place of the value when the input is not focused. |
| [helpText](#helpText)                | Sets the help text displayed below the input.    |
| [label](#label)                   | Sets the label text for the input.               |
| [optionalLabel](#optionalLabel)           | Allows overriding the optional display text "(optional)", which appears next to the label. |

## CSS Shadow Parts

| Part            | Description                                      |
|-----------------|--------------------------------------------------|
| `accent-left`   | Use for customizing the style of the left accent element (e.g. padding, margin) |
| `accent-right`  | Use for customizing the style of the right accent element (e.g. padding, margin) |
| [accentIcon](#accentIcon)    | Use for customizing the style of the accentIcon element (e.g. credit card icon, calendar icon) |
| [helpText](#helpText)      | Use for customizing the style of the helpText element |
| [iconContainer](#iconContainer) | Use for customizing the style of the iconContainer (e.g. X icon for clearing input value) |
| [input](#input)         | Use for customizing the style of the input element |
| [label](#label)         | Use for customizing the style of the label element |
| [wrapper](#wrapper)       | Use for customizing the style of the root element |
<!-- AURO-GENERATED-CONTENT:END -->

# API Examples

## Localization Support

The `auro-input` element supports the localization of all content managed within the scope of the element. This DOES NOT include any custom content placed in the `slot` element.

<auro-radio-group required horizontal>
  <span slot="legend">Use the options here to toggle between languages</span>
  <auro-radio id="enButton" name="langDemo" value="en" checked>English</auro-radio>
  <auro-radio id="esButton" name="langDemo" value="es">Spanish</auro-radio>
</auro-radio-group>

## Basic

The default component supports the basic input `type="text"` structure. The `(optional)` label is provided to instruct the user that their input is not required. Use the `bordered` attribute for a bordered `<auro-input>`.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/basic.html) -->
  <!-- The below content is automatically added from ./../apiExamples/basic.html -->
  <auro-input>
    <span slot="ariaLabel.clear">Clear All</span>
    <span slot="label">Label</span>
    <span slot="helpText">Help Text</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearance.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearance.html -->
  <auro-input appearance="inverse">
    <span slot="label">Label</span>
    <span slot="helpText">Help Text</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/basic.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/basic.html -->

```html
<auro-input>
  <span slot="ariaLabel.clear">Clear All</span>
  <span slot="label">Label</span>
  <span slot="helpText">Help Text</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/inverseAppearance.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/inverseAppearance.html -->

```html
<auro-input appearance="inverse">
  <span slot="label">Label</span>
  <span slot="helpText">Help Text</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

## Attribute Examples

### Disabled <a name="disabled"></a>
Use the `disable` attribute to prevent the user from interacting with the input.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/disabled.html) -->
  <!-- The below content is automatically added from ./../apiExamples/disabled.html -->
  <auro-input disabled type="date">
    <span slot="label">Disabled</span>
    <span slot="helpText">Help Text</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceDisabled.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearanceDisabled.html -->
  <auro-input appearance="inverse" disabled type="date">
    <span slot="label">Arrival date</span>
    <span slot="helpText">Help Text</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/disabled.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/disabled.html -->

```html
<auro-input disabled type="date">
  <span slot="label">Disabled</span>
  <span slot="helpText">Help Text</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/inverseAppearanceDisabled.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/inverseAppearanceDisabled.html -->

```html
<auro-input appearance="inverse" disabled type="date">
  <span slot="label">Arrival date</span>
  <span slot="helpText">Help Text</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### Input Mode

Set the input mode for the input.

*IMPORTANT:* If you are also passing a `type`, most browsers will use the `type` attribute to determine what keyboard to display on mobile devices and ignore the `inputmode` attribute.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inputmode.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inputmode.html -->
  <auro-input inputmode="tel">
    <span slot="label">Telephone</span>
    <span slot="helpText">Help Text</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/inputmode.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/inputmode.html -->

```html
<auro-input inputmode="tel">
  <span slot="label">Telephone</span>
  <span slot="helpText">Help Text</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Placeholder <a name="placeholder"></a>
Use the `placeholder` attribute to add a custom placeholder message within the element.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/placeholder.html) -->
  <!-- The below content is automatically added from ../apiExamples/placeholder.html -->
  <auro-input placeholder="John Doe" required>
    <span slot="label">Full name</span>
    <span slot="helpText">Please enter your full name.</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/placeholder.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/placeholder.html -->

```html
<auro-input placeholder="John Doe" required>
  <span slot="label">Full name</span>
  <span slot="helpText">Please enter your full name.</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Value <a name="value"></a>
Use the `value` attribute to programmatically set the value of the input.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/programmaticValue.html) -->
  <!-- The below content is automatically added from ../apiExamples/programmaticValue.html -->
  <auro-input value="Alaska Airlines is the best!">
    <span slot="label">Name</span>
    <span slot="helpText">Please enter your full name.</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/programmaticValue.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/programmaticValue.html -->

```html
<auro-input value="Alaska Airlines is the best!">
  <span slot="label">Name</span>
  <span slot="helpText">Please enter your full name.</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### Dynamically Set Value

Use the `value` and other components to dynamically set the value of the input.

Note: Setting the `value` to `undefined` will also reset the element.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/value.html) -->
  <!-- The below content is automatically added from ../apiExamples/value.html -->
  <auro-button id="setValidValueBtn">Set Value to Alaska</auro-button>
  <auro-button id="setUndefinedValueBtn">Set Value to Undefined</auro-button>
  <br /><br />
  <auro-input id="setProgrammaticValueExample" value="Press one of the buttons above!">
    <span slot="label">Name</span>
    <span slot="helpText">Please enter your full name.</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/value.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/value.html -->

```html
<auro-button id="setValidValueBtn">Set Value to Alaska</auro-button>
<auro-button id="setUndefinedValueBtn">Set Value to Undefined</auro-button>
<br /><br />
<auro-input id="setProgrammaticValueExample" value="Press one of the buttons above!">
  <span slot="label">Name</span>
  <span slot="helpText">Please enter your full name.</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/value.js) -->
<!-- The below code snippet is automatically added from ../apiExamples/value.js -->

```js
export function programmaticallySetValue() {
  const elem = document.querySelector('#setProgrammaticValueExample');

  // set value of auro-input element
  document.querySelector('#setValidValueBtn').addEventListener('click', () => {
    elem.value = "Alaska Airlines is the best";
  });

  // reset the value of auro-input element
  document.querySelector('#setUndefinedValueBtn').addEventListener('click', () => {
    elem.value = undefined;
  });
}
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Max <a name="max"></a>
Use the `max` attribute to define a maximum value used during validation. The attribute will only apply when `<auro-input>` also has a `type` attribute for `number` or any date format.

The `setCustomValidityRangeOverflow` attribute may optionally be used in combination with the `max` attribute to define custom help text used when the input value is greater than the value of the `max` attribute.

#### Date Example

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/maxDate.html) -->
  <!-- The below content is automatically added from ../apiExamples/maxDate.html -->
  <auro-input type="date" max="03/25/2023" setCustomValidityRangeOverflow="The selected date is past the defined maximum date.">
    <span slot="label">Choose a date</span>
    <span slot="helpText">Help Text</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/maxDate.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/maxDate.html -->

```html
<auro-input type="date" max="03/25/2023" setCustomValidityRangeOverflow="The selected date is past the defined maximum date.">
  <span slot="label">Choose a date</span>
  <span slot="helpText">Help Text</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### Number Example

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/maxNumber.html) -->
  <!-- The below content is automatically added from ../apiExamples/maxNumber.html -->
  <auro-input type="number" max="10" setCustomValidityRangeOverflow="The selected value is above the defined maximum.">
    <span slot="label">Choose a number</span>
    <span slot="helpText">Help Text</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/maxNumber.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/maxNumber.html -->

```html
<auro-input type="number" max="10" setCustomValidityRangeOverflow="The selected value is above the defined maximum.">
  <span slot="label">Choose a number</span>
  <span slot="helpText">Help Text</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Min <a name="min"></a>
Use the `min` attribute to define a minimum value used during validation. The attribute will only apply when `<auro-input>` also has a `type` attribute for `number` or any date format.

The `setCustomValidityRangeUnderflow` attribute may optionally be used in combination with the `min` attribute to define custom help text used when the input value is less than the value of the `min` attribute.

#### Date Example

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/minDate.html) -->
  <!-- The below content is automatically added from ../apiExamples/minDate.html -->
  <auro-input type="date" min="03/25/2023" setCustomValidityRangeUnderflow="The selected date is before the defined minimum date.">
    <span slot="label">Choose a date</span>
    <span slot="helpText">Help Text</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/minDate.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/minDate.html -->

```html
<auro-input type="date" min="03/25/2023" setCustomValidityRangeUnderflow="The selected date is before the defined minimum date.">
  <span slot="label">Choose a date</span>
  <span slot="helpText">Help Text</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### Number Example

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/minNumber.html) -->
  <!-- The below content is automatically added from ../apiExamples/minNumber.html -->
  <auro-input type="number" min="10" setCustomValidityRangeUnderflow="The selected value is below the defined minimum.">
    <span slot="label">Choose a number</span>
    <span slot="helpText">Help Text</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/minNumber.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/minNumber.html -->

```html
<auro-input type="number" min="10" setCustomValidityRangeUnderflow="The selected value is below the defined minimum.">
  <span slot="label">Choose a number</span>
  <span slot="helpText">Help Text</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Max Length <a name="maxLength"></a>
Use the `maxlength` attribute to control the length of the input entered.

The `setCustomValidityTooLong` attribute may optionally be used in combination with the `maxLength` attribute to define custom help text used when the length of the input is too long.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/maxLength.html) -->
  <!-- The below content is automatically added from ../apiExamples/maxLength.html -->
  <auro-input maxlength="12" setCustomValidityTooLong="Oops! There were too many characters entered." required>
    <span slot="label">Voucher Code</span>
    <span slot="helpText">Please enter your 12 character voucher code.</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/maxLength.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/maxLength.html -->

```html
<auro-input maxlength="12" setCustomValidityTooLong="Oops! There were too many characters entered." required>
  <span slot="label">Voucher Code</span>
  <span slot="helpText">Please enter your 12 character voucher code.</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Min Length <a name="minLength"></a>
Use the `minlength` attribute to control the length of the input entered.

The `setCustomValidityTooShort` attribute may optionally be used in combination with the `minLength` attribute to define custom help text used when the length of the input is not long enough.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/minLength.html) -->
  <!-- The below content is automatically added from ../apiExamples/minLength.html -->
  <auro-input minlength="4" setCustomValidityTooShort="Please enter a full voucher code." required>
    <span slot="label">Voucher Code</span>
    <span slot="helpText">Please enter your 4 character voucher code.</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/minLength.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/minLength.html -->

```html
<auro-input minlength="4" setCustomValidityTooShort="Please enter a full voucher code." required>
  <span slot="label">Voucher Code</span>
  <span slot="helpText">Please enter your 4 character voucher code.</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Pattern <a name="pattern"></a>
Use the `pattern` attribute to set custom input validation. This example also uses the `spellcheck` attribute set to `false` which in turn sets `autocorrect` to `off` and `autocapitalize` to `none`. Additionally the `maxlength` attribute sets the maximum length of characters that can be entered.

The `<auro-input>` component supports setting a custom validity message specific to the pattern validation by using the `setCustomValidityPatternMismatch` attribute.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/pattern.html) -->
  <!-- The below content is automatically added from ../apiExamples/pattern.html -->
  <auro-input pattern="[a-z]{1,15}" spellcheck="false" setCustomValidityPatternMismatch="Only contain lowercase letters w/no spaces">
    <span slot="label">Username</span>
    <span slot="helpText">Please enter a username.</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/pattern.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/pattern.html -->

```html
<auro-input pattern="[a-z]{1,15}" spellcheck="false" setCustomValidityPatternMismatch="Only contain lowercase letters w/no spaces">
  <span slot="label">Username</span>
  <span slot="helpText">Please enter a username.</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Readonly <a name="readonly"></a>
Use the `readonly` attribute to prevent the user from editing the value of the input.

In this example, the user is able to programmatically change the value of the input by clicking the button or clear out the contents of the input.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/readonly.html) -->
  <!-- The below content is automatically added from ../apiExamples/readonly.html -->
  <auro-button id="setReadonlyValueBtn">Set Value to Auro Alaska</auro-button>
  <auro-button id="resetReadonlyValueBtn">Reset</auro-button>
  <br /><br />
  <auro-input readonly id="readonlyExample">
    <span slot="label">Name</span>
    <span slot="helpText">Please enter your full name.</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/readonly.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/readonly.html -->

```html
<auro-button id="setReadonlyValueBtn">Set Value to Auro Alaska</auro-button>
<auro-button id="resetReadonlyValueBtn">Reset</auro-button>
<br /><br />
<auro-input readonly id="readonlyExample">
  <span slot="label">Name</span>
  <span slot="helpText">Please enter your full name.</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/readonly.js) -->
<!-- The below code snippet is automatically added from ../apiExamples/readonly.js -->

```js
export function setReadonlyValue() {
  const elem = document.querySelector('#readonlyExample');

  // set value of auro-input element
  document.querySelector('#setReadonlyValueBtn').addEventListener('click', () => {
      elem.value = "Auro Alaska";
  });

  document.querySelector('#resetReadonlyValueBtn').addEventListener('click', () => {
    elem.value = undefined;
});
}
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Active Label <a name="activeLabel"></a>
Example use cases for auro-input support the `activeLabel` attribute. If set, the label will stay fixed in the active position.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/activeLabel.html) -->
  <!-- The below content is automatically added from ../apiExamples/activeLabel.html -->
  <auro-input activeLabel>
    <span slot="label">Address</span>
    <span slot="helpText">Please enter your home address.</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/activeLabel.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/activeLabel.html -->

```html
<auro-input activeLabel>
  <span slot="label">Address</span>
  <span slot="helpText">Please enter your home address.</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Disable auto-validation <a name="noValidate"></a>
For use cases where the field is `required`, but live validation is not wanted, use the `noValidate` attribute.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/noValidate.html) -->
  <!-- The below content is automatically added from ../apiExamples/noValidate.html -->
  <auro-input noValidate required>
    <span slot="label">Address</span>
    <span slot="helpText">Please enter your home address.</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/noValidate.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/noValidate.html -->

```html
<auro-input noValidate required>
  <span slot="label">Address</span>
  <span slot="helpText">Please enter your home address.</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Format <a name="format"></a>
Use the `format` attribute to set the format of the IMask. 

Default masking definitions:
- 0 : number
- a : letter
- \* : any character

See [IMask](https://imask.js.org/) for more information on how to configure a mask.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/format.html) -->
  <!-- The below content is automatically added from ../apiExamples/format.html -->
  <auro-input format="47440000">
    <span slot="label">Custom format</span>
    <span slot="helpText">Format is: 47440000</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/format.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/format.html -->

```html
<auro-input format="47440000">
  <span slot="label">Custom format</span>
  <span slot="helpText">Format is: 47440000</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

## Error support and HTML5 Validity

The `<auro-input>` component follows the HTML5 input `validity` and `validityState` [specification](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input#client-side_validation).

> if there is a form control that fails constraint validation, supporting browsers will display an error message on the first invalid form control; displaying a default message based on the error type, or a message set by you.

### Required <a name="required"></a>
When present, the `required` attribute specifies that an input field must be filled out before submitting the form.

When the validity check fails, the validityState equals `valueMissing`. The error message for the `valueMissing` validityState can be changed to a custom string using the `setCustomValidityValueMissing`.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/required.html) -->
  <!-- The below content is automatically added from ../apiExamples/required.html -->
  <auro-input required placeholder="John Doe">
    <span slot="label">Full name</span>
    <span slot="helpText">Please enter your full name.</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/required.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/required.html -->

```html
<auro-input required placeholder="John Doe">
  <span slot="label">Full name</span>
  <span slot="helpText">Please enter your full name.</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Custom optional label <a name="optionalLabel"></a>
The `<auro-input>` supports an `optionalLabel` slot, where users can can override the default `(optional)` notification text.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/optionalLabel.html) -->
  <!-- The below content is automatically added from ./../apiExamples/optionalLabel.html -->
  <auro-input placeholder="John Doe" bordered>
    <span slot="label">Full name</span>
    <span slot="optionalLabel" style="color: grey; font-size: small"> - optional</span>
    <span slot="helpText">Please enter your full name.</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/optionalLabel.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/optionalLabel.html -->

```html
<auro-input placeholder="John Doe" bordered>
  <span slot="label">Full name</span>
  <span slot="optionalLabel" style="color: grey; font-size: small"> - optional</span>
  <span slot="helpText">Please enter your full name.</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Validation on input <a name="validateOnInput"></a>
Use the `validateOnInput` attribute to enable live validation on the `input` event. Recommended use is with setting a custom `pattern` and validation is required prior to a `blur` event.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/validateOnInput.html) -->
  <!-- The below content is automatically added from ../apiExamples/validateOnInput.html -->
  <auro-input validateOnInput required pattern="[a-zA-Z-.']+( +[a-zA-Z-.']+)+" setCustomValidityPatternMismatch="Full name requires two or more names with at least one space.">
    <span slot="label">Full Name</span>
    <span slot="helpText">Please enter your full name as it appears on the card.</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/validateOnInput.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/validateOnInput.html -->

```html
<auro-input validateOnInput required pattern="[a-zA-Z-.']+( +[a-zA-Z-.']+)+" setCustomValidityPatternMismatch="Full name requires two or more names with at least one space.">
  <span slot="label">Full Name</span>
  <span slot="helpText">Please enter your full name as it appears on the card.</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### setCustomValidity <a name="setCustomValidity"></a>
The `setCustomValidity` attribute can be used to set a custom string for all validityStates. When the component is first loaded, if this attribute is set on the element, all validityStates (except `valid`) will display the defined message.

**NOTE:** Custom strings are NOT localized. It is the responsibility of the element consumer to provide localized strings when using this element property.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/setCustomValidity.html) -->
  <!-- The below content is automatically added from ../apiExamples/setCustomValidity.html -->
  <auro-input required minlength="3" setCustomValidity="Sorry, please enter your first and last name (one space required).">
    <span slot="label">Full Name</span>
    <span slot="helpText">Please enter your full name.</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/setCustomValidity.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/setCustomValidity.html -->

```html
<auro-input required minlength="3" setCustomValidity="Sorry, please enter your first and last name (one space required).">
  <span slot="label">Full Name</span>
  <span slot="helpText">Please enter your full name.</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Error <a name="error"></a>
Use the `error` attribute to apply a persistent custom error that supersedes the HTML5 validation logic.

A custom error message can be set using the `error` attribute, or it can be used in conjuction with the `setCustomValidityCustomError` attribute.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/error.html) -->
  <!-- The below content is automatically added from ../apiExamples/error.html -->
  <auro-button id="setCustomErrorBtn">Set Custom Error</auro-button>
  <auro-button id="setCustomErrorClearBtn">Clear Custom Error</auro-button>
  <br /><br />
  <auro-input id="setCustomErrorExample" error="Initial error attribute value">
    <span slot="label">Name</span>
    <span slot="helpText">Please enter your full name.</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/error.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/error.html -->

```html
<auro-button id="setCustomErrorBtn">Set Custom Error</auro-button>
<auro-button id="setCustomErrorClearBtn">Clear Custom Error</auro-button>
<br /><br />
<auro-input id="setCustomErrorExample" error="Initial error attribute value">
  <span slot="label">Name</span>
  <span slot="helpText">Please enter your full name.</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/error.js) -->
<!-- The below code snippet is automatically added from ../apiExamples/error.js -->

```js
export function customError() {
  const elem = document.querySelector('#setCustomErrorExample');
  // set custom error
  document.querySelector('#setCustomErrorBtn').addEventListener('click', () => {
    elem.error = "Custom Error Message";
  });

  // remove custom error
  document.querySelector('#setCustomErrorClearBtn').addEventListener('click', () => {
    elem.removeAttribute('error');
  });
}
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### Visual state on dark backgrounds

<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/inverseAppearanceError.html) -->
  <!-- The below content is automatically added from ../apiExamples/inverseAppearanceError.html -->
  <auro-button appearance="inverse" id="setCustomErrorBtnOnDark">Set Custom Error</auro-button>
  <auro-button appearance="inverse" id="setCustomErrorClearBtnOnDark">Clear Custom Error</auro-button>
  <br /><br />
  <auro-input appearance="inverse" id="setCustomErrorExampleOnDark" error="Initial error attribute value">
    <span slot="label">Name</span>
    <span slot="helpText">Please enter your full name.</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/inverseAppearanceError.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/inverseAppearanceError.html -->

```html
<auro-button appearance="inverse" id="setCustomErrorBtnOnDark">Set Custom Error</auro-button>
<auro-button appearance="inverse" id="setCustomErrorClearBtnOnDark">Clear Custom Error</auro-button>
<br /><br />
<auro-input appearance="inverse" id="setCustomErrorExampleOnDark" error="Initial error attribute value">
  <span slot="label">Name</span>
  <span slot="helpText">Please enter your full name.</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/inverseAppearanceError.js) -->
<!-- The below code snippet is automatically added from ../apiExamples/inverseAppearanceError.js -->

```js
export function customErrorOnDark() {
  const elem = document.querySelector('#setCustomErrorExampleOnDark');
  // set custom error
  document.querySelector('#setCustomErrorBtnOnDark').addEventListener('click', () => {
    elem.error = "Custom Error Message";
  });

  // remove custom error
  document.querySelector('#setCustomErrorClearBtnOnDark').addEventListener('click', () => {
    elem.removeAttribute('error');
  });
}
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

## Types

### Password

Use the `type="password"` attribute for a password style input. The hide/show password feature will automatically appear once a user begins to enter data.

Default help text will be added to the input `type="password"` if custom help text is not provided. See the example below.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/password.html) -->
  <!-- The below content is automatically added from ../apiExamples/password.html -->
  <auro-input type="password" required>
    <span slot="ariaLabel.clear">Clear All</span>
    <span slot="ariaLabel.password.show">Show</span>
    <span slot="ariaLabel.password.hide">Hide</span>
    <span slot="label">Password</span>
    <span slot="helpText">Please enter a secure password.</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/inverseAppearancePassword.html) -->
  <!-- The below content is automatically added from ../apiExamples/inverseAppearancePassword.html -->
  <auro-input appearance="inverse" type="password" required>
    <span slot="label">Password</span>
    <span slot="helpText">Please enter a secure password.</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/inverseAppearancePassword.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/inverseAppearancePassword.html -->

```html
<auro-input appearance="inverse" type="password" required>
  <span slot="label">Password</span>
  <span slot="helpText">Please enter a secure password.</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Email

Use the `type="email"` attribute for a email style input. These examples illustrate the default error messaging per that browser. Content may vary.

Default help text will be added to the input `type="email"` if custom help text is not provided. See the example below.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/email.html) -->
  <!-- The below content is automatically added from ../apiExamples/email.html -->
  <auro-input type="email" required>
    <span slot="label">Email address</span>
    <span slot="helpText">Please enter your email address.</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/email.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/email.html -->

```html
<auro-input type="email" required>
  <span slot="label">Email address</span>
  <span slot="helpText">Please enter your email address.</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Number

Use the `type="number"` attribute for a numeric style input and invoke a numeric virtual keyboard on handheld devices.

This `number` input type should only be used for incremental numeric values, meaning values with decimals will be considered invalid. The `number` input type is not appropriate for values that happen to only consist of but aren't strictly speaking a number, such as postal codes in many countries or credit card numbers. See [MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input/number) for more information.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/number.html) -->
  <!-- The below content is automatically added from ../apiExamples/number.html -->
  <auro-input type="number" required>
    <span slot="label">Number of Passengers</span>
    <span slot="helpText">Please enter the number of passengers.</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/number.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/number.html -->

```html
<auro-input type="number" required>
  <span slot="label">Number of Passengers</span>
  <span slot="helpText">Please enter the number of passengers.</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Credit Card

Use the `type="credit-card"` attribute for a credit card formatted input.

Default help text will be added to the input `type="credit-card"` if custom help text is not provided. See the example below.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/creditCard.html) -->
  <!-- The below content is automatically added from ../apiExamples/creditCard.html -->
  <auro-input type="credit-card" required>
    <span slot="label">Card number</span>
    <span slot="helpText">Valid credit card numbers must include 16 digits (15 for Amex).</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/creditCard.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/creditCard.html -->

```html
<auro-input type="credit-card" required>
  <span slot="label">Card number</span>
  <span slot="helpText">Valid credit card numbers must include 16 digits (15 for Amex).</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>
Use the `type="credit-card"` and `icon` attributes for a credit card formatted input with credit card icon support.

**Dependency**: Please be sure to also install [auro-icon](https://auro.alaskaair.com/components/auro/icon/install) as a peer dependency.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/creditCardIcon.html) -->
  <!-- The below content is automatically added from ../apiExamples/creditCardIcon.html -->
  <auro-input icon type="credit-card" required>
    <span slot="label">Card number</span>
    <span slot="helpText">Valid credit card numbers must include 16 digits (15 for Amex).</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
// Use 4147 3411 1111 1111 to see the Alaska Airline's credit card!
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/creditCardIcon.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/creditCardIcon.html -->

```html
<auro-input icon type="credit-card" required>
  <span slot="label">Card number</span>
  <span slot="helpText">Valid credit card numbers must include 16 digits (15 for Amex).</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Phone Number

Use the `type="tel"` attribute for a phone number formatted input. The default format is `+1 (000) 000-0000`.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/tel.html) -->
  <!-- The below content is automatically added from ../apiExamples/tel.html -->
  <auro-input type="tel">
    <span slot="label">Telephone</span>
    <span slot="helpText">Help Text</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/tel.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/tel.html -->

```html
<auro-input type="tel">
  <span slot="label">Telephone</span>
  <span slot="helpText">Help Text</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### Formatting

Use the `format` attribute to set a custom phone number format.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/telFormat.html) -->
  <!-- The below content is automatically added from ../apiExamples/telFormat.html -->
  <auro-input type="tel" format="+22 999 99 9999">
    <span slot="label">Telephone</span>
    <span slot="helpText">Help Text</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/telFormat.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/telFormat.html -->

```html
<auro-input type="tel" format="+22 999 99 9999">
  <span slot="label">Telephone</span>
  <span slot="helpText">Help Text</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Date

Use the `type="date"` attribute for a date formatted input. The default date format is `mm/dd/yyyy`.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/monthDayYear.html) -->
  <!-- The below content is automatically added from ../apiExamples/monthDayYear.html -->
  <auro-input type="date">
    <span slot="label">Arrival date</span>
    <span slot="helpText">Help Text</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/monthDayYear.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/monthDayYear.html -->

```html
<auro-input type="date">
  <span slot="label">Arrival date</span>
  <span slot="helpText">Help Text</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### Formatting

Use the `format` attribute to put together any combination of `mm`, `dd`, & `yyyy` or `yy`.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/yearMonthDay.html) -->
  <!-- The below content is automatically added from ../apiExamples/yearMonthDay.html -->
  <auro-input type="date" format="yyyy/mm/dd">
    <span slot="label">Arrival date</span>
    <span slot="helpText">Help Text</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/yearMonthDay.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/yearMonthDay.html -->

```html
<auro-input type="date" format="yyyy/mm/dd">
  <span slot="label">Arrival date</span>
  <span slot="helpText">Help Text</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>
<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/monthYear.html) -->
  <!-- The below content is automatically added from ../apiExamples/monthYear.html -->
  <auro-input type="date" format="mm/yy">
    <span slot="label">Expiration date</span>
    <span slot="helpText">Help Text</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/monthYear.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/monthYear.html -->

```html
<auro-input type="date" format="mm/yy">
  <span slot="label">Expiration date</span>
  <span slot="helpText">Help Text</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>
<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/day.html) -->
  <!-- The below content is automatically added from ../apiExamples/day.html -->
  <auro-input type="date" format="dd">
    <span slot="label">Day</span>
    <span slot="helpText">Help Text</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/day.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/day.html -->

```html
<auro-input type="date" format="dd">
  <span slot="label">Day</span>
  <span slot="helpText">Help Text</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

## Additional Use Cases

### Reset State

Use the `reset()` method to reset the `<auro-input>`'s `value` and `validity` state. Doing so will preserve all other attributes and properties.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/resetState.html) -->
  <!-- The below content is automatically added from ../apiExamples/resetState.html -->
  <auro-button id="resetStateBtn">Reset</auro-button>
  <br /><br />
  <auro-input id="resetStateExample" minlength="12" value="Auro Team" setCustomValidityTooShort="Please enter your full name!">
    <span slot="label">Full Name</span>
    <span slot="helpText">Please enter your full name.</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/resetState.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/resetState.html -->

```html
<auro-button id="resetStateBtn">Reset</auro-button>
<br /><br />
<auro-input id="resetStateExample" minlength="12" value="Auro Team" setCustomValidityTooShort="Please enter your full name!">
  <span slot="label">Full Name</span>
  <span slot="helpText">Please enter your full name.</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/resetState.js) -->
<!-- The below code snippet is automatically added from ../apiExamples/resetState.js -->

```js
export function resetStateExample() {
  const elem = document.querySelector('#resetStateExample');

  document.querySelector('#resetStateBtn').addEventListener('click', () => {
    elem.reset();
  });
}
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Swapping Values Between Inputs

Example illustrates using a JavaScript function attached to an `auro-button` component `click` event to swap the values of two `auro-input` elements. An example of this use case would be swapping the departure and arrival airports in a flight search form.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/swapValue.html) -->
  <!-- The below content is automatically added from ../apiExamples/swapValue.html -->
  <auro-input id="swapExampleLeft">
    <span slot="label">Left Input</span>
    <span slot="helpText">Help Text</span>
  </auro-input>
  <auro-button id="swapExampleBtn">Swap Values</auro-button>
  <auro-input id="swapExampleRight">
    <span slot="label">Right Input</span>
    <span slot="helpText">Help Text</span>
  </auro-input>
  <style>
    #swapExampleWrapper {
      align-items: center;
    }

    #swapExampleLeft,
    #swapExampleRight {
      flex: 1;
    }

    #swapExampleBtn {
      width: unset;
      margin: 0 var(--auro-size-xs);
    }
  </style>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/swapValue.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/swapValue.html -->

```html
<auro-input id="swapExampleLeft">
  <span slot="label">Left Input</span>
  <span slot="helpText">Help Text</span>
</auro-input>
<auro-button id="swapExampleBtn">Swap Values</auro-button>
<auro-input id="swapExampleRight">
  <span slot="label">Right Input</span>
  <span slot="helpText">Help Text</span>
</auro-input>
<style>
  #swapExampleWrapper {
    align-items: center;
  }

  #swapExampleLeft,
  #swapExampleRight {
    flex: 1;
  }

  #swapExampleBtn {
    width: unset;
    margin: 0 var(--auro-size-xs);
  }
</style>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/swapValue.js) -->
<!-- The below code snippet is automatically added from ../apiExamples/swapValue.js -->

```js
export function swapInputValues() {
  const btn = document.querySelector('#swapExampleBtn');
  const inputOne = document.querySelector('#swapExampleLeft');
  const inputTwo = document.querySelector('#swapExampleRight');

  btn.addEventListener('click', () => {
    const valueOne = inputOne.value;
    const valueTwo = inputTwo.value;

    inputOne.value = valueTwo;
    inputTwo.value = valueOne;
  });
}
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

## Theme Support

The component may be restyled using the following code sample and changing the values of the following token(s).

<!-- AURO-GENERATED-CONTENT:START (CODE:src=../src/styles/tokens.scss) -->
<!-- The below code snippet is automatically added from ../src/styles/tokens.scss -->

```scss
/* stylelint-disable custom-property-empty-line-before */

@use "@aurodesignsystem/design-tokens/dist/themes/alaska/SCSSVariables--alaska" as v;

:host(:not([ondark])),
:host(:not([appearance="inverse"])) {
  --ds-auro-input-border-color: var(--ds-basic-color-border-bold, #{v.$ds-basic-color-border-bold});
  --ds-auro-input-container-color: var(--ds-basic-color-surface-default, #{v.$ds-basic-color-surface-default});
  --ds-auro-input-caret-color: var(--ds-advanced-color-state-focused, #{v.$ds-advanced-color-state-focused});
  --ds-auro-input-label-text-color: var(--ds-basic-color-texticon-muted, #{v.$ds-basic-color-texticon-muted});
  --ds-auro-input-placeholder-text-color: var(--ds-basic-color-texticon-default, #{v.$ds-basic-color-texticon-default});
  --ds-auro-input-text-color: var(--ds-basic-color-texticon-default, #{v.$ds-basic-color-texticon-default});
  --ds-auro-input-error-icon-color: var(--ds-basic-color-status-error, #{v.$ds-basic-color-status-error});

  --ds-auro-input-outline-color: transparent;
}

:host([ondark]),
:host([appearance="inverse"]) {
  --ds-auro-input-border-color: var(--ds-basic-color-border-inverse, #{v.$ds-basic-color-border-inverse});
  --ds-auro-input-container-color: var(--ds-advanced-color-shared-background-inverse, #{v.$ds-advanced-color-shared-background-inverse});
  --ds-auro-input-caret-color: var(--ds-advanced-color-state-focused-inverse, #{v.$ds-advanced-color-state-focused-inverse});
  --ds-auro-input-label-text-color: var(--ds-basic-color-texticon-inverse-muted, #{v.$ds-basic-color-texticon-inverse-muted});
  --ds-auro-input-placeholder-text-color: var(--ds-basic-color-texticon-inverse, #{v.$ds-basic-color-texticon-inverse});
  --ds-auro-input-text-color: var(--ds-basic-color-texticon-inverse, #{v.$ds-basic-color-texticon-inverse});
  --ds-auro-input-error-icon-color: var(--ds-advanced-color-state-error-inverse, #{v.$ds-advanced-color-state-error-inverse});

  --ds-auro-input-outline-color: transparent;
}
```
<!-- AURO-GENERATED-CONTENT:END -->
