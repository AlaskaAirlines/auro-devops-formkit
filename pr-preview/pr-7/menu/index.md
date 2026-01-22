<!--
The demo.md file is a compiled document. No edits should be made directly to this file.
README.md is created by running `npm run build:docs`.
This file is generated based on a template fetched from `./docs/partials/demo.md`
-->

# Menu

<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../docs/partials/description.md) -->
<!-- The below content is automatically added from ./../docs/partials/description.md -->
The `<auro-menu>` element provides a list of options for a user to select from.

A list of options is created within the `<slot>` of the `<auro-menu>` element by using the `<auro-menuoption>` element to define options. Use a standard `<hr>` element to create dividers within the list of options.

The `<auro-menu>` element is designed for contextual menus, e.g. a dropdown menus. They are not intended to be used for navigation menus which have a different semantic meaning. The `<auro-menu>` element does not support hide/show functionality within its scope. This functionality will be managed by a wrapping element such as a drop-down menu composite element.
<!-- AURO-GENERATED-CONTENT:END -->

## auro-menu use cases

<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../docs/partials/useCases.md) -->
<!-- The below content is automatically added from ./../docs/partials/useCases.md -->
The `<auro-menu>` element should be used in situations where users may:

* A user needs to select one option from a list of options.
<!-- AURO-GENERATED-CONTENT:END -->

## Example(s)

### Default

A basic `auro-menu` element with nested `auro-menuoption` elements to generate a list.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/basic.html) -->
  <!-- The below content is automatically added from ./../apiExamples/basic.html -->
  <auro-menu>
    <auro-menuoption value="stops">Stops</auro-menuoption>
    <auro-menuoption value="price">Price</auro-menuoption>
    <auro-menuoption value="duration">Duration</auro-menuoption>
    <auro-menuoption value="departure">Departure</auro-menuoption>
    <auro-menuoption value="arrival">Arrival</auro-menuoption>
  </auro-menu>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/basic.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/basic.html -->

```html
<auro-menu>
  <auro-menuoption value="stops">Stops</auro-menuoption>
  <auro-menuoption value="price">Price</auro-menuoption>
  <auro-menuoption value="duration">Duration</auro-menuoption>
  <auro-menuoption value="departure">Departure</auro-menuoption>
  <auro-menuoption value="arrival">Arrival</auro-menuoption>
</auro-menu>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Using Keys

When setting the `value` property, matches are actually performed on the value of the `key` property of the `auro-menuoption` and not the `value` property. By default, the value of `key` is equal to the value of the `value` property. However, for advanced use cases, the `key` value can be overriden to allow for more specific matches.

In the below example, there is a list of "popular" options at the top, with the same values repeated underneath. To allow more specific selections, we can add a `key` attribute to the top options to allow them to be more specifically selected, or to prevent them from interfering with matches on the lower options.

In the below example, setting the value of the menu `'stops'` will select the bottom-most option with the value `'stops'`, and setting the value of menu to `'stops-top'` will select the top-most option with the value `'stops'` since the key now differs from the value. In either case, the resulting value of the menu will be `'stops'` because the resulting value of the menu is based on the `value` property and not the `key` property.

Due to a limitation with Lit change detection to the `value` property, if multiple options with the same exist and one is selected, you must first clear the current value before attempting to select another option with the same value, even if the keys are unique. See code example below.

_Note: Since the value passed to the `value` property when programmatically setting it is overwritten with the proper derived value once the menu has updated, note that it will take one lifecycle before the `value` property is updated to the value that represents the actual menu state._

<div class="exampleWrapper">
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/keys.html) -->
<!-- The below content is automatically added from ./../apiExamples/keys.html -->
<auro-button id="stopsTopButton">Call `menu.value = 'stops-top'`</auro-button>
<auro-button id="stopsButton">Call `menu.value = 'stops'`</auro-button>
<auro-menu id="keys-menu">
  <auro-menuoption value="stops" key="stops-top">Stops</auro-menuoption>
  <auro-menuoption value="price" key="price-top">Price</auro-menuoption>
  <hr>
  <auro-menuoption value="duration">Duration</auro-menuoption>
  <auro-menuoption value="departure">Departure</auro-menuoption>
  <auro-menuoption value="arrival">Arrival</auro-menuoption>
  <auro-menuoption value="stops">Stops</auro-menuoption>
  <auro-menuoption value="price">Price</auro-menuoption>
</auro-menu>
<p id="output" class="body-sm"></p>
<!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/keys.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/keys.html -->

```html
<auro-button id="stopsTopButton">Call `menu.value = 'stops-top'`</auro-button>
<auro-button id="stopsButton">Call `menu.value = 'stops'`</auro-button>
<auro-menu id="keys-menu">
  <auro-menuoption value="stops" key="stops-top">Stops</auro-menuoption>
  <auro-menuoption value="price" key="price-top">Price</auro-menuoption>
  <hr>
  <auro-menuoption value="duration">Duration</auro-menuoption>
  <auro-menuoption value="departure">Departure</auro-menuoption>
  <auro-menuoption value="arrival">Arrival</auro-menuoption>
  <auro-menuoption value="stops">Stops</auro-menuoption>
  <auro-menuoption value="price">Price</auro-menuoption>
</auro-menu>
<p id="output" class="body-sm"></p>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/keys.js) -->
<!-- The below code snippet is automatically added from ./../apiExamples/keys.js -->

```js
export function initKeysExample() {
  const menu = document.getElementById('keys-menu');
  const stopsButton = document.getElementById('stopsButton');
  const stopsTopButton = document.getElementById('stopsTopButton');
  const output = document.getElementById('output');

  const createConsoleEntry = (message) => {
    const node = document.createElement('span');
    node.innerHTML = message;
    output.appendChild(node);
    output.appendChild(document.createElement('br'));
  };

  const resetConsole = () => {
    output.innerHTML = '';
  };

  const updateMenuValue = (value) => {
    resetConsole();
    createConsoleEntry(`Setting menu.value: <em>"${value}"</em>`);
    menu.value = '';
    menu.value = value;
    createConsoleEntry(`menu.value before next lifecycle: <em>"${menu.value}"</em>`);
    setTimeout(() => {
      createConsoleEntry(`menu.value after lifecycle: <em>"${menu.value}"</em>`);
    });
  };

  stopsButton.addEventListener('click', () => {
    updateMenuValue('stops');
  });

  stopsTopButton.addEventListener('click', () => {
    updateMenuValue('stops-top');
  });
};
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>