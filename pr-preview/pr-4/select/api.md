<!--
The apiExamples.md file is a compiled document. No edits should be made directly to this file.

apiExamples.md is created by running `npm run build:markdownDocs`.

This file is generated based on a template fetched from `./docs/partials/apiExamples.md`
-->
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../docs/api.md) -->
<!-- The below content is automatically added from ./../docs/api.md -->

# auro-select

The auro-select element is a wrapper for auro-dropdown and auro-menu to create a dropdown menu control.

## Properties

| Property                        | Attribute                       | Type                              | Default        | Description                                      |
|---------------------------------|---------------------------------|-----------------------------------|----------------|--------------------------------------------------|
| [appearance](#appearance)                    | `appearance`                    | `string`                          | "'default'"    | Defines whether the component will be on lighter or darker backgrounds. |
| [autoPlacement](#autoPlacement)                 | `autoPlacement`                 | `boolean`                         | "false"        | If declared, bib's position will be automatically calculated where to appear. |
| [autocomplete](#autocomplete)                  | `autocomplete`                  | `string`                          |                | If declared, sets the autocomplete attribute for the select element. |
| [disabled](#disabled)                      | `disabled`                      | `boolean`                         |                | When attribute is present, element shows disabled state. |
| [error](#error)                         | `error`                         | `string`                          |                | When defined, sets persistent validity to `customError` and sets `setCustomValidity` = attribute value. |
| [fluid](#fluid)                         | `fluid`                         | `boolean`                         |                | When attribute is present, element will be 100% width of container element. |
| [forceDisplayValue](#forceDisplayValue)             | `forceDisplayValue`             | `boolean`                         | false          | If declared, the label and value will be visually hidden and the displayValue will render 100% of the time. |
| [fullscreenBreakpoint](#fullscreenBreakpoint)          | `fullscreenBreakpoint`          | `string`                          | "sm"           | Defines the screen size breakpoint (`xs`, `sm`, `md`, `lg`, `xl`, `disabled`)<br />at which the dropdown switches to fullscreen mode on mobile. `disabled` indicates a dropdown should _never_ enter fullscreen.<br /><br />When expanded, the dropdown will automatically display in fullscreen mode<br />if the screen size is equal to or smaller than the selected breakpoint. |
| [largeFullscreenHeadline](#largeFullscreenHeadline)       | `largeFullscreenHeadline`       | `boolean`                         |                | If declared, make bib.fullscreen.headline in HeadingDisplay.<br />Otherwise, Heading 600. |
| [layout](#layout)                        |                                 | `string`                          |                |                                                  |
| [matchWidth](#matchWidth)                    | `matchWidth`                    | `boolean`                         | false          | If declared, the popover and trigger will be set to the same width. |
| [multiSelect](#multiSelect)                   | `multiselect`                   | `boolean`                         |                | Sets multi-select mode, allowing multiple options to be selected at once. |
| [name](#name)                          | `name`                          | `string`                          |                | The name for the select element.                 |
| [noCheckmark](#noCheckmark)                   | `noCheckmark`                   | `boolean`                         |                | When true, checkmark on selected option will no longer be present. |
| [noFlip](#noFlip)                        | `noFlip`                        | `boolean`                         | "false"        | If declared, the bib will NOT flip to an alternate position<br />when there isn't enough space in the specified `placement`. |
| [noValidate](#noValidate)                    | `noValidate`                    | `boolean`                         |                | If set, disables auto-validation on blur.        |
| [offset](#offset)                        | `offset`                        | `number`                          | "0"            | Gap between the trigger element and bib.         |
| [onDark](#onDark)                        | `onDark`                        | `boolean`                         |                | DEPRECATED - use `appearance` instead.           |
| [optionSelected](#optionSelected)                | `optionSelected`                | `HTMLElement\|Array<HTMLElement>` |                | Specifies the current selected menuOption. Default type is `HTMLElement`, changing to `Array<HTMLElement>` when `multiSelect` is true. |
| [placeholder](#placeholder)                   | `placeholder`                   | `string`                          |                | Define custom placeholder text.                  |
| [placement](#placement)                     | `placement`                     | `string`                          | "bottom-start" | Position where the bib should appear relative to the trigger.<br />Accepted values:<br />"top" \| "right" \| "bottom" \| "left" \|<br />"bottom-start" \| "top-start" \| "top-end" \|<br />"right-start" \| "right-end" \| "bottom-end" \|<br />"left-start" \| "left-end". |
| [required](#required)                      | `required`                      | `boolean`                         |                | Populates the `required` attribute on the element. Used for client-side validation. |
| [setCustomValidity](#setCustomValidity)             | `setCustomValidity`             | `string`                          |                | Sets a custom help text message to display for all validityStates. |
| [setCustomValidityCustomError](#setCustomValidityCustomError)  | `setCustomValidityCustomError`  | `string`                          |                | Custom help text message to display when validity = `customError`. |
| [setCustomValidityValueMissing](#setCustomValidityValueMissing) | `setCustomValidityValueMissing` | `string`                          |                | Custom help text message to display when validity = `valueMissing`. |
| [shift](#shift)                         | `shift`                         | `boolean`                         | "false"        | If set, the dropdown will shift its position to avoid being cut off by the viewport. |
| [validity](#validity)                      | `validity`                      | `string`                          |                | Specifies the `validityState` this element is in. |
| [value](#value)                         | `value`                         | `string`                          |                | Value selected for the component.                |

## Methods

| Method         | Type                                   | Description                                      |
|----------------|----------------------------------------|--------------------------------------------------|
| [hideBib](#hideBib)      | `(): void`                             | Hides the dropdown bib if its open.              |
| [reset](#reset)        | `(): void`                             | Resets component to initial state.               |
| [setMenuValue](#setMenuValue) | `(value: any): void`                   |                                                  |
| [showBib](#showBib)      | `(): void`                             | Shows the dropdown bib if there are options to show. |
| [validate](#validate)     | `(force?: boolean \| undefined): void` | Validates value.<br /><br />**force**: Whether to force validation. |

## Events

| Event                       | Type                                             | Description                                      |
|-----------------------------|--------------------------------------------------|--------------------------------------------------|
| `auroFormElement-validated` |                                                  | Notifies that the `validity` and `errorMessage` values have changed. |
| `auroSelect-valueSet`       | `CustomEvent<any>`                               | Notifies that the component has a new value set. |
| [input](#input)                     | `CustomEvent<{ optionSelected: any; value: any; }>` | Notifies every time the value prop of the element is changed. The updated `value` and `optionSelected` will be delivered in `detail` object. |

## Slots

| Name                      | Description                                      |
|---------------------------|--------------------------------------------------|
|                           | Default slot for the menu content.               |
| `ariaLabel.bib.close`     | Sets aria-label on close button in fullscreen bib |
| `bib.fullscreen.headline` | Defines the headline to display above menu-options |
| [displayValue](#displayValue)            | Allows custom HTML content to display the selected value when select is not focused. |
| [helpText](#helpText)                | Defines the content of the helpText.             |
| [label](#label)                   | Defines the content of the label.                |
| [optionalLabel](#optionalLabel)           | Allows overriding the optional display text "(optional)", which appears next to the label. |
| [valueText](#valueText)               | Dropdown value text display.                     |

## CSS Shadow Parts

| Part              | Description                                      |
|-------------------|--------------------------------------------------|
| [dropdownChevron](#dropdownChevron) | Apply CSS to the collapsed/expanded state icon container. |
| [dropdownSize](#dropdownSize)    | Apply size styles to the dropdown bib. (height, width, maxHeight, maxWidth only) |
| [dropdownTrigger](#dropdownTrigger) | Apply CSS to the trigger content container.      |
| [helpText](#helpText)        | Apply CSS to the help text.                      |
<!-- AURO-GENERATED-CONTENT:END -->

## API Examples

### Default example

A baseline `auro-select` using `auro-menu` and `auro-menuoption` elements.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/basic.html) -->
  <!-- The below content is automatically added from ./../apiExamples/basic.html -->
  <auro-select>
    <span slot="ariaLabel.bib.close">Close Popup</span>
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Select Example</span>
    <auro-menu>
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearance.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearance.html -->
  <auro-select appearance="inverse">
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Select Example</span>
    <auro-menu>
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/basic.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/basic.html -->

```html
<auro-select>
  <span slot="ariaLabel.bib.close">Close Popup</span>
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Select Example</span>
  <auro-menu>
    <auro-menuoption value="stops">Stops</auro-menuoption>
    <auro-menuoption value="price">Price</auro-menuoption>
    <auro-menuoption value="duration">Duration</auro-menuoption>
    <auro-menuoption value="departure">Departure</auro-menuoption>
    <auro-menuoption value="arrival">Arrival</auro-menuoption>
    <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
  </auro-menu>
</auro-select>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearance.html) -->
<!-- The below content is automatically added from ./../apiExamples/inverseAppearance.html -->
<auro-select appearance="inverse">
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Select Example</span>
  <auro-menu>
    <auro-menuoption value="stops">Stops</auro-menuoption>
    <auro-menuoption value="price">Price</auro-menuoption>
    <auro-menuoption value="duration">Duration</auro-menuoption>
    <auro-menuoption value="departure">Departure</auro-menuoption>
    <auro-menuoption value="arrival">Arrival</auro-menuoption>
    <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
  </auro-menu>
</auro-select>
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Property Examples

#### value <a name="value"></a>
Use the `value` property to define a preset value on the `auro-select` element. The `value` of `auro-select` must match the `value` defined of a single `auro-menuoption`. Upon initially rendering the component, if the `value` does not match an `auro-menuoption`, the `value` of `auro-select` will be set to `undefined`.

To pre-set the value of auro-select on load, use the `value` property. The `selected` attribute on auro-menuoption is designed to illustrate state in the DOM.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/value.html) -->
  <!-- The below content is automatically added from ./../apiExamples/value.html -->
  <auro-button id="validValueExampleBtn">Set Value to Valid Option</auro-button>
  <auro-button id="invalidValueExampleBtn">Set Value to Invalid Option</auro-button>
  <br/><br/>
  <auro-select id="valueExample" multiselect value='["price", "duration"]'>
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption id="option-0" value="stops">Stops</auro-menuoption>
      <auro-menuoption id="option-1" value="price">Price</auro-menuoption>
      <auro-menuoption id="option-2" value="duration">Duration</auro-menuoption>
      <auro-menuoption id="option-3" value="departure">Departure</auro-menuoption>
      <auro-menuoption id="option-4" value="arrival">Arrival</auro-menuoption>
      <auro-menuoption id="option-5" value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/value.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/value.html -->

```html
<auro-button id="validValueExampleBtn">Set Value to Valid Option</auro-button>
<auro-button id="invalidValueExampleBtn">Set Value to Invalid Option</auro-button>
<br/><br/>
<auro-select id="valueExample" multiselect value='["price", "duration"]'>
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Name</span>
  <auro-menu>
    <auro-menuoption id="option-0" value="stops">Stops</auro-menuoption>
    <auro-menuoption id="option-1" value="price">Price</auro-menuoption>
    <auro-menuoption id="option-2" value="duration">Duration</auro-menuoption>
    <auro-menuoption id="option-3" value="departure">Departure</auro-menuoption>
    <auro-menuoption id="option-4" value="arrival">Arrival</auro-menuoption>
    <auro-menuoption id="option-5" value="prefer alaska">Prefer Alaska</auro-menuoption>
  </auro-menu>
</auro-select>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/value.js) -->
<!-- The below code snippet is automatically added from ./../apiExamples/value.js -->

```js
export function valueExample() {
  const valueExample = document.querySelector('#valueExample');

  document.querySelector('#validValueExampleBtn').addEventListener('click', () => {
    valueExample.value = '["arrival", "prefer alaska"]';
  });

  document.querySelector('#invalidValueExampleBtn').addEventListener('click', () => {
    valueExample.value = '["flight course"]';
  });
}
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### Autocomplete <a name="autocomplete"></a>
Use the `autocomplete` attribute to let browser's know what information to use to fill out the form.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/autocomplete.html) -->
  <!-- The below content is automatically added from ./../apiExamples/autocomplete.html -->
  <div class="autofill-example-form">
    <div class="input-row">
      <auro-input autocomplete="given-name">
        <span slot="label">First Name</span>
        <span slot="bib.fullscreen.headline">First Name</span>
      </auro-input>
      <auro-input autocomplete="family-name">
        <span slot="label">Last Name</span>
        <span slot="bib.fullscreen.headline">Last Name</span>
      </auro-input>
    </div>
    <div class="input-row">
      <auro-input autocomplete="address-line1">
        <span slot="label">Street Address</span>
        <span slot="bib.fullscreen.headline">Street Address</span>
      </auro-input>
      <auro-input autocomplete="address-level2">
        <span slot="label">City</span>
        <span slot="bib.fullscreen.headline">City</span>
      </auro-input>
      <auro-select autocomplete="address-level1">
        <span slot="bib.fullscreen.headline">Select Your State</span>
        <span slot="label">Select Your State</span>
        <auro-menu>
          <auro-menuoption value="AL">Alabama</auro-menuoption>
          <auro-menuoption value="AK">Alaska</auro-menuoption>
          <auro-menuoption value="AZ">Arizona</auro-menuoption>
          <auro-menuoption value="AR">Arkansas</auro-menuoption>
          <auro-menuoption value="CA">California</auro-menuoption>
          <auro-menuoption value="CO">Colorado</auro-menuoption>
          <auro-menuoption value="CT">Connecticut</auro-menuoption>
          <auro-menuoption value="DE">Delaware</auro-menuoption>
          <auro-menuoption value="DC">District of Columbia</auro-menuoption>
          <auro-menuoption value="FL">Florida</auro-menuoption>
          <auro-menuoption value="GA">Georgia</auro-menuoption>
          <auro-menuoption value="HI">Hawaii</auro-menuoption>
          <auro-menuoption value="ID">Idaho</auro-menuoption>
          <auro-menuoption value="IL">Illinois</auro-menuoption>
          <auro-menuoption value="IN">Indiana</auro-menuoption>
          <auro-menuoption value="IA">Iowa</auro-menuoption>
          <auro-menuoption value="KS">Kansas</auro-menuoption>
          <auro-menuoption value="KY">Kentucky</auro-menuoption>
          <auro-menuoption value="LA">Louisiana</auro-menuoption>
          <auro-menuoption value="ME">Maine</auro-menuoption>
          <auro-menuoption value="MD">Maryland</auro-menuoption>
          <auro-menuoption value="MA">Massachusetts</auro-menuoption>
          <auro-menuoption value="MI">Michigan</auro-menuoption>
          <auro-menuoption value="MN">Minnesota</auro-menuoption>
          <auro-menuoption value="MS">Mississippi</auro-menuoption>
          <auro-menuoption value="MO">Missouri</auro-menuoption>
          <auro-menuoption value="MT">Montana</auro-menuoption>
          <auro-menuoption value="NE">Nebraska</auro-menuoption>
          <auro-menuoption value="NV">Nevada</auro-menuoption>
          <auro-menuoption value="NH">New Hampshire</auro-menuoption>
          <auro-menuoption value="NJ">New Jersey</auro-menuoption>
          <auro-menuoption value="NM">New Mexico</auro-menuoption>
          <auro-menuoption value="NY">New York</auro-menuoption>
          <auro-menuoption value="NC">North Carolina</auro-menuoption>
          <auro-menuoption value="ND">North Dakota</auro-menuoption>
          <auro-menuoption value="OH">Ohio</auro-menuoption>
          <auro-menuoption value="OK">Oklahoma</auro-menuoption>
          <auro-menuoption value="OR">Oregon</auro-menuoption>
          <auro-menuoption value="PA">Pennsylvania</auro-menuoption>
          <auro-menuoption value="RI">Rhode Island</auro-menuoption>
          <auro-menuoption value="SC">South Carolina</auro-menuoption>
          <auro-menuoption value="SD">South Dakota</auro-menuoption>
          <auro-menuoption value="TN">Tennessee</auro-menuoption>
          <auro-menuoption value="TX">Texas</auro-menuoption>
          <auro-menuoption value="UT">Utah</auro-menuoption>
          <auro-menuoption value="VT">Vermont</auro-menuoption>
          <auro-menuoption value="VA">Virginia</auro-menuoption>
          <auro-menuoption value="WA">Washington</auro-menuoption>
          <auro-menuoption value="WV">West Virginia</auro-menuoption>
          <auro-menuoption value="WI">Wisconsin</auro-menuoption>
          <auro-menuoption value="WY">Wyoming</auro-menuoption>
        </auro-menu>
      </auro-select>
    </div>
  </div>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/autocomplete.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/autocomplete.html -->

```html
<div class="autofill-example-form">
  <div class="input-row">
    <auro-input autocomplete="given-name">
      <span slot="label">First Name</span>
      <span slot="bib.fullscreen.headline">First Name</span>
    </auro-input>
    <auro-input autocomplete="family-name">
      <span slot="label">Last Name</span>
      <span slot="bib.fullscreen.headline">Last Name</span>
    </auro-input>
  </div>
  <div class="input-row">
    <auro-input autocomplete="address-line1">
      <span slot="label">Street Address</span>
      <span slot="bib.fullscreen.headline">Street Address</span>
    </auro-input>
    <auro-input autocomplete="address-level2">
      <span slot="label">City</span>
      <span slot="bib.fullscreen.headline">City</span>
    </auro-input>
    <auro-select autocomplete="address-level1">
      <span slot="bib.fullscreen.headline">Select Your State</span>
      <span slot="label">Select Your State</span>
      <auro-menu>
        <auro-menuoption value="AL">Alabama</auro-menuoption>
        <auro-menuoption value="AK">Alaska</auro-menuoption>
        <auro-menuoption value="AZ">Arizona</auro-menuoption>
        <auro-menuoption value="AR">Arkansas</auro-menuoption>
        <auro-menuoption value="CA">California</auro-menuoption>
        <auro-menuoption value="CO">Colorado</auro-menuoption>
        <auro-menuoption value="CT">Connecticut</auro-menuoption>
        <auro-menuoption value="DE">Delaware</auro-menuoption>
        <auro-menuoption value="DC">District of Columbia</auro-menuoption>
        <auro-menuoption value="FL">Florida</auro-menuoption>
        <auro-menuoption value="GA">Georgia</auro-menuoption>
        <auro-menuoption value="HI">Hawaii</auro-menuoption>
        <auro-menuoption value="ID">Idaho</auro-menuoption>
        <auro-menuoption value="IL">Illinois</auro-menuoption>
        <auro-menuoption value="IN">Indiana</auro-menuoption>
        <auro-menuoption value="IA">Iowa</auro-menuoption>
        <auro-menuoption value="KS">Kansas</auro-menuoption>
        <auro-menuoption value="KY">Kentucky</auro-menuoption>
        <auro-menuoption value="LA">Louisiana</auro-menuoption>
        <auro-menuoption value="ME">Maine</auro-menuoption>
        <auro-menuoption value="MD">Maryland</auro-menuoption>
        <auro-menuoption value="MA">Massachusetts</auro-menuoption>
        <auro-menuoption value="MI">Michigan</auro-menuoption>
        <auro-menuoption value="MN">Minnesota</auro-menuoption>
        <auro-menuoption value="MS">Mississippi</auro-menuoption>
        <auro-menuoption value="MO">Missouri</auro-menuoption>
        <auro-menuoption value="MT">Montana</auro-menuoption>
        <auro-menuoption value="NE">Nebraska</auro-menuoption>
        <auro-menuoption value="NV">Nevada</auro-menuoption>
        <auro-menuoption value="NH">New Hampshire</auro-menuoption>
        <auro-menuoption value="NJ">New Jersey</auro-menuoption>
        <auro-menuoption value="NM">New Mexico</auro-menuoption>
        <auro-menuoption value="NY">New York</auro-menuoption>
        <auro-menuoption value="NC">North Carolina</auro-menuoption>
        <auro-menuoption value="ND">North Dakota</auro-menuoption>
        <auro-menuoption value="OH">Ohio</auro-menuoption>
        <auro-menuoption value="OK">Oklahoma</auro-menuoption>
        <auro-menuoption value="OR">Oregon</auro-menuoption>
        <auro-menuoption value="PA">Pennsylvania</auro-menuoption>
        <auro-menuoption value="RI">Rhode Island</auro-menuoption>
        <auro-menuoption value="SC">South Carolina</auro-menuoption>
        <auro-menuoption value="SD">South Dakota</auro-menuoption>
        <auro-menuoption value="TN">Tennessee</auro-menuoption>
        <auro-menuoption value="TX">Texas</auro-menuoption>
        <auro-menuoption value="UT">Utah</auro-menuoption>
        <auro-menuoption value="VT">Vermont</auro-menuoption>
        <auro-menuoption value="VA">Virginia</auro-menuoption>
        <auro-menuoption value="WA">Washington</auro-menuoption>
        <auro-menuoption value="WV">West Virginia</auro-menuoption>
        <auro-menuoption value="WI">Wisconsin</auro-menuoption>
        <auro-menuoption value="WY">Wyoming</auro-menuoption>
      </auro-menu>
    </auro-select>
  </div>
</div>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### required <a name="required"></a>
When present, the `required` attribute specifies that a select field must be filled out before submitting the form.

When the validity check fails the validityState, equals `valueMissing`. The error message for the `valueMissing` validityState can be set to a custom string using the `setCustomValidityValueMissing`. There is no default error message defined.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/required.html) -->
  <!-- The below content is automatically added from ./../apiExamples/required.html -->
  <auro-select required setCustomValidityValueMissing="Custom required validation error message." placeholder="Placeholder Text">
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Label</span>
    <auro-menu>
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/required.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/required.html -->

```html
<auro-select required setCustomValidityValueMissing="Custom required validation error message." placeholder="Placeholder Text">
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Label</span>
  <auro-menu>
    <auro-menuoption value="stops">Stops</auro-menuoption>
    <auro-menuoption value="price">Price</auro-menuoption>
    <auro-menuoption value="duration">Duration</auro-menuoption>
    <auro-menuoption value="departure">Departure</auro-menuoption>
    <auro-menuoption value="arrival">Arrival</auro-menuoption>
    <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
  </auro-menu>
</auro-select>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Custom optional label <a name="optionalLabel"></a>
The `<auro-select>` supports an `optionalLabel` slot, where users can can override the default `(optional)` notification text.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/optionalLabel.html) -->
  <!-- The below content is automatically added from ./../apiExamples/optionalLabel.html -->
  <auro-select>
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Please select a preference</span>
    <span slot="optionalLabel" style="color: grey; font-size: small"> - optional</span>
    <auro-menu>
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/optionalLabel.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/optionalLabel.html -->

```html
<auro-select>
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Please select a preference</span>
  <span slot="optionalLabel" style="color: grey; font-size: small"> - optional</span>
  <auro-menu>
    <auro-menuoption value="stops">Stops</auro-menuoption>
    <auro-menuoption value="price">Price</auro-menuoption>
    <auro-menuoption value="duration">Duration</auro-menuoption>
    <auro-menuoption value="departure">Departure</auro-menuoption>
    <auro-menuoption value="arrival">Arrival</auro-menuoption>
    <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
  </auro-menu>
</auro-select>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### error <a name="error"></a>
Use the `error` boolean attribute to toggle the error UI.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/error.html) -->
  <!-- The below content is automatically added from ./../apiExamples/error.html -->
  <auro-select error="Custom error message" placeholder="Placeholder Text">
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Label</span>
    <auro-menu>
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceError.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearanceError.html -->
  <auro-select appearance="inverse" error="Custom error message" placeholder="Placeholder Text">
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Label</span>
    <auro-menu>
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/error.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/error.html -->

```html
<auro-select error="Custom error message" placeholder="Placeholder Text">
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Label</span>
  <auro-menu>
    <auro-menuoption value="stops">Stops</auro-menuoption>
    <auro-menuoption value="price">Price</auro-menuoption>
    <auro-menuoption value="duration">Duration</auro-menuoption>
    <auro-menuoption value="departure">Departure</auro-menuoption>
    <auro-menuoption value="arrival">Arrival</auro-menuoption>
    <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
  </auro-menu>
</auro-select>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceError.html) -->
<!-- The below content is automatically added from ./../apiExamples/inverseAppearanceError.html -->
<auro-select appearance="inverse" error="Custom error message" placeholder="Placeholder Text">
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Label</span>
  <auro-menu>
    <auro-menuoption value="stops">Stops</auro-menuoption>
    <auro-menuoption value="price">Price</auro-menuoption>
    <auro-menuoption value="duration">Duration</auro-menuoption>
    <auro-menuoption value="departure">Departure</auro-menuoption>
    <auro-menuoption value="arrival">Arrival</auro-menuoption>
    <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
  </auro-menu>
</auro-select>
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### disabled <a name="disabled"></a>
Use the `disabled` boolean attribute to toggle the disabled UI.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/disabled.html) -->
  <!-- The below content is automatically added from ./../apiExamples/disabled.html -->
  <auro-select disabled placeholder="Placeholder Text">
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Label</span>
    <auro-menu>
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceDisabled.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearanceDisabled.html -->
  <auro-select appearance="inverse" disabled placeholder="Placeholder Text">
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Label</span>
    <auro-menu>
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/disabled.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/disabled.html -->

```html
<auro-select disabled placeholder="Placeholder Text">
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Label</span>
  <auro-menu>
    <auro-menuoption value="stops">Stops</auro-menuoption>
    <auro-menuoption value="price">Price</auro-menuoption>
    <auro-menuoption value="duration">Duration</auro-menuoption>
    <auro-menuoption value="departure">Departure</auro-menuoption>
    <auro-menuoption value="arrival">Arrival</auro-menuoption>
    <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
  </auro-menu>
</auro-select>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceDisabled.html) -->
<!-- The below content is automatically added from ./../apiExamples/inverseAppearanceDisabled.html -->
<auro-select appearance="inverse" disabled placeholder="Placeholder Text">
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Label</span>
  <auro-menu>
    <auro-menuoption value="stops">Stops</auro-menuoption>
    <auro-menuoption value="price">Price</auro-menuoption>
    <auro-menuoption value="duration">Duration</auro-menuoption>
    <auro-menuoption value="departure">Departure</auro-menuoption>
    <auro-menuoption value="arrival">Arrival</auro-menuoption>
    <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
  </auro-menu>
</auro-select>
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### multiselect <a name="multiselect"></a>
Sets multi-select mode, allowing multiple options to be selected at once.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/multiselect.html) -->
  <!-- The below content is automatically added from ./../apiExamples/multiselect.html -->
  <auro-select multiselect>
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <label slot="placeholder">Select one or more options</label>
    <span slot="label">multiselect select example</span>
    <auro-menu>
      <auro-menuoption value="1">Option 1</auro-menuoption>
      <auro-menuoption value="2">Option 2</auro-menuoption>
      <auro-menuoption value="3">Option 3</auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/multiselect.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/multiselect.html -->

```html
<auro-select multiselect>
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <label slot="placeholder">Select one or more options</label>
  <span slot="label">multiselect select example</span>
  <auro-menu>
    <auro-menuoption value="1">Option 1</auro-menuoption>
    <auro-menuoption value="2">Option 2</auro-menuoption>
    <auro-menuoption value="3">Option 3</auro-menuoption>
  </auro-menu>
</auro-select>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### flexMenuWidth <a name="flexMenuWidth"></a>
Use the `flexMenuWidth` boolean attribute to toggle the width of the `<auro-select>` element to match the width of the bib content, rather than the width of the trigger.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/flexMenuWidth.html) -->
  <!-- The below content is automatically added from ../apiExamples/flexMenuWidth.html -->
  <auro-select flexMenuWidth id="flexMenuWidthExample" placeholder="Placeholder Text">
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Label</span>
    <auro-menu>
      <auro-menuoption value="united states">United States has a country code of (+1)</auro-menuoption>
      <auro-menuoption value="costa rica">Costa Rica has a country code of (+506)</auro-menuoption>
      <auro-menuoption value="mexico">Mexico has a country code of (+52)</auro-menuoption>
      <auro-menuoption value="afghanistan">Afghanistan has a country code of (+93)</auro-menuoption>
      <auro-menuoption value="albania">Albania has a country code of (+355)</auro-menuoption>
    </auro-menu>
  </auro-select>
  <style>
    #flexMenuWidthExample::part(dropdownTrigger) {
      width: 25%;
    }
  </style>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/flexMenuWidth.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/flexMenuWidth.html -->

```html
<auro-select flexMenuWidth id="flexMenuWidthExample" placeholder="Placeholder Text">
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Label</span>
  <auro-menu>
    <auro-menuoption value="united states">United States has a country code of (+1)</auro-menuoption>
    <auro-menuoption value="costa rica">Costa Rica has a country code of (+506)</auro-menuoption>
    <auro-menuoption value="mexico">Mexico has a country code of (+52)</auro-menuoption>
    <auro-menuoption value="afghanistan">Afghanistan has a country code of (+93)</auro-menuoption>
    <auro-menuoption value="albania">Albania has a country code of (+355)</auro-menuoption>
  </auro-menu>
</auro-select>
<style>
  #flexMenuWidthExample::part(dropdownTrigger) {
    width: 25%;
  }
</style>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Slot Examples

#### label <a name="label"></a>
Use the `label` slot to give your users contextual information about their selection options. This `label` content is also helpful for assistive devices.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/label.html) -->
  <!-- The below content is automatically added from ./../apiExamples/label.html -->
  <auro-select>
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Please select a preference</span>
    <auro-menu>
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/label.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/label.html -->

```html
<auro-select>
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Please select a preference</span>
  <auro-menu>
    <auro-menuoption value="stops">Stops</auro-menuoption>
    <auro-menuoption value="price">Price</auro-menuoption>
    <auro-menuoption value="duration">Duration</auro-menuoption>
    <auro-menuoption value="departure">Departure</auro-menuoption>
    <auro-menuoption value="arrival">Arrival</auro-menuoption>
    <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
  </auro-menu>
</auro-select>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### helpText <a name="helpText"></a>
Use the `helpText` slot to provide additional information back to your user about their selection option(s).

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/helpText.html) -->
  <!-- The below content is automatically added from ./../apiExamples/helpText.html -->
  <auro-select placeholder="Placeholder Text">
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Label</span>
    <span slot="helpText">Custom help text message.</span>
    <auro-menu>
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/helpText.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/helpText.html -->

```html
<auro-select placeholder="Placeholder Text">
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Label</span>
  <span slot="helpText">Custom help text message.</span>
  <auro-menu>
    <auro-menuoption value="stops">Stops</auro-menuoption>
    <auro-menuoption value="price">Price</auro-menuoption>
    <auro-menuoption value="duration">Duration</auro-menuoption>
    <auro-menuoption value="departure">Departure</auro-menuoption>
    <auro-menuoption value="arrival">Arrival</auro-menuoption>
    <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
  </auro-menu>
</auro-select>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

## Functional Examples

### Reset State

Use the `reset()` method to reset the `<auro-select>`'s `value` and `validity` state. Doing so will preserve all other attributes and properties.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/resetState.html) -->
  <!-- The below content is automatically added from ./../apiExamples/resetState.html -->
  <auro-button id="resetStateBtn">Reset</auro-button>
  <br/><br/>
  <auro-select id="resetStateExample" value="price" placeholder="Placeholder Text">
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Label</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/resetState.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/resetState.html -->

```html
<auro-button id="resetStateBtn">Reset</auro-button>
<br/><br/>
<auro-select id="resetStateExample" value="price" placeholder="Placeholder Text">
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Label</span>
  <span slot="label">Name</span>
  <auro-menu>
    <auro-menuoption value="stops">Stops</auro-menuoption>
    <auro-menuoption value="price">Price</auro-menuoption>
    <auro-menuoption value="duration">Duration</auro-menuoption>
    <auro-menuoption value="departure">Departure</auro-menuoption>
    <auro-menuoption value="arrival">Arrival</auro-menuoption>
    <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
  </auro-menu>
</auro-select>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/resetState.js) -->
<!-- The below code snippet is automatically added from ./../apiExamples/resetState.js -->

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

### Extract value

The following example illustrates how a user may query the `element.value` or `element.optionSelected` for the current value or complete option object that is selected.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/valueExtraction.html) -->
  <!-- The below content is automatically added from ./../apiExamples/valueExtraction.html -->
  <auro-select id="valueExtraction" placeholder="Placeholder Text">
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Label</span>
    <auro-menu>
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
  <auro-button id="valueExtractionBtn">Get current value</auro-button>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/valueExtraction.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/valueExtraction.html -->

```html
<auro-select id="valueExtraction" placeholder="Placeholder Text">
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Label</span>
  <auro-menu>
    <auro-menuoption value="stops">Stops</auro-menuoption>
    <auro-menuoption value="price">Price</auro-menuoption>
    <auro-menuoption value="duration">Duration</auro-menuoption>
    <auro-menuoption value="departure">Departure</auro-menuoption>
    <auro-menuoption value="arrival">Arrival</auro-menuoption>
    <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
  </auro-menu>
</auro-select>
<auro-button id="valueExtractionBtn">Get current value</auro-button>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/valueExtraction.js) -->
<!-- The below code snippet is automatically added from ./../apiExamples/valueExtraction.js -->

```js
export function valueExtractionExample() {
  const valueExtractionExample = document.querySelector('#valueExtraction');
  const valueExtractionBtn = document.querySelector('#valueExtractionBtn');

  valueExtractionBtn.addEventListener('click', () => {
    console.warn('Value selected:', valueExtractionExample.value);
    console.warn('Option selected:', valueExtractionExample.optionSelected);

    alert(`Value selected: ${valueExtractionExample.value}`);
  })
}
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Custom Validity with Error State

This example programmatically adds the `error` state when a user selects an option that is greater than `2`.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/customErrorValidity.html) -->
  <!-- The below content is automatically added from ./../apiExamples/customErrorValidity.html -->
  <auro-select id="primaryError" placeholder="Placeholder Text">
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Label</span>
    <auro-menu>
      <auro-menuoption value="1">1</auro-menuoption>
      <auro-menuoption value="2">2</auro-menuoption>
      <auro-menuoption value="3">3</auro-menuoption>
      <auro-menuoption value="4">4</auro-menuoption>
      <auro-menuoption value="5">5</auro-menuoption>
      <auro-menuoption value="6">6</auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/customErrorValidity.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/customErrorValidity.html -->

```html
<auro-select id="primaryError" placeholder="Placeholder Text">
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Label</span>
  <auro-menu>
    <auro-menuoption value="1">1</auro-menuoption>
    <auro-menuoption value="2">2</auro-menuoption>
    <auro-menuoption value="3">3</auro-menuoption>
    <auro-menuoption value="4">4</auro-menuoption>
    <auro-menuoption value="5">5</auro-menuoption>
    <auro-menuoption value="6">6</auro-menuoption>
  </auro-menu>
</auro-select>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/customErrorValidity.js) -->
<!-- The below code snippet is automatically added from ./../apiExamples/customErrorValidity.js -->

```js
export function customErrorValidityExample(elem) {
  const customErrorValidityExample = document.querySelector('#primaryError');

  customErrorValidityExample.addEventListener('auroSelect-valueSet', () => {
    if (+customErrorValidityExample.value > 2) {
      customErrorValidityExample.setAttribute('error', 'Quantity Exceeded');
    } else if (customErrorValidityExample.hasAttribute('error')) {
      customErrorValidityExample.removeAttribute('error');
    }
  })
};
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Loading<a name="loading"></a>
While content is loading, the menu can either remain empty or display a loading placeholder

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/loading.html) -->
  <!-- The below content is automatically added from ./../apiExamples/loading.html -->
  <auro-select id="loadingExample">
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Please select a preference</span>
    <auro-menu id="loadingExampleSelectMenu">
      <auro-loader slot="loadingIcon" orbit xs></auro-loader><span slot="loadingText">Loading...</span>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/loading.js) -->
<!-- The below code snippet is automatically added from ./../apiExamples/loading.js -->

```js
export function auroMenuLoadingExample() {
  const select = document.querySelector("#loadingExample");
  const menu = document.querySelector("#loadingExampleSelectMenu");

  const emptyMenu = () => {
    const menuoptions = menu.querySelectorAll('auro-menuoption');
    menuoptions.forEach(mo => menu.removeChild(mo));
  }

  const fillMenu = () => {
      menu.innerHTML += `
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>`;
  }

  select.addEventListener("click", () => {
    if (!menu.hasAttribute('loading') && !select.value) {
      emptyMenu();
      menu.setAttribute('loading', 'loading');
      setTimeout(() => {
        menu.removeAttribute('loading');
        fillMenu();
      }, 1000);
    }
  });
}
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/loading.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/loading.html -->

```html
<auro-select id="loadingExample">
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Please select a preference</span>
  <auro-menu id="loadingExampleSelectMenu">
    <auro-loader slot="loadingIcon" orbit xs></auro-loader><span slot="loadingText">Loading...</span>
  </auro-menu>
</auro-select>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### displayValue <a name="displayValue"></a>
The label for selected option can be customized using `displayValue` slot under `<menuoption>.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/displayValue.html) -->
  <!-- The below content is automatically added from ./../apiExamples/displayValue.html -->
  <auro-select id="displayValueExample" autocomplete="address-level1">
    <span slot="bib.fullscreen.headline">Select Your Gender</span>
    <span slot="label">Gender</span>
    <span slot="displayValue"></span>
      <auro-menu>
        <auro-menuoption value="m" data-display="Male">M - Male
          <span slot="displayValue">Male</span>
        </auro-menuoption>
        <auro-menuoption value="f" data-display="Female">F - Female
          <span slot="displayValue">Female</span>
        </auro-menuoption>
        <auro-menuoption value="x" data-display="Unspecified">X - Unspecified
          <span slot="displayValue">Unspecified</span>
        </auro-menuoption>
        <auro-menuoption value="u" data-display="Undisclosed">U - Undisclosed
          <span slot="displayValue">Undisclosed</span>
        </auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/displayValue.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/displayValue.html -->

```html
<auro-select id="displayValueExample" autocomplete="address-level1">
  <span slot="bib.fullscreen.headline">Select Your Gender</span>
  <span slot="label">Gender</span>
  <span slot="displayValue"></span>
    <auro-menu>
      <auro-menuoption value="m" data-display="Male">M - Male
        <span slot="displayValue">Male</span>
      </auro-menuoption>
      <auro-menuoption value="f" data-display="Female">F - Female
        <span slot="displayValue">Female</span>
      </auro-menuoption>
      <auro-menuoption value="x" data-display="Unspecified">X - Unspecified
        <span slot="displayValue">Unspecified</span>
      </auro-menuoption>
      <auro-menuoption value="u" data-display="Undisclosed">U - Undisclosed
        <span slot="displayValue">Undisclosed</span>
      </auro-menuoption>
  </auro-menu>
</auro-select>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Customized bib position
The bib position can be customized with `placement`, `offset`, `flip`, `autoPlacement`, and `shift` attributes.

- `placement` specifies the preferred position where the bib should appear relative to the trigger.
- `offset` sets the distance between the trigger and the bib.
- When `autoPlacement` is enabled, smart positioning logic is applied to determine the best placement for the bib. If all sides have sufficient space, the bib will appear in the position specified by `placement`.
- Unless `noFlip` is enabled, if there isn't enough space for the preferred `placement`, the bib will automatically flip to an alternative position.
- `shift` when enabled, adjusts the bib position when it would overflow the viewport boundaries, ensuring it remains visible.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/floaterConfig.html) -->
  <!-- The below content is automatically added from ./../apiExamples/floaterConfig.html -->
  <div style="width: 350px">
    <auro-select offset="20" noFlip placement="bottom-end">
      <span slot="bib.fullscreen.headline">Bib Headline</span>
      <span slot="label">Label</span>
      <span slot="helpText">bottom-end bib with 20px offset and noFlip</span>
      <auro-menu>
        <auro-menuoption value="stops">Stops</auro-menuoption>
        <auro-menuoption value="price">Price</auro-menuoption>
        <auro-menuoption value="duration">Duration</auro-menuoption>
        <auro-menuoption value="departure">Departure</auro-menuoption>
        <auro-menuoption value="arrival">Arrival</auro-menuoption>
        <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
      </auro-menu>
    </auro-select>
    <auro-select offset="20" placement="bottom-end">
      <span slot="bib.fullscreen.headline">Bib Headline</span>
      <span slot="label">Label</span>
      <span slot="helpText">bottom-end bib with 20px offset and flip</span>
      <auro-menu>
        <auro-menuoption value="stops">Stops</auro-menuoption>
        <auro-menuoption value="price">Price</auro-menuoption>
        <auro-menuoption value="duration">Duration</auro-menuoption>
        <auro-menuoption value="departure">Departure</auro-menuoption>
        <auro-menuoption value="arrival">Arrival</auro-menuoption>
        <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
      </auro-menu>
    </auro-select>
    <auro-select offset="20" noFlip placement="right" autoPlacement noFlip >
      <span slot="bib.fullscreen.headline">Bib Headline</span>
      <span slot="label">Label</span>
      <span slot="helpText">right bib with 20px offset, noFlip and autoPlacement</span>
      <auro-menu>
        <auro-menuoption value="stops">Stops</auro-menuoption>
        <auro-menuoption value="price">Price</auro-menuoption>
        <auro-menuoption value="duration">Duration</auro-menuoption>
        <auro-menuoption value="departure">Departure</auro-menuoption>
        <auro-menuoption value="arrival">Arrival</auro-menuoption>
        <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
      </auro-menu>
    </auro-select>
    <auro-select width="350px" offset="20" noFlip placement="bottom-start" shift noFlip >
      <span slot="bib.fullscreen.headline">Bib Headline</span>
      <span slot="label">Label</span>
      <span slot="helpText">bottom-start bib with 20px offset, noFlip and shift</span>
      <auro-menu>
        <auro-menuoption value="stops">Stops</auro-menuoption>
        <auro-menuoption value="price">Price</auro-menuoption>
        <auro-menuoption value="duration">Duration</auro-menuoption>
        <auro-menuoption value="departure">Departure</auro-menuoption>
        <auro-menuoption value="arrival">Arrival</auro-menuoption>
        <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
      </auro-menu>
    </auro-select>
  </div>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/floaterConfig.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/floaterConfig.html -->

```html
<div style="width: 350px">
  <auro-select offset="20" noFlip placement="bottom-end">
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Label</span>
    <span slot="helpText">bottom-end bib with 20px offset and noFlip</span>
    <auro-menu>
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
  <auro-select offset="20" placement="bottom-end">
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Label</span>
    <span slot="helpText">bottom-end bib with 20px offset and flip</span>
    <auro-menu>
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
  <auro-select offset="20" noFlip placement="right" autoPlacement noFlip >
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Label</span>
    <span slot="helpText">right bib with 20px offset, noFlip and autoPlacement</span>
    <auro-menu>
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
  <auro-select width="350px" offset="20" noFlip placement="bottom-start" shift noFlip >
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Label</span>
    <span slot="helpText">bottom-start bib with 20px offset, noFlip and shift</span>
    <auro-menu>
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
</div>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Dropdown with fullscreen bib

You can make the dropdown open in fullscreen at a specific breakpoint by setting `fullscreenBreakpoint`.

The default value of `fullscreenBreakpoint` is `sm`. 

Breakpoint token can be found [here](https://auro.alaskaair.com/getting-started/developers/design-tokens)

To support fullcreen bib, setting `bib.fullscreen.headline` is **STRONGLY RECOMMENDED**.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/fullscreenBreakpoint.html) -->
  <!-- The below content is automatically added from ./../apiExamples/fullscreenBreakpoint.html -->
  <auro-select fullscreenBreakpoint="lg">
    <span slot="label">Select Example</span>
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <auro-menu>
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/fullscreenBreakpoint.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/fullscreenBreakpoint.html -->

```html
<auro-select fullscreenBreakpoint="lg">
  <span slot="label">Select Example</span>
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <auro-menu>
    <auro-menuoption value="stops">Stops</auro-menuoption>
    <auro-menuoption value="price">Price</auro-menuoption>
    <auro-menuoption value="duration">Duration</auro-menuoption>
    <auro-menuoption value="departure">Departure</auro-menuoption>
    <auro-menuoption value="arrival">Arrival</auro-menuoption>
    <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
  </auro-menu>
</auro-select>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### in Dialog

The component can be in a dialog.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inDialog.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inDialog.html -->
  <div>
    <auro-button id="select-dialog-opener">Select in Dialog</auro-button>
    <auro-dialog id="select-dialog">
      <span slot="header">Select in Dialog</span>
      <div slot="content">
        <auro-select id="valueExample" value="price">
          <span slot="bib.fullscreen.headline">Bib Headline</span>
          <span slot="label">Name</span>
          <auro-menu>
            <auro-menuoption id="option-0" value="stops">Stops</auro-menuoption>
            <auro-menuoption id="option-1" value="price">Price</auro-menuoption>
            <auro-menuoption id="option-2" value="duration">Duration</auro-menuoption>
            <auro-menuoption id="option-3" value="departure">Departure</auro-menuoption>
            <auro-menuoption id="option-4" value="arrival">Arrival</auro-menuoption>
            <auro-menuoption id="option-5" value="prefer alaska">Prefer Alaska</auro-menuoption>
          </auro-menu>
        </auro-select>
      </div>
    </auro-dialog>
  </div>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/inDialog.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/inDialog.html -->

```html
<div>
  <auro-button id="select-dialog-opener">Select in Dialog</auro-button>
  <auro-dialog id="select-dialog">
    <span slot="header">Select in Dialog</span>
    <div slot="content">
      <auro-select id="valueExample" value="price">
        <span slot="bib.fullscreen.headline">Bib Headline</span>
        <span slot="label">Name</span>
        <auro-menu>
          <auro-menuoption id="option-0" value="stops">Stops</auro-menuoption>
          <auro-menuoption id="option-1" value="price">Price</auro-menuoption>
          <auro-menuoption id="option-2" value="duration">Duration</auro-menuoption>
          <auro-menuoption id="option-3" value="departure">Departure</auro-menuoption>
          <auro-menuoption id="option-4" value="arrival">Arrival</auro-menuoption>
          <auro-menuoption id="option-5" value="prefer alaska">Prefer Alaska</auro-menuoption>
        </auro-menu>
      </auro-select>
    </div>
  </auro-dialog>
</div>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/inDialog.js) -->
<!-- The below code snippet is automatically added from ./../apiExamples/inDialog.js -->

```js
export function inDialogExample() {
  document.querySelector("#select-dialog-opener").addEventListener("click", () => {
    const dialog = document.querySelector("#select-dialog");
    dialog.open = true;
  });
};
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### Watch for value changes

The following example listens for the `auroMenu-selectedOption` event. Once triggered, element.value or element.optionSelected may be queried for the new value or complete option object.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/valueAlert.html) -->
  <!-- The below content is automatically added from ./../apiExamples/valueAlert.html -->
  <auro-select id="valueAlert" placeholder="Placeholder Text">
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Label</span>
    <auro-menu id="valueAlertMenu">
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/valueAlert.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/valueAlert.html -->

```html
<auro-select id="valueAlert" placeholder="Placeholder Text">
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Label</span>
  <auro-menu id="valueAlertMenu">
    <auro-menuoption value="stops">Stops</auro-menuoption>
    <auro-menuoption value="price">Price</auro-menuoption>
    <auro-menuoption value="duration">Duration</auro-menuoption>
    <auro-menuoption value="departure">Departure</auro-menuoption>
    <auro-menuoption value="arrival">Arrival</auro-menuoption>
    <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
  </auro-menu>
</auro-select>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/valueAlert.js) -->
<!-- The below code snippet is automatically added from ./../apiExamples/valueAlert.js -->

```js
export function valueAlertExample() {
  const select = document.querySelector('#valueAlert');
  const menu = document.querySelector('#valueAlertMenu');

  menu.addEventListener('auroMenu-selectedOption', () => {
    console.warn('Select value changed to:', select.value);
    console.warn('Select optionSelected changed to:', select.optionSelected);
  });
}
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>
