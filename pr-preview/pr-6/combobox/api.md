<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../docs/api.md) -->
<!-- The below content is automatically added from ./../docs/api.md -->

# auro-combobox

## Properties

| Property                              | Attribute                             | Modifiers | Type                  | Default                    | Description                                      |
|---------------------------------------|---------------------------------------|-----------|-----------------------|----------------------------|--------------------------------------------------|
| [appearance](#appearance)                          | `appearance`                          |           | `string`              | "'default'"                | Defines whether the component will be on lighter or darker backgrounds. |
| [autoPlacement](#autoPlacement)                       | `autoPlacement`                       |           | `boolean`             | false                      | If declared, bib's position will be automatically calculated where to appear. |
| [autocomplete](#autocomplete)                        | `autocomplete`                        |           | `string`              | "false"                    | An enumerated attribute that defines what the user agent can suggest for autofill. At this time, only `autocomplete="off"` is supported. |
| [behavior](#behavior)                            | `behavior`                            |           | `string`              | "suggestion"               | Sets the behavior of the combobox, "filter" or "suggestion".<br />"filter" requires the user to select an option from the menu.<br />"suggestion" allows the user to enter a value not present in the menu options. |
| [checkmark](#checkmark)                           | `checkmark`                           |           | `boolean`             | false                      | When attribute is present auro-menu will apply check marks to selected options. |
| [disabled](#disabled)                            | `disabled`                            |           | `boolean`             | false                      | If set, disables the combobox.                   |
| [dvInputOnly](#dvInputOnly)                         | `dvInputOnly`                         |           | `boolean`             | false                      | If defined, the display value slot content will only mask the HTML5 input element. The inputs label will not be masked. |
| [error](#error)                               | `error`                               |           | `string`              |                            | When defined, sets persistent validity to `customError` and sets the validation message to the attribute value. |
| [format](#format)                              | `format`                              |           | `string`              |                            | Specifies the input mask format.                 |
| [fullscreenBreakpoint](#fullscreenBreakpoint)                | `fullscreenBreakpoint`                |           | `string`              | "sm"                       | Defines the screen size breakpoint (`xs`, `sm`, `md`, `lg`, `xl`, `disabled`)<br />at which the dropdown switches to fullscreen mode on mobile. `disabled` indicates a dropdown should _never_ enter fullscreen.<br /><br />When expanded, the dropdown will automatically display in fullscreen mode<br />if the screen size is equal to or smaller than the selected breakpoint. |
| [inputValue](#inputValue)                          |                                       | readonly  | `string \| undefined` |                            | Returns the current value of the input element within the combobox. |
| [inputmode](#inputmode)                           | `inputmode`                           |           | `string`              |                            | Exposes inputmode attribute for input.           |
| [largeFullscreenHeadline](#largeFullscreenHeadline)             | `largeFullscreenHeadline`             |           | `boolean`             |                            | If declared, make bib.fullscreen.headline in HeadingDisplay.<br />Otherwise, Heading 600 |
| [layout](#layout)                              |                                       |           | `string`              | "classic"                  |                                                  |
| [matchWidth](#matchWidth)                          | `matchWidth`                          |           | `boolean`             | true                       | If declared, the popover and trigger will be set to the same width. |
| [msgSelectionMissing](#msgSelectionMissing)                 |                                       |           | `string`              | "Please select an option." |                                                  |
| [noFilter](#noFilter)                            | `noFilter`                            |           | `boolean`             | false                      | If set, combobox will not filter menuoptions based on input. |
| [noFlip](#noFlip)                              | `noFlip`                              |           | `boolean`             | "false"                    | If declared, the bib will NOT flip to an alternate position<br />when there isn't enough space in the specified `placement`. |
| [noValidate](#noValidate)                          | `noValidate`                          |           | `boolean`             | false                      | If set, disables auto-validation on blur.        |
| [offset](#offset)                              | `offset`                              |           | `number`              | "0"                        | Gap between the trigger element and bib.         |
| [onDark](#onDark)                              | `onDark`                              |           | `boolean`             |                            | DEPRECATED - use `appearance` instead.           |
| [optionSelected](#optionSelected)                      | `optionSelected`                      |           | `HTMLElement`         |                            | Specifies the current selected option.           |
| [persistInput](#persistInput)                        | `persistInput`                        |           | `Boolean`             | false                      | If declared, selecting a menu option will not change the input value. By doing so,<br />the current menu filter will be preserved and the user can continue from their last<br />filter state. It is recommended to use this in combination with the `displayValue` slot. |
| [placeholder](#placeholder)                         | `placeholder`                         |           | `string`              |                            | Define custom placeholder text, only supported by date input formats. |
| [placement](#placement)                           | `placement`                           |           | `string`              | "bottom-start"             | Position where the bib should appear relative to the trigger.<br />Accepted values:<br />"top" \| "right" \| "bottom" \| "left" \|<br />"bottom-start" \| "top-start" \| "top-end" \|<br />"right-start" \| "right-end" \| "bottom-end" \|<br />"left-start" \| "left-end" |
| [required](#required)                            | `required`                            |           | `boolean`             | false                      | Populates the `required` attribute on the input. Used for client-side validation. |
| [setCustomValidity](#setCustomValidity)                   | `setCustomValidity`                   |           | `string`              |                            | Sets a custom help text message to display for all validityStates. |
| [setCustomValidityCustomError](#setCustomValidityCustomError)        | `setCustomValidityCustomError`        |           | `string`              |                            | Custom help text message to display when validity = `customError`. |
| [setCustomValidityValueMissing](#setCustomValidityValueMissing)       | `setCustomValidityValueMissing`       |           | `string`              |                            | Custom help text message to display when validity = `valueMissing`. |
| [setCustomValidityValueMissingFilter](#setCustomValidityValueMissingFilter) | `setCustomValidityValueMissingFilter` |           | `string`              |                            | Custom help text message to display when validity = `valueMissing` due to the user not choosing a menu option when behavior = "filter". |
| [shape](#shape)                               |                                       |           | `string`              | "classic"                  |                                                  |
| [shift](#shift)                               | `shift`                               |           | `boolean`             | "false"                    | If declared, the dropdown will shift its position to avoid being cut off by the viewport. |
| [size](#size)                                |                                       |           | `string`              | "xl"                       |                                                  |
| [triggerIcon](#triggerIcon)                         | `triggerIcon`                         |           | `boolean`             | false                      | If set, the `icon` attribute will be applied to the trigger `auro-input` element. |
| [type](#type)                                | `type`                                |           | `string`              |                            | Applies the defined value as the type attribute on auro-input. |
| [typedValue](#typedValue)                          | `typedValue`                          |           | `string`              | "undefined"                | Specifies the value of the input element within the combobox. |
| [validity](#validity)                            | `validity`                            |           | `string`              |                            | Specifies the `validityState` this element is in. |
| [value](#value)                               | `value`                               |           | `string`              | "undefined"                | Value selected for the dropdown menu.            |

## Methods

| Method               | Type                                   | Description                                      |
|----------------------|----------------------------------------|--------------------------------------------------|
| [clear](#clear)              | `(): void`                             | Clears the current value of the combobox.        |
| [focus](#focus)              | `(): void`                             | Focuses the combobox trigger input.              |
| [hideBib](#hideBib)            | `(): void`                             | Hides the dropdown bib if its open.              |
| [isValid](#isValid)            | `(): boolean`                          | Checks if the element is valid.                  |
| [reset](#reset)              | `(): void`                             | Resets component to initial state.               |
| [setMenuValue](#setMenuValue)       | `(value: string): void`                | Sets the menu value if menu is available.<br /><br />**value**: The value to set on the menu. |
| [showBib](#showBib)            | `(): void`                             | Shows the dropdown bib if there are options to show. |
| [updateActiveOption](#updateActiveOption) | `(index: number): void`                | Updates the active option in the menu.<br /><br />**index**: Index of the option to make active. |
| [validate](#validate)           | `(force?: boolean \| undefined): void` | Validates value.<br /><br />**force**: Whether to force validation. |

## Events

| Event                       | Type                                             | Description                                      |
|-----------------------------|--------------------------------------------------|--------------------------------------------------|
| `auroCombobox-valueSet`     | `CustomEvent<any>`                               | (Deprecated) Notifies that the component has a new value set. |
| `auroFormElement-validated` |                                                  | Notifies that the component value(s) have been validated. |
| [input](#input)                     | `CustomEvent<{ optionSelected: any; value: any; }>` | Notifies that the component has a new value set. |
| [inputValue](#inputValue)                | `CustomEvent<{ value: string \| undefined; }>`   | Notifies that the components internal HTML5 input value has changed. |

## Slots

| Name                      | Description                                      |
|---------------------------|--------------------------------------------------|
|                           | Default slot for the menu content.               |
| `ariaLabel.bib.close`     | Sets aria-label on close button in fullscreen bib |
| `ariaLabel.input.clear`   | Sets aria-label on clear button                  |
| `bib.fullscreen.headline` | Defines the headline to display above menu-options |
| [displayValue](#displayValue)            | Allows custom HTML content to display the selected value when the combobox is not focused. Only works with `snowflake` and `emphasized` layouts. |
| [helpText](#helpText)                | Defines the content of the helpText.             |
| [label](#label)                   | Defines the content of the label.                |
| [optionalLabel](#optionalLabel)           | Allows overriding the optional display text "(optional)", which appears next to the label. |
<!-- AURO-GENERATED-CONTENT:END -->

## API Examples

### Basic

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/basic.html) -->
  <!-- The below content is automatically added from ./../apiExamples/basic.html -->
  <auro-combobox>
    <span slot="ariaLabel.bib.close">Close combobox</span>
    <span slot="ariaLabel.input.clear">Clear All</span>
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearance.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearance.html -->
  <auro-combobox appearance="inverse">
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/basic.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/basic.html -->

```html
<auro-combobox>
  <span slot="ariaLabel.bib.close">Close combobox</span>
  <span slot="ariaLabel.input.clear">Clear All</span>
  <span slot="bib.fullscreen.headline">Bib Header</span>
  <span slot="label">Name</span>
  <auro-menu>
    <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
    <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
    <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
    <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
    <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
    <auro-menuoption static nomatch>No matching option</auro-menuoption>
  </auro-menu>
</auro-combobox>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearance.html) -->
<!-- The below content is automatically added from ./../apiExamples/inverseAppearance.html -->
<auro-combobox appearance="inverse">
  <span slot="bib.fullscreen.headline">Bib Header</span>
  <span slot="label">Name</span>
  <auro-menu>
    <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
    <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
    <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
    <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
    <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
    <auro-menuoption static nomatch>No matching option</auro-menuoption>
  </auro-menu>
</auro-combobox>
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Behavior

There are two behaviors available for the combo box: suggestion and filter.
The default behavior is "suggestion".

#### Suggestion

With the suggestion behavior, the menu options are displayed to the user as suggestions, but the user may enter whatever value they like into the input

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/suggestion.html) -->
  <!-- The below content is automatically added from ./../apiExamples/suggestion.html -->
  <auro-combobox behavior="suggestion">
    <span slot="ariaLabel.bib.close">Close combobox</span>
    <span slot="ariaLabel.input.clear">Clear All</span>
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/suggestion.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/suggestion.html -->

```html
<auro-combobox behavior="suggestion">
  <span slot="ariaLabel.bib.close">Close combobox</span>
  <span slot="ariaLabel.input.clear">Clear All</span>
  <span slot="bib.fullscreen.headline">Bib Header</span>
  <span slot="label">Name</span>
  <auro-menu>
    <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
    <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
    <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
    <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
    <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
    <auro-menuoption static nomatch>No matching option</auro-menuoption>
  </auro-menu>
</auro-combobox>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### Filter

With the filter behavior, the menu options are displayed to the user, and the user is required to choose one of the menu options in order for the input to be considered valid.

The `setCustomValidityValueMissingFilter` attribute is also available to display a custom message to the user when this validation check fails.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/filter.html) -->
  <!-- The below content is automatically added from ./../apiExamples/filter.html -->
  <auro-combobox behavior="filter" setCustomValidityValueMissingFilter="Please select an option from the list">
    <span slot="ariaLabel.bib.close">Close combobox</span>
    <span slot="ariaLabel.input.clear">Clear All</span>
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/filter.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/filter.html -->

```html
<auro-combobox behavior="filter" setCustomValidityValueMissingFilter="Please select an option from the list">
  <span slot="ariaLabel.bib.close">Close combobox</span>
  <span slot="ariaLabel.input.clear">Clear All</span>
  <span slot="bib.fullscreen.headline">Bib Header</span>
  <span slot="label">Name</span>
  <auro-menu>
    <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
    <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
    <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
    <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
    <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
    <auro-menuoption static nomatch>No matching option</auro-menuoption>
  </auro-menu>
</auro-combobox>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Dynamic Menu

This example demonstrates a data driven combobox. The data is used to populate the `auro-menu`. In this example, each time the input's value changes, the data is updated and the menu is recreated.

The menu in this example was populated from data from a country/city API. To keep the data set small, the data in the menu is based off an API call that returns all countries and cities that contain the substring "**germ**" (non case-sensitive) in their name.

<div class="exampleWrapper--ondark">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/dynamicMenu.html) -->
  <!-- The below content is automatically added from ./../apiExamples/dynamicMenu.html -->
  <!-- HTML example file -->
  <!-- ----------------- -->
  <auro-combobox
    id="dynamicMenuExample"
    value="TAN"
    layout="snowflake"
    shape="snowflake"
    size="lg"
    appearance="inverse"
    noFilter
    persistInput
    dvInputOnly
    setCustomValidityValueMissing="Please select an option from the list."
    required>
    <span slot="bib.fullscreen.headline">Dynamic Combobox Header</span>
    <span slot="label">First</span>
    <!--
      The auro-combobox element requires an empty auro-menu element
      due to the requirements of auro-dropdown and auro-input
    -->
    <auro-menu id="initMenu"></auro-menu>
  </auro-combobox>
  <br>
  <auro-combobox
    id="dynamicMenuExampleTwo"
    value="GER"
    layout="snowflake"
    shape="snowflake"
    size="lg"
    appearance="inverse"
    noFilter
    persistInput
    dvInputOnly
    setCustomValidityValueMissing="Please select an option from the list."
    required>
    <span slot="bib.fullscreen.headline">Dynamic Combobox Header</span>
    <span slot="label">Second</span>
    <!--
      The auro-combobox element requires an empty auro-menu element
      due to the requirements of auro-dropdown and auro-input
    -->
    <auro-menu id="initMenuTwo"></auro-menu>
  </auro-combobox>
  <br>
  <auro-button id="dynamicMenuSwapButton">
    Swap Values
  </auro-button>
  <auro-button id="dynamicMenuPersistButton">
    Toggle Persist Input
  </auro-button>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/dynamicMenu.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/dynamicMenu.html -->

```html
<!-- HTML example file -->
<!-- ----------------- -->
<auro-combobox
  id="dynamicMenuExample"
  value="TAN"
  layout="snowflake"
  shape="snowflake"
  size="lg"
  appearance="inverse"
  noFilter
  persistInput
  dvInputOnly
  setCustomValidityValueMissing="Please select an option from the list."
  required>
  <span slot="bib.fullscreen.headline">Dynamic Combobox Header</span>
  <span slot="label">First</span>
  <!--
    The auro-combobox element requires an empty auro-menu element
    due to the requirements of auro-dropdown and auro-input
  -->
  <auro-menu id="initMenu"></auro-menu>
</auro-combobox>
<br>
<auro-combobox
  id="dynamicMenuExampleTwo"
  value="GER"
  layout="snowflake"
  shape="snowflake"
  size="lg"
  appearance="inverse"
  noFilter
  persistInput
  dvInputOnly
  setCustomValidityValueMissing="Please select an option from the list."
  required>
  <span slot="bib.fullscreen.headline">Dynamic Combobox Header</span>
  <span slot="label">Second</span>
  <!--
    The auro-combobox element requires an empty auro-menu element
    due to the requirements of auro-dropdown and auro-input
  -->
  <auro-menu id="initMenuTwo"></auro-menu>
</auro-combobox>
<br>
<auro-button id="dynamicMenuSwapButton">
  Swap Values
</auro-button>
<auro-button id="dynamicMenuPersistButton">
  Toggle Persist Input
</auro-button>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/dynamicMenu.js) -->
<!-- The below code snippet is automatically added from ./../apiExamples/dynamicMenu.js -->

```js
// Javascript example file
// -----------------------
import { DynamicData } from './dynamicMenuDataApi';

export async function dynamicMenuExample() {
  // Resets the root menu
  function resetMenu(root) {
    while (root.firstChild) {
      root.removeChild(root.firstChild);
    }
  }

  function swapValues() {
    const elOne = document.querySelector('#dynamicMenuExample');
    const elTwo = document.querySelector('#dynamicMenuExampleTwo');

    const elOneValue = elOne.value;
    const elTwoValue = elTwo.value;

    const elOneInputValue = elOne.input.value;
    const elTwoInputValue = elTwo.input.value;

    elOne.reset();
    elTwo.reset();

    elOne.value = elTwoValue;
    elTwo.value = elOneValue;

    setTimeout(() => {
      elOne.typedValue = elTwoInputValue;
      elTwo.typedValue = elOneInputValue;
    }, 0);
  }

  document.querySelector('#dynamicMenuSwapButton').addEventListener('click', () => {
    swapValues();
  });

  document.querySelector('#dynamicMenuPersistButton').addEventListener('click', () => {
    const elOne = document.querySelector('#dynamicMenuExample');
    const elTwo = document.querySelector('#dynamicMenuExampleTwo');

    elOne.persistInput = !elOne.persistInput;
    elTwo.persistInput = !elTwo.persistInput;
  });

  // Generates HTML for menu and submenus using country & city data from an external API
  function generateHtml(data, selector) {
    const initialMenu = document.querySelector(selector);

    resetMenu(initialMenu);

    for (let index = 0; index < data.length; index++) {
      const country = data[index]['country'];
      const cities = data[index]['cities'];

      generateMenuOptionHtml(initialMenu, country, country.substring(0, 3).toUpperCase());

      for (let indexB = 0; indexB < cities.length; indexB++) {
        const subMenu = document.createElement('auro-menu');

        generateMenuOptionHtml(subMenu, cities[indexB], cities[indexB].substring(0, 3).toUpperCase());

        initialMenu.appendChild(subMenu);
      }
    };
  }

  // Helper function that generates HTML for menuoptions
  function generateMenuOptionHtml(menu, label, value) {
    const option = document.createElement('auro-menuoption');
    const displayValue = document.createElement('div');
    displayValue.setAttribute("slot", "displayValue");
    displayValue.innerHTML = value;

    option.value = value;
    option.innerHTML = label;
    menu.appendChild(option);
    option.appendChild(displayValue);
  }

  // Main javascript that runs all JS to create example
  const dynamicData = new DynamicData();
  const dynamicMenuExampleEl = document.querySelector('#dynamicMenuExample');
  const dropdownEl = dynamicMenuExampleEl.shadowRoot.querySelector(dynamicMenuExampleEl.dropdownTag._$litStatic$);
  const inputEl = dropdownEl.querySelector(dynamicMenuExampleEl.inputTag._$litStatic$);

  inputEl.addEventListener('input', () => {
    let data = dynamicData.getData();
    data = dynamicData.filterData(data, inputEl.value);

    generateHtml(data, '#initMenu');
  });

  if (dynamicMenuExampleEl.value && dynamicMenuExampleEl.value.length > 0 && dynamicMenuExampleEl.input.value && (!dynamicMenuExampleEl.menu.availableOptions || dynamicMenuExampleEl.menu.availableOptions.length === 0)) {
    let data = dynamicData.getData();
    data = dynamicData.filterData(data, inputEl.value);
    generateHtml(data, '#initMenu');
  }

  // TODO: Need to refactor this to to not console a console error
  const dynamicDataTwo = new DynamicData();
  const dynamicMenuExampleElTwo = document.querySelector('#dynamicMenuExampleTwo');
  const dropdownElTwo = dynamicMenuExampleElTwo.shadowRoot.querySelector(dynamicMenuExampleElTwo.dropdownTag._$litStatic$);
  const inputElTwo = dropdownElTwo.querySelector(dynamicMenuExampleElTwo.inputTag._$litStatic$);

  inputElTwo.addEventListener('input', () => {
    let data = dynamicDataTwo.getData();
    data = dynamicDataTwo.filterData(data, inputElTwo.value);

    generateHtml(data, '#initMenuTwo');
  });

  if (dynamicMenuExampleElTwo.value && dynamicMenuExampleElTwo.value.length > 0 && dynamicMenuExampleElTwo.input.value && (!dynamicMenuExampleElTwo.menu.availableOptions || dynamicMenuExampleElTwo.menu.availableOptions.length === 0)) {
    let data = dynamicDataTwo.getData();
    data = dynamicDataTwo.filterData(data, inputElTwo.value);
    generateHtml(data, '#initMenuTwo');
  }
}
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Persistent Input

The `persistInput` attribute allows you to set the combo box to persist the value of the input regardless of the current value set for the combo box.

A persistent input is typically used in conjunction with display values to show the actual value of the selected option to the user when the input is not focused.

This is helpful for things like dynamic menus where you want the user to be able to continue their search where they left off but display a full selected value when the input is not focused.

_*Note:*_ When using `persistInput` with the `required` attribute, you must also pass an error message for when there isn't a valid value but the user has typed something in the input to the `setCustomValidityValueMissing` attribute.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/persistInput.html) -->
  <!-- The below content is automatically added from ./../apiExamples/persistInput.html -->
  <auro-combobox
    required
    persistInput
    setCustomValidityValueMissing="Please select an option from the list."
    >
    <span slot="bib.fullscreen.headline">Persistant Input</span>
    <span slot="label">Persistant Input</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">
        Apples
        <div slot="displayValue">Apples</div>
      </auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">
        Oranges
        <div slot="displayValue">Oranges</div>
      </auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">
        Peaches
        <div slot="displayValue">Peaches</div>
      </auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">
        Grapes
        <div slot="displayValue">Grapes</div>
      </auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">
        Cherries
        <div slot="displayValue">Cherries</div>
      </auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/persistInput.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/persistInput.html -->

```html
<auro-combobox
  required
  persistInput
  setCustomValidityValueMissing="Please select an option from the list."
  >
  <span slot="bib.fullscreen.headline">Persistant Input</span>
  <span slot="label">Persistant Input</span>
  <auro-menu>
    <auro-menuoption value="Apples" id="option-0">
      Apples
      <div slot="displayValue">Apples</div>
    </auro-menuoption>
    <auro-menuoption value="Oranges" id="option-1">
      Oranges
      <div slot="displayValue">Oranges</div>
    </auro-menuoption>
    <auro-menuoption value="Peaches" id="option-2">
      Peaches
      <div slot="displayValue">Peaches</div>
    </auro-menuoption>
    <auro-menuoption value="Grapes" id="option-3">
      Grapes
      <div slot="displayValue">Grapes</div>
    </auro-menuoption>
    <auro-menuoption value="Cherries" id="option-4">
      Cherries
      <div slot="displayValue">Cherries</div>
    </auro-menuoption>
  </auro-menu>
</auro-combobox>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Updating Externally

This example demonstrates using the <code>updateActiveOption</code> method to set a specific menu option as "active."

This is useful for situations like matching IATA codes (sea -> SeaTac airport) 

<div class="exampleWrapper--ondark">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/externalSelection.html) -->
  <!-- The below content is automatically added from ./../apiExamples/externalSelection.html -->
  <p style="color: white;">
      Type 'a' in the combobox for best testing results :)
  </p>
  <auro-combobox appearance="inverse" id="externalSelectionExample" layout="classic" shape="classic" size="lg" placeholder="Placeholder content" required style="width: 249px;">
    <span slot="ariaLabel.bib.close">Close combobox</span>
    <span slot="ariaLabel.input.clear">Clear All</span>
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
    <span slot="helpText">
      Help text - Lorem ipsum solar lorem ipsum solar
    </span>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/externalSelection.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/externalSelection.html -->

```html
<p style="color: white;">
    Type 'a' in the combobox for best testing results :)
</p>
<auro-combobox appearance="inverse" id="externalSelectionExample" layout="classic" shape="classic" size="lg" placeholder="Placeholder content" required style="width: 249px;">
  <span slot="ariaLabel.bib.close">Close combobox</span>
  <span slot="ariaLabel.input.clear">Clear All</span>
  <span slot="bib.fullscreen.headline">Bib Header</span>
  <span slot="label">Name</span>
  <auro-menu>
    <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
    <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
    <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
    <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
    <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
    <auro-menuoption static nomatch>No matching option</auro-menuoption>
  </auro-menu>
  <span slot="helpText">
    Help text - Lorem ipsum solar lorem ipsum solar
  </span>
</auro-combobox>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/externalSelection.js) -->
<!-- The below code snippet is automatically added from ./../apiExamples/externalSelection.js -->

```js
import { AuroCombobox } from "../src/auro-combobox";

/**
 * Demonstrates how to make external selection in the combobox.
 */
export function setupExternalSelectionExample() {

  /** @type {AuroCombobox} */
  const combobox = document.getElementById('externalSelectionExample');

  combobox.addEventListener('input', () => {
    // Perform whatever matching logic you need here

    // This comes from your custom code, for example matching SEA to SeaTac IATA code.
    // This matches "peaches" as configured.
    const matchingMenuOption = 2;
    combobox.updateActiveOption(matchingMenuOption);
  });
}
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Property Examples

#### disabled

If set, disables the combobox.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/disabled.html) -->
  <!-- The below content is automatically added from ./../apiExamples/disabled.html -->
  <auro-combobox disabled>
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption value="Prefer Alaska" id="option-5">Prefer Alaska</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceDisabled.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearanceDisabled.html -->
  <auro-combobox appearance="inverse" disabled>
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption value="Prefer Alaska" id="option-5">Prefer Alaska</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/disabled.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/disabled.html -->

```html
<auro-combobox disabled>
  <span slot="bib.fullscreen.headline">Bib Header</span>
  <span slot="label">Name</span>
  <auro-menu>
    <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
    <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
    <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
    <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
    <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
    <auro-menuoption value="Prefer Alaska" id="option-5">Prefer Alaska</auro-menuoption>
    <auro-menuoption static nomatch>No matching option</auro-menuoption>
  </auro-menu>
</auro-combobox>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceDisabled.html) -->
<!-- The below content is automatically added from ./../apiExamples/inverseAppearanceDisabled.html -->
<auro-combobox appearance="inverse" disabled>
  <span slot="bib.fullscreen.headline">Bib Header</span>
  <span slot="label">Name</span>
  <auro-menu>
    <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
    <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
    <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
    <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
    <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
    <auro-menuoption value="Prefer Alaska" id="option-5">Prefer Alaska</auro-menuoption>
    <auro-menuoption static nomatch>No matching option</auro-menuoption>
  </auro-menu>
</auro-combobox>
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### Input Mode

You can manually set the input mode for the input.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inputmode.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inputmode.html -->
  <auro-combobox inputmode="numeric">
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="1" id="option-0">1</auro-menuoption>
      <auro-menuoption value="2" id="option-1">2</auro-menuoption>
      <auro-menuoption value="3" id="option-2">3</auro-menuoption>
      <auro-menuoption value="4" id="option-3">4</auro-menuoption>
      <auro-menuoption value="5" id="option-4">5</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/inputmode.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/inputmode.html -->

```html
<auro-combobox inputmode="numeric">
  <span slot="bib.fullscreen.headline">Bib Header</span>
  <span slot="label">Name</span>
  <auro-menu>
    <auro-menuoption value="1" id="option-0">1</auro-menuoption>
    <auro-menuoption value="2" id="option-1">2</auro-menuoption>
    <auro-menuoption value="3" id="option-2">3</auro-menuoption>
    <auro-menuoption value="4" id="option-3">4</auro-menuoption>
    <auro-menuoption value="5" id="option-4">5</auro-menuoption>
    <auro-menuoption static nomatch>No matching option</auro-menuoption>
  </auro-menu>
</auro-combobox>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### noFilter

If set, combobox will not do suggestion filtering of the menuoptions. This option is useful when the `<auro-menuoption>` elements are being pre-filtered externally to combobox (e.g. using the citysearch API).

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/noFilter.html) -->
  <!-- The below content is automatically added from ./../apiExamples/noFilter.html -->
  <auro-combobox noFilter>
    <span slot="bib.fullscreen.headline">noFilter Combobox Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/noFilter.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/noFilter.html -->

```html
<auro-combobox noFilter>
  <span slot="bib.fullscreen.headline">noFilter Combobox Header</span>
  <span slot="label">Name</span>
  <auro-menu>
    <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
    <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
    <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
    <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
    <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
    <auro-menuoption static nomatch>No matching option</auro-menuoption>
  </auro-menu>
</auro-combobox>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### error

Sets a persistent error state (e.g. an error state returned from the server).

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/error.html) -->
  <!-- The below content is automatically added from ./../apiExamples/error.html -->
  <auro-combobox error="Custom error message">
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption value="Prefer Alaska" id="option-5">Prefer Alaska</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceError.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearanceError.html -->
  <auro-combobox appearance="inverse" error="Custom error message">
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption value="Prefer Alaska" id="option-5">Prefer Alaska</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/error.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/error.html -->

```html
<auro-combobox error="Custom error message">
  <span slot="bib.fullscreen.headline">Bib Header</span>
  <span slot="label">Name</span>
  <auro-menu>
    <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
    <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
    <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
    <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
    <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
    <auro-menuoption value="Prefer Alaska" id="option-5">Prefer Alaska</auro-menuoption>
    <auro-menuoption static nomatch>No matching option</auro-menuoption>
  </auro-menu>
</auro-combobox>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceError.html) -->
<!-- The below content is automatically added from ./../apiExamples/inverseAppearanceError.html -->
<auro-combobox appearance="inverse" error="Custom error message">
  <span slot="bib.fullscreen.headline">Bib Header</span>
  <span slot="label">Name</span>
  <auro-menu>
    <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
    <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
    <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
    <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
    <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
    <auro-menuoption value="Prefer Alaska" id="option-5">Prefer Alaska</auro-menuoption>
    <auro-menuoption static nomatch>No matching option</auro-menuoption>
  </auro-menu>
</auro-combobox>
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### noValidate

Intended for use with the `required` attribute. If set, disables auto-validation on blur. By using these two attributes in combination the validation for required fields is still computed for forms but no validation messaging will be generated in the UI.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/noValidate.html) -->
  <!-- The below content is automatically added from ./../apiExamples/noValidate.html -->
  <auro-combobox required noValidate>
    <span slot="bib.fullscreen.headline">noValidate Combobox Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption value="Prefer Alaska" id="option-5">Prefer Alaska</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/noValidate.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/noValidate.html -->

```html
<auro-combobox required noValidate>
  <span slot="bib.fullscreen.headline">noValidate Combobox Header</span>
  <span slot="label">Name</span>
  <auro-menu>
    <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
    <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
    <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
    <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
    <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
    <auro-menuoption value="Prefer Alaska" id="option-5">Prefer Alaska</auro-menuoption>
    <auro-menuoption static nomatch>No matching option</auro-menuoption>
  </auro-menu>
</auro-combobox>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### required

Populates the `required` attribute on the input. Used for client-side validation.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/required.html) -->
  <!-- The below content is automatically added from ./../apiExamples/required.html -->
  <auro-combobox required>
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption value="Prefer Alaska" id="option-5">Prefer Alaska</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/required.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/required.html -->

```html
<auro-combobox required>
  <span slot="bib.fullscreen.headline">Bib Header</span>
  <span slot="label">Name</span>
  <auro-menu>
    <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
    <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
    <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
    <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
    <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
    <auro-menuoption value="Prefer Alaska" id="option-5">Prefer Alaska</auro-menuoption>
    <auro-menuoption static nomatch>No matching option</auro-menuoption>
  </auro-menu>
</auro-combobox>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Custom optional label <a name="optionalLabel"></a>
The `<auro-combobox>` supports an `optionalLabel` slot, where users can can override the default `(optional)` notification text.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/optionalLabel.html) -->
  <!-- The below content is automatically added from ./../apiExamples/optionalLabel.html -->
  <auro-combobox>
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Name</span>
    <span slot="optionalLabel" style="font-size: small; color: grey"> - optional</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/optionalLabel.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/optionalLabel.html -->

```html
<auro-combobox>
  <span slot="bib.fullscreen.headline">Bib Header</span>
  <span slot="label">Name</span>
  <span slot="optionalLabel" style="font-size: small; color: grey"> - optional</span>
  <auro-menu>
    <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
    <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
    <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
    <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
    <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
    <auro-menuoption static nomatch>No matching option</auro-menuoption>
  </auro-menu>
</auro-combobox>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### value

Use the `value` attribute to programmatically set the value of the combobox.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/programmaticValue.html) -->
  <!-- The below content is automatically added from ./../apiExamples/programmaticValue.html -->
  <auro-combobox>
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption value="Prefer Alaska" id="option-5">Prefer Alaska</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/programmaticValue.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/programmaticValue.html -->

```html
<auro-combobox>
  <span slot="bib.fullscreen.headline">Bib Header</span>
  <span slot="label">Name</span>
  <auro-menu>
    <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
    <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
    <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
    <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
    <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
    <auro-menuoption value="Prefer Alaska" id="option-5">Prefer Alaska</auro-menuoption>
    <auro-menuoption static nomatch>No matching option</auro-menuoption>
  </auro-menu>
</auro-combobox>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### Dynamically Set Value

Use the `value` attribute in combination with another element to dynamically set the value of the combobox.

Can be used in the following ways:
* Preset the value of the combobox to valid menu option
* Set the value of the combobox to invalid menu option
* Reset the value of the combobox to undefined

Note: using a value that does not match a menu option will reset the combobox value to undefined.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/value.html) -->
  <!-- The below content is automatically added from ./../apiExamples/value.html -->
  <auro-button id="valueValidExampleBtn">Set to an existing option</auro-button>
  <auro-button id="valueInvalidExampleBtn">Set to custom value</auro-button>
  <auro-button id="valueUndefinedExampleBtn">Reset</auro-button>
  <br/><br/>
  <auro-combobox id="valueExample">
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption value="Prefer Alaska" id="option-5">Prefer Alaska</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/value.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/value.html -->

```html
<auro-button id="valueValidExampleBtn">Set to an existing option</auro-button>
<auro-button id="valueInvalidExampleBtn">Set to custom value</auro-button>
<auro-button id="valueUndefinedExampleBtn">Reset</auro-button>
<br/><br/>
<auro-combobox id="valueExample">
  <span slot="bib.fullscreen.headline">Bib Header</span>
  <span slot="label">Name</span>
  <auro-menu>
    <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
    <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
    <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
    <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
    <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
    <auro-menuoption value="Prefer Alaska" id="option-5">Prefer Alaska</auro-menuoption>
    <auro-menuoption static nomatch>No matching option</auro-menuoption>
  </auro-menu>
</auro-combobox>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/value.js) -->
<!-- The below code snippet is automatically added from ./../apiExamples/value.js -->

```js
export function valueExample() {
  const valueExample = document.querySelector('#valueExample');

  document.querySelector('#valueValidExampleBtn').addEventListener('click', () => {
    valueExample.value = 'Oranges';
  });

  document.querySelector('#valueInvalidExampleBtn').addEventListener('click', () => {
    valueExample.value = 'Dragon Fruit';
  });

  document.querySelector('#valueUndefinedExampleBtn').addEventListener('click', () => {
    valueExample.value = undefined;
  });
}
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### type

When defined, the `auro-input` in the combobox trigger will use the defined `type` (e.g. `credit-card`).

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/typeMonthDayYear.html) -->
  <!-- The below content is automatically added from ./../apiExamples/typeMonthDayYear.html -->
  <auro-combobox type="date" triggerIcon>
    <span slot="bib.fullscreen.headline">Date Combobox Header</span>
    <span slot="label">Date</span>
    <auro-menu>
      <auro-menuoption value="01/02/2020" id="option-date-0">
        01/02/2020
      </auro-menuoption>
      <auro-menuoption value="05/16/2022" id="option-date-1">
        05/16/2022
      </auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/typeMonthDayYear.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/typeMonthDayYear.html -->

```html
<auro-combobox type="date" triggerIcon>
  <span slot="bib.fullscreen.headline">Date Combobox Header</span>
  <span slot="label">Date</span>
  <auro-menu>
    <auro-menuoption value="01/02/2020" id="option-date-0">
      01/02/2020
    </auro-menuoption>
    <auro-menuoption value="05/16/2022" id="option-date-1">
      05/16/2022
    </auro-menuoption>
  </auro-menu>
</auro-combobox>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Method Examples

#### focus

The focus method will apply focus state to the combobox input field.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/focus.html) -->
  <!-- The below content is automatically added from ./../apiExamples/focus.html -->
  <auro-button id="focusExampleBtn">Apply focus to combobox</auro-button>
  <br /><br />
  <auro-combobox id="focusExample">
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/focus.js) -->
<!-- The below code snippet is automatically added from ./../apiExamples/focus.js -->

```js
export function focusExample() {
  const focusExample = document.querySelector('#focusExample');
  const focusExampleBtnElem = document.querySelector('#focusExampleBtn');

  focusExampleBtnElem.addEventListener('click', () => {
    focusExample.focus();
  });
}
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/focus.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/focus.html -->

```html
<auro-button id="focusExampleBtn">Apply focus to combobox</auro-button>
<br /><br />
<auro-combobox id="focusExample">
  <span slot="bib.fullscreen.headline">Bib Header</span>
  <span slot="label">Name</span>
  <auro-menu>
    <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
    <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
    <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
    <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
    <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
    <auro-menuoption static nomatch>No matching option</auro-menuoption>
  </auro-menu>
</auro-combobox>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### reset

Use the `reset()` method to reset the `<auro-combobox>`'s `value` and `validity` state. Doing so will preserve all other attributes and properties.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/resetState.html) -->
  <!-- The below content is automatically added from ./../apiExamples/resetState.html -->
  <auro-button id="resetStateBtn">Reset</auro-button>
  <br /><br />
  <auro-combobox id="resetStateExample" required>
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/resetState.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/resetState.html -->

```html
<auro-button id="resetStateBtn">Reset</auro-button>
<br /><br />
<auro-combobox id="resetStateExample" required>
  <span slot="bib.fullscreen.headline">Bib Header</span>
  <span slot="label">Name</span>
  <auro-menu>
    <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
    <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
    <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
    <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
    <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
    <auro-menuoption static nomatch>No matching option</auro-menuoption>
  </auro-menu>
</auro-combobox>
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

### Slot Examples

#### helpText

Sets the help text displayed below the trigger. The `helpText` slot can be used to provide additional context for the combobox. When using the `error` property, the `helpText` slot can be used to describe the error.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/helpText.html) -->
  <!-- The below content is automatically added from ./../apiExamples/helpText.html -->
  <auro-combobox>
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Name</span>
    <span slot="helpText">Custom help text</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption value="Prefer Alaska" id="option-5">Prefer Alaska</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/helpText.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/helpText.html -->

```html
<auro-combobox>
  <span slot="bib.fullscreen.headline">Bib Header</span>
  <span slot="label">Name</span>
  <span slot="helpText">Custom help text</span>
  <auro-menu>
    <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
    <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
    <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
    <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
    <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
    <auro-menuoption value="Prefer Alaska" id="option-5">Prefer Alaska</auro-menuoption>
    <auro-menuoption static nomatch>No matching option</auro-menuoption>
  </auro-menu>
</auro-combobox>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### Loading<a name="loading"></a>
While content is loading, the menu can either remain empty or display a loading placeholder

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/loading.html) -->
  <!-- The below content is automatically added from ./../apiExamples/loading.html -->
  <auro-combobox id="loadingExample">
    <span slot="bib.fullscreen.headline">Loading Combobox Header</span>
    <span slot="label">Please select a preference</span>
    <auro-menu id="loadingExampleComboboxMenu">
      <auro-loader slot="loadingIcon" orbit xs></auro-loader><span slot="loadingText">Loading...</span>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/loading.js) -->
<!-- The below code snippet is automatically added from ./../apiExamples/loading.js -->

```js
export function auroMenuLoadingExample() {
  const combobox = document.querySelector("#loadingExample");
  const menu = document.querySelector("#loadingExampleComboboxMenu");

  const emptyMenu = () => {
    const menuoptions = menu.querySelectorAll('auro-menuoption');
    menuoptions.forEach(mo => menu.removeChild(mo));
  }

  const fillMenu = () => {
    menu.innerHTML += `
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    `;
  }

  const load = () => {
    clearTimeout(load.id);
    emptyMenu();
    menu.setAttribute('loading', 'loading');
    load.id = setTimeout(() => {
      menu.removeAttribute('loading');
      fillMenu();
    }, 1000);

  }

  combobox.addEventListener("inputValue", (e) => {
    if (e.target.inputValue && e.target.value !== e.target.inputValue) {
      load();
    }
  });
}
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/loading.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/loading.html -->

```html
<auro-combobox id="loadingExample">
  <span slot="bib.fullscreen.headline">Loading Combobox Header</span>
  <span slot="label">Please select a preference</span>
  <auro-menu id="loadingExampleComboboxMenu">
    <auro-loader slot="loadingIcon" orbit xs></auro-loader><span slot="loadingText">Loading...</span>
  </auro-menu>
</auro-combobox>
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
    <auro-combobox offset="20" noFlip placement="bottom-end">
      <span slot="bib.fullscreen.headline">Bib Header</span>
      <span slot="label">Label</span>
      <span slot="helpText">bottom-end bib with 20px offset and noFlip</span>
      <auro-menu>
        <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
        <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
        <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
        <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
        <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
        <auro-menuoption static nomatch>No matching option</auro-menuoption>
      </auro-menu>
    </auro-combobox>
    <auro-combobox offset="20" placement="bottom-end">
      <span slot="bib.fullscreen.headline">Bib Header</span>
      <span slot="label">Label</span>
      <span slot="helpText">bottom-end bib with 20px offset and flip</span>
      <auro-menu>
        <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
        <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
        <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
        <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
        <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
        <auro-menuoption static nomatch>No matching option</auro-menuoption>
      </auro-menu>
    </auro-combobox>
    <auro-combobox offset="20" noFlip placement="right" autoPlacement>
      <span slot="bib.fullscreen.headline">Bib Header</span>
      <span slot="label">Label</span>
      <span slot="helpText">right bib with 20px offset, noFlip and autoPlacement</span>
      <auro-menu>
        <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
        <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
        <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
        <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
        <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
        <auro-menuoption static nomatch>No matching option</auro-menuoption>
      </auro-menu>
    </auro-combobox>
    <auro-combobox width="350px" offset="20" noFlip placement="bottom-start" shift>
      <span slot="bib.fullscreen.headline">Bib Header</span>
      <span slot="label">Label</span>
      <span slot="helpText">bottom-start bib with 20px offset, noFlip and shift</span>
      <auro-menu>
        <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
        <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
        <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
        <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
        <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
        <auro-menuoption static nomatch>No matching option</auro-menuoption>
      </auro-menu>
    </auro-combobox>
  </div>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/floaterConfig.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/floaterConfig.html -->

```html
<div style="width: 350px">
  <auro-combobox offset="20" noFlip placement="bottom-end">
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Label</span>
    <span slot="helpText">bottom-end bib with 20px offset and noFlip</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <auro-combobox offset="20" placement="bottom-end">
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Label</span>
    <span slot="helpText">bottom-end bib with 20px offset and flip</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <auro-combobox offset="20" noFlip placement="right" autoPlacement>
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Label</span>
    <span slot="helpText">right bib with 20px offset, noFlip and autoPlacement</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <auro-combobox width="350px" offset="20" noFlip placement="bottom-start" shift>
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Label</span>
    <span slot="helpText">bottom-start bib with 20px offset, noFlip and shift</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
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
  <auro-combobox fullscreenBreakpoint="lg">
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/fullscreenBreakpoint.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/fullscreenBreakpoint.html -->

```html
<auro-combobox fullscreenBreakpoint="lg">
  <span slot="bib.fullscreen.headline">Bib Header</span>
  <span slot="label">Name</span>
  <auro-menu>
    <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
    <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
    <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
    <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
    <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
    <auro-menuoption static nomatch>No matching option</auro-menuoption>
  </auro-menu>
</auro-combobox>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### in Dialog

The component can be in a dialog.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inDialog.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inDialog.html -->
  <div>
    <auro-button id="combobox-dialog-opener">Combobox in Dialog</auro-button>
    <auro-dialog id="combobox-dialog">
      <span slot="header">Combobox in Dialog</span>
      <div slot="content">
        <auro-combobox id="focusExample">
          <span slot="bib.fullscreen.headline">Bib Header</span>
          <span slot="label">Name</span>
          <auro-menu>
            <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
            <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
            <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
            <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
            <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
            <auro-menuoption static nomatch>No matching option</auro-menuoption>
          </auro-menu>
        </auro-combobox>
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
  <auro-button id="combobox-dialog-opener">Combobox in Dialog</auro-button>
  <auro-dialog id="combobox-dialog">
    <span slot="header">Combobox in Dialog</span>
    <div slot="content">
      <auro-combobox id="focusExample">
        <span slot="bib.fullscreen.headline">Bib Header</span>
        <span slot="label">Name</span>
        <auro-menu>
          <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
          <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
          <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
          <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
          <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
          <auro-menuoption static nomatch>No matching option</auro-menuoption>
        </auro-menu>
      </auro-combobox>
    </div>
  </auro-dialog>
</div>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/inDialog.js) -->
<!-- The below code snippet is automatically added from ./../apiExamples/inDialog.js -->

```js
export function inDialogExample() {
  document.querySelector("#combobox-dialog-opener").addEventListener("click", () => {
    const dialog = document.querySelector("#combobox-dialog");
    dialog.open = true;
  });
};
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### Custom display value

You can fully customize how selected values appear by using the `displayValue` slot. This slot allows you to pass in any HTML content. Only the `snowflake` and `emphasized` layouts are supported.

<div class="exampleWrapper--ondark">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/displayValueSlot.html) -->
  <!-- The below content is automatically added from ./../apiExamples/displayValueSlot.html -->
  <auro-combobox layout="snowflake" shape="snowflake" size="xl" appearance="inverse" value="Apples">
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
    <div slot="displayValue">
        <div class="mainText">Custom display value</div>
        <div class="subText">Any html can be used</div>
    </div>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/displayValueSlot.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/displayValueSlot.html -->

```html
<auro-combobox layout="snowflake" shape="snowflake" size="xl" appearance="inverse" value="Apples">
  <span slot="bib.fullscreen.headline">Bib Header</span>
  <span slot="label">Name</span>
  <auro-menu>
    <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
    <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
    <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
    <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
    <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
    <auro-menuoption static nomatch>No matching option</auro-menuoption>
  </auro-menu>
  <div slot="displayValue">
      <div class="mainText">Custom display value</div>
      <div class="subText">Any html can be used</div>
  </div>
</auro-combobox>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>
