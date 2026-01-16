<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../docs/api.md) -->
<!-- The below content is automatically added from ./../docs/api.md -->

# auro-counter

## Properties

| Property     | Attribute    | Type      | Default     | Description                                      |
|--------------|--------------|-----------|-------------|--------------------------------------------------|
| [appearance](#appearance) | `appearance` | `string`  | "'default'" | Defines whether the component will be on lighter or darker backgrounds. |
| [disabled](#disabled)   | `disabled`   | `boolean` | false       | Indicates if the counter is disabled.            |
| [error](#error)      | `error`      | `string`  |             | Error state and message.<br />True if set, value is the error message. |
| [max](#max)        | `max`        | `number`  | 9           | The maximum value for the counter.               |
| [min](#min)        | `min`        | `number`  | 0           | The minimum value for the counter.               |
| [onDark](#onDark)     | `onDark`     | `boolean` | false       | DEPRECATED - use `appearance` instead.           |
| [validity](#validity)   | `validity`   | `string`  | "undefined" | The validity state of the counter.               |
| [value](#value)      | `value`      | `number`  | "undefined" | The current value of the counter.                |

## Methods

| Method      | Type                                   | Description                                      |
|-------------|----------------------------------------|--------------------------------------------------|
| [decrement](#decrement) | `(value?: number \| undefined): void`  | Decrements the value of the counter by 1. If a value is provided, it decrements by that amount.<br /><br />**value**: The amount to decrement by. |
| [increment](#increment) | `(value?: number \| undefined): void`  | Increments the counter value by 1. If a value is provided, it increments by that amount.<br /><br />**value**: The amount to increment by. |
| [validate](#validate)  | `(force?: boolean \| undefined): void` | Validates value.<br /><br />**force**: Whether to force validation. |

## Events

| Event   | Type                                           |
|---------|------------------------------------------------|
| [input](#input) | `CustomEvent<{ value: number \| undefined; }>` |

## Slots

| Name              | Description                                |
|-------------------|--------------------------------------------|
|                   | Main label content for the counter.        |
| `ariaLabel.minus` | Accessible label for the decrement button. |
| `ariaLabel.plus`  | Accessible label for the increment button. |
| [description](#description)     | Descriptive content for the counter.       |
| [helpText](#helpText)        | Help text content for the counter.         |

# auro-counter-group

## Properties

| Property                  | Attribute                 | Type                     | Default        | Description                                      |
|---------------------------|---------------------------|--------------------------|----------------|--------------------------------------------------|
| [appearance](#appearance)              | `appearance`              | `string`                 | "'default'"    | Defines whether the component will be on lighter or darker backgrounds. |
| [autoPlacement](#autoPlacement)           | `autoPlacement`           | `boolean`                | "false"        | If declared, bib's position will be automatically calculated where to appear. |
| [error](#error)                   | `error`                   | `string`                 |                | The current error message to display when the component is invalid. |
| [fullscreenBreakpoint](#fullscreenBreakpoint)    | `fullscreenBreakpoint`    | `string`                 | "sm"           | Defines the screen size breakpoint (`xs`, `sm`, `md`, `lg`, `xl`, `disabled`)<br />at which the dropdown switches to fullscreen mode on mobile. `disabled` indicates a dropdown should _never_ enter fullscreen.<br /><br />When expanded, the dropdown will automatically display in fullscreen mode<br />if the screen size is equal to or smaller than the selected breakpoint. |
| [isDropdown](#isDropdown)              | `isDropdown`              | `boolean`                | false          | Indicates if the counter group is displayed as a dropdown. |
| [largeFullscreenHeadline](#largeFullscreenHeadline) | `largeFullscreenHeadline` | `boolean`                | false          | If declared, make bib.fullscreen.headline in HeadingDisplay.<br />Otherwise, Heading 600. |
| [layout](#layout)                  |                           | `'classic'\|'snowflake'` |                | Determines the layout style of the counter group when it is a dropdown. Options are 'classic' or 'snowflake'. Default is 'classic'. |
| [matchWidth](#matchWidth)              | `matchWidth`              | `boolean`                | false          | If declared, the dropdown will expand to the width of its parent container.<br />Otherwise, the dropdown width will be determined by its content. |
| [max](#max)                     | `max`                     | `number`                 | "undefined"    | The maximum value allowed for the whole group of counters. |
| [min](#min)                     | `min`                     | `number`                 | "undefined"    | The minimum value allowed for the whole group of counters. |
| [noFlip](#noFlip)                  | `noFlip`                  | `boolean`                | "false"        | If declared, the bib will NOT flip to an alternate position<br />when there isn't enough space in the specified `placement`. |
| [offset](#offset)                  | `offset`                  | `number`                 | "0"            | Gap between the trigger element and bib.         |
| [onDark](#onDark)                  | `onDark`                  | `boolean`                | false          | DEPRECATED - use `appearance` instead.           |
| [placement](#placement)               | `placement`               | `string`                 | "bottom-start" | Position where the bib should appear relative to the trigger.<br />Accepted values:<br />"top" \| "right" \| "bottom" \| "left" \|<br />"bottom-start" \| "top-start" \| "top-end" \|<br />"right-start" \| "right-end" \| "bottom-end" \|<br />"left-start" \| "left-end". |
| [shift](#shift)                   | `shift`                   | `boolean`                | "false"        | If declared, the dropdown will shift its position to avoid being cut off by the viewport. |
| [total](#total)                   | `total`                   | `number`                 | "undefined"    | The total value of the counters.                 |
| [validity](#validity)                | `validity`                | `string`                 | "undefined"    | Reflects the validity state.                     |
| [value](#value)                   | `value`                   | `object`                 | "undefined"    | The current individual values of the nested counters. |

## Methods

| Method     | Type                                   | Description                                      |
|------------|----------------------------------------|--------------------------------------------------|
| [hideBib](#hideBib)  | `(): void`                             | Hides the dropdown bib if its open.              |
| [showBib](#showBib)  | `(): void`                             | Shows the dropdown bib if there are options to show. |
| [validate](#validate) | `(force?: boolean \| undefined): void` | Validates value.<br /><br />**force**: Whether to force validation. |

## Events

| Event   | Type                                             |
|---------|--------------------------------------------------|
| [input](#input) | `CustomEvent<{ total: number \| undefined; value: {} \| undefined; }>` |

## Slots

| Name                      | Description                                      |
|---------------------------|--------------------------------------------------|
| `ariaLabel.bib.close`     | Sets aria-label on close button in fullscreen bib |
| `bib.fullscreen.footer`   | Defines the footer to display at the bottom of fullscreen bib. Only used when `isDropdown` is true. |
| `bib.fullscreen.headline` | Defines the headline to display above menu-options. Only used when `isDropdown` is true. Required. |
| [default](#default)                 | Slot for counter elements.                       |
| [helpText](#helpText)                | Dropdown help text content. Only used when `isDropdown` is true. |
| [label](#label)                   | Dropdown label content. Only used when `isDropdown` is true. |
| [valueText](#valueText)               | Dropdown value text display. Only used when `isDropdown` is true. |
<!-- AURO-GENERATED-CONTENT:END -->

## API Examples

### Counter

#### Min/Max and Value
<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/counter-minmax.html) -->
  <!-- The below content is automatically added from ./../apiExamples/counter-minmax.html -->
  <auro-counter min="1" max="5" value="2">
    Adults
    <span slot="description">Min: 1, Max: 5</span>
  </auro-counter>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/counter-minmax.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/counter-minmax.html -->

```html
<auro-counter min="1" max="5" value="2">
  Adults
  <span slot="description">Min: 1, Max: 5</span>
</auro-counter>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### Disabled State

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/counter-disabled.html) -->
  <!-- The below content is automatically added from ./../apiExamples/counter-disabled.html -->
  <auro-counter disabled value="0">
    Disabled counter
    <span slot="description">This counter cannot be modified</span>
  </auro-counter>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceDisabled.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearanceDisabled.html -->
  <auro-counter appearance="inverse" disabled value="0">
    Disabled counter
    <span slot="description">This counter cannot be modified</span>
  </auro-counter>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/counter-disabled.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/counter-disabled.html -->

```html
<auro-counter disabled value="0">
  Disabled counter
  <span slot="description">This counter cannot be modified</span>
</auro-counter>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceDisabled.html) -->
<!-- The below content is automatically added from ./../apiExamples/inverseAppearanceDisabled.html -->
<auro-counter appearance="inverse" disabled value="0">
  Disabled counter
  <span slot="description">This counter cannot be modified</span>
</auro-counter>
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Counter Group

#### Group Properties
All available counter-group properties:

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/api-group-properties.html) -->
  <!-- The below content is automatically added from ./../apiExamples/api-group-properties.html -->
  <!-- Example of counter-group properties -->
  <auro-counter-group max="10" min="2" isDropdown>
    <div slot="bib.fullscreen.headline">Group fullscreen label</div>
    <div slot="label">Group with all properties</div>
    <div slot="helpText">Total must be between 2-10</div>
    <div slot="valueText">Custom total display</div>
    <auro-counter>
      Counter 1
    </auro-counter>
    <auro-counter>
      Counter 2
    </auro-counter>
  </auro-counter-group>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/api-group-properties.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/api-group-properties.html -->

```html
<!-- Example of counter-group properties -->
<auro-counter-group max="10" min="2" isDropdown>
  <div slot="bib.fullscreen.headline">Group fullscreen label</div>
  <div slot="label">Group with all properties</div>
  <div slot="helpText">Total must be between 2-10</div>
  <div slot="valueText">Custom total display</div>
  <auro-counter>
    Counter 1
  </auro-counter>
  <auro-counter>
    Counter 2
  </auro-counter>
</auro-counter-group>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### Available Slots
All available slots for both components:

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/api-slots.html) -->
  <!-- The below content is automatically added from ./../apiExamples/api-slots.html -->
  <!-- Example of all available slots -->
  <auro-counter-group isDropdown>
    <!-- Group slots -->
    <div slot="label">Group with all slots</div>
    <div slot="bib.fullscreen.headline">Group fullscreen label</div>
    <div slot="helpText">Help text appears below the group</div>
    <div slot="valueText">Custom value display</div>
    <!-- Counter with all slots -->
    <auro-counter>
      Default slot content
      <span slot="ariaLabel.minus">Custom Minus Button Label</span>
      <span slot="ariaLabel.plus">Custom Plus Button Label</span>
      <span slot="description">Description slot content</span>
    </auro-counter>
  </auro-counter-group>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/api-slots.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/api-slots.html -->

```html
<!-- Example of all available slots -->
<auro-counter-group isDropdown>
  <!-- Group slots -->
  <div slot="label">Group with all slots</div>
  <div slot="bib.fullscreen.headline">Group fullscreen label</div>
  <div slot="helpText">Help text appears below the group</div>
  <div slot="valueText">Custom value display</div>
  <!-- Counter with all slots -->
  <auro-counter>
    Default slot content
    <span slot="ariaLabel.minus">Custom Minus Button Label</span>
    <span slot="ariaLabel.plus">Custom Plus Button Label</span>
    <span slot="description">Description slot content</span>
  </auro-counter>
</auro-counter-group>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Event Handling
Listen for `input` events to react to user interactions.

<code id="eventOutput">
  Event values will appear here
</code><br><br>
<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/events.html) -->
  <!-- The below content is automatically added from ./../apiExamples/events.html -->
  <auro-counter-group id="eventExample">
    <auro-counter>
      Adults
    </auro-counter>
    <auro-counter>
      Children
    </auro-counter>
  </auro-counter-group>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/events.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/events.html -->

```html
<auro-counter-group id="eventExample">
  <auro-counter>
    Adults
  </auro-counter>
  <auro-counter>
    Children
  </auro-counter>
</auro-counter-group>
```
<!-- AURO-GENERATED-CONTENT:END -->
----

```javascript
const counter = document.getElementById('eventExample');
counter.addEventListener('input', (event) => {
  console.log(`Values updated: ${JSON.stringify(event.detail)}`);
});
```

</auro-accordion>

#### Custom Value Display
<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/dropdown-value-text.html) -->
  <!-- The below content is automatically added from ./../apiExamples/dropdown-value-text.html -->
  <div style="max-width: 350px;">
    <auro-counter-group isDropdown>
      <span slot="ariaLabel.bib.close">Close Popup</span>
      <span slot="bib.fullscreen.headline">Passengers</span>
      <div slot="valueText">Custom value text</div>
      <div slot="label"></div>
      <auro-counter>
        Adults
        <span slot="description">18 years or older</span>
      </auro-counter>
      <auro-counter>
        Children
        <span slot="description">Under 17 years old. Restrictions apply if traveling without an adult.</span>
      </auro-counter>
      <auro-counter>
        Lap Infants
        <span slot="description">Under 2 years</span>
      </auro-counter>
    </auro-counter-group>
  </div>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/dropdown-value-text.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/dropdown-value-text.html -->

```html
<div style="max-width: 350px;">
  <auro-counter-group isDropdown>
    <span slot="ariaLabel.bib.close">Close Popup</span>
    <span slot="bib.fullscreen.headline">Passengers</span>
    <div slot="valueText">Custom value text</div>
    <div slot="label"></div>
    <auro-counter>
      Adults
      <span slot="description">18 years or older</span>
    </auro-counter>
    <auro-counter>
      Children
      <span slot="description">Under 17 years old. Restrictions apply if traveling without an adult.</span>
    </auro-counter>
    <auro-counter>
      Lap Infants
      <span slot="description">Under 2 years</span>
    </auro-counter>
  </auro-counter-group>
</div>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Counter with Custom Error

A custom error can be set on the counter by adding the `error` attribute the desired message.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/counter-error.html) -->
  <!-- The below content is automatically added from ./../apiExamples/counter-error.html -->
  <auro-counter error="There is an error with the counter">
    Adults
  </auro-counter>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearance-counter-error.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearance-counter-error.html -->
  <auro-counter appearance="inverse" error="There is an error with the counter">
    Adults
  </auro-counter>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/counter-error.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/counter-error.html -->

```html
<auro-counter error="There is an error with the counter">
  Adults
</auro-counter>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearance-counter-error.html) -->
<!-- The below content is automatically added from ./../apiExamples/inverseAppearance-counter-error.html -->
<auro-counter appearance="inverse" error="There is an error with the counter">
  Adults
</auro-counter>
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Counter Dropdown with Errored Counters

A counter dropdown with counters in an errored state will display the errors for each errored counter by default

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/dropdown-error-basic.html) -->
  <!-- The below content is automatically added from ./../apiExamples/dropdown-error-basic.html -->
  <auro-counter-group isDropdown>
    <span slot="ariaLabel.bib.close">Close Popup</span>
    <div slot="bib.fullscreen.headline">Passengers</div>
    <div slot="label">Passengers</div>
    <auro-counter error="Cannot have less than 1 adult passenger">
      Adults
      <span slot="description">18 years or older</span>
    </auro-counter>
    <auro-counter error="Cannot have more than 2 child passengers">
      Children
      <span slot="description">2-17 years</span>
    </auro-counter>
  </auro-counter-group>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/dropdown-error-basic.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/dropdown-error-basic.html -->

```html
<auro-counter-group isDropdown>
  <span slot="ariaLabel.bib.close">Close Popup</span>
  <div slot="bib.fullscreen.headline">Passengers</div>
  <div slot="label">Passengers</div>
  <auro-counter error="Cannot have less than 1 adult passenger">
    Adults
    <span slot="description">18 years or older</span>
  </auro-counter>
  <auro-counter error="Cannot have more than 2 child passengers">
    Children
    <span slot="description">2-17 years</span>
  </auro-counter>
</auro-counter-group>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Counter Dropdown with Custom Error

The error message for a dropdown counter with errored counters can also be overridden with the `error` attribute.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/dropdown-error-custom.html) -->
  <!-- The below content is automatically added from ./../apiExamples/dropdown-error-custom.html -->
  <auro-counter-group error="Please select the appropriate number of passengers" isDropdown>
    <span slot="ariaLabel.bib.close">Close Popup</span>
    <div slot="bib.fullscreen.headline">Passengers</div>
    <div slot="label">Passengers</div>
    <auro-counter error="Cannot have less than 1 adult passenger">
      Adults
      <span slot="description">18 years or older</span>
    </auro-counter>
    <auro-counter error="Cannot have more than 2 child passengers">
      Children
      <span slot="description">2-17 years</span>
    </auro-counter>
  </auro-counter-group>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/dropdown-error-custom.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/dropdown-error-custom.html -->

```html
<auro-counter-group error="Please select the appropriate number of passengers" isDropdown>
  <span slot="ariaLabel.bib.close">Close Popup</span>
  <div slot="bib.fullscreen.headline">Passengers</div>
  <div slot="label">Passengers</div>
  <auro-counter error="Cannot have less than 1 adult passenger">
    Adults
    <span slot="description">18 years or older</span>
  </auro-counter>
  <auro-counter error="Cannot have more than 2 child passengers">
    Children
    <span slot="description">2-17 years</span>
  </auro-counter>
</auro-counter-group>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Group Max/Min

The group counter max or min property sets the value for all counters in the group. If a counter has a max value set, the group max attribute will override it. All increment buttons as a result will be disabled to prevent the group of counters from exceeding the group max.

**Example has group max set to 12**

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/group-max.html) -->
  <!-- The below content is automatically added from ./../apiExamples/group-max.html -->
  <auro-counter-group max="12" min="0">
    <auro-counter>
      Short label
    </auro-counter>
    <auro-counter>
      This is an example of the wrapping behavior for a long label
    </auro-counter>
  </auro-counter-group>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/group-max.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/group-max.html -->

```html
<auro-counter-group max="12" min="0">
  <auro-counter>
    Short label
  </auro-counter>
  <auro-counter>
    This is an example of the wrapping behavior for a long label
  </auro-counter>
</auro-counter-group>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Counter Max/Min

You can also individually set the max or min value for each counter in a group.

**Example has group max set to 12**

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/group-counter-max.html) -->
  <!-- The below content is automatically added from ./../apiExamples/group-counter-max.html -->
  <auro-counter-group max="12" min="0">
    <auro-counter max="5">
      This counter has a max value of 5
    </auro-counter>
    <auro-counter max="8">
      This counter has a max value of 8
    </auro-counter>
  </auro-counter-group>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/group-counter-max.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/group-counter-max.html -->

```html
<auro-counter-group max="12" min="0">
  <auro-counter max="5">
    This counter has a max value of 5
  </auro-counter>
  <auro-counter max="8">
    This counter has a max value of 8
  </auro-counter>
</auro-counter-group>
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
    <auro-counter-group isDropdown offset="20" placement="bottom-end">
      <div slot="bib.fullscreen.headline">Passengers</div>
      <span slot="label">Label</span>
      <span slot="helpText">bottom-end bib with 20px offset</span>
      <auro-counter>
        Adults
        <span slot="description">18 years or older</span>
      </auro-counter>
      <auro-counter>
        Children
        <span slot="description">2-17 years</span>
      </auro-counter>
    </auro-counter-group>
    <auro-counter-group isDropdown offset="20" placement="bottom-end" noFlip>
      <div slot="bib.fullscreen.headline">Passengers</div>
      <span slot="label">Label</span>
      <span slot="helpText">bottom-end bib with 20px offset and noFlip</span>
      <auro-counter>
        Adults
        <span slot="description">18 years or older</span>
      </auro-counter>
      <auro-counter>
        Children
        <span slot="description">2-17 years</span>
      </auro-counter>
    </auro-counter-group>
    <auro-counter-group isDropdown offset="20" placement="right" noFlip autoPlacement>
      <div slot="bib.fullscreen.headline">Passengers</div>
      <span slot="label">Label</span>
      <span slot="helpText">right bib with 20px offset, noFlip and autoPlacement</span>
      <auro-counter>
        Adults
        <span slot="description">18 years or older</span>
      </auro-counter>
      <auro-counter>
        Children
        <span slot="description">2-17 years</span>
      </auro-counter>
    </auro-counter-group>
    <auro-counter-group width="350px" isDropdown offset="20" placement="bottom-start" shift noFlip>
      <div slot="bib.fullscreen.headline">Passengers</div>
      <span slot="label">Label</span>
      <span slot="helpText">bottom-start with 20px offset, noFlip and shift enabled</span>
      <auro-counter>
        Adults
        <span slot="description">18 years or older</span>
      </auro-counter>
      <auro-counter>
        Children
        <span slot="description">2-17 years</span>
      </auro-counter>
    </auro-counter-group>
  </div>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/floaterConfig.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/floaterConfig.html -->

```html
<div style="width: 350px">
  <auro-counter-group isDropdown offset="20" placement="bottom-end">
    <div slot="bib.fullscreen.headline">Passengers</div>
    <span slot="label">Label</span>
    <span slot="helpText">bottom-end bib with 20px offset</span>
    <auro-counter>
      Adults
      <span slot="description">18 years or older</span>
    </auro-counter>
    <auro-counter>
      Children
      <span slot="description">2-17 years</span>
    </auro-counter>
  </auro-counter-group>
  <auro-counter-group isDropdown offset="20" placement="bottom-end" noFlip>
    <div slot="bib.fullscreen.headline">Passengers</div>
    <span slot="label">Label</span>
    <span slot="helpText">bottom-end bib with 20px offset and noFlip</span>
    <auro-counter>
      Adults
      <span slot="description">18 years or older</span>
    </auro-counter>
    <auro-counter>
      Children
      <span slot="description">2-17 years</span>
    </auro-counter>
  </auro-counter-group>
  <auro-counter-group isDropdown offset="20" placement="right" noFlip autoPlacement>
    <div slot="bib.fullscreen.headline">Passengers</div>
    <span slot="label">Label</span>
    <span slot="helpText">right bib with 20px offset, noFlip and autoPlacement</span>
    <auro-counter>
      Adults
      <span slot="description">18 years or older</span>
    </auro-counter>
    <auro-counter>
      Children
      <span slot="description">2-17 years</span>
    </auro-counter>
  </auro-counter-group>
  <auro-counter-group width="350px" isDropdown offset="20" placement="bottom-start" shift noFlip>
    <div slot="bib.fullscreen.headline">Passengers</div>
    <span slot="label">Label</span>
    <span slot="helpText">bottom-start with 20px offset, noFlip and shift enabled</span>
    <auro-counter>
      Adults
      <span slot="description">18 years or older</span>
    </auro-counter>
    <auro-counter>
      Children
      <span slot="description">2-17 years</span>
    </auro-counter>
  </auro-counter-group>
</div>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Dropdown with fullscreen bib

You can make the dropdown open in fullscreen at a specific breakpoint by setting `fullscreenBreakpoint`.

The default value of `fullscreenBreakpoint` is `sm`. 

Breakpoint token can be found [here](https://auro.alaskaair.com/getting-started/developers/design-tokens)

To support fullscreen bib, setting the `bib.fullscreen.headline` slot is **REQUIRED**.
You can also set `bib.fullscreen.footer` slot to add any additional options on fullscreen view.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/dropdown-mobile-properties.html) -->
  <!-- The below content is automatically added from ./../apiExamples/dropdown-mobile-properties.html -->
  <div style="max-width: 350px;">
    <auro-counter-group id="dropdownCouterExample" isDropdown fullscreenBreakpoint="lg">
      <span slot="ariaLabel.bib.close">Close Popup</span>
      <span slot="label">Passengers</span>
      <span slot="bib.fullscreen.headline">Passengers</span>
      <div slot="helpText">This is help text</div>
      <auro-counter>
        Adults
        <span slot="description">18 years or older</span>
      </auro-counter>
      <auro-counter>
        Children
        <span slot="description">Under 17 years old. Restrictions apply if traveling without an adult.</span>
      </auro-counter>
      <auro-counter>
        Lap Infants
        <span slot="description">Under 2 years</span>
      </auro-counter>
      <div slot="bib.fullscreen.footer" style="display:flex; justify-content: stretch; gap: 1.5rem">
        <auro-button id="dropdownCounterExampleResetbutton" fluid variant="secondary" style="flex: 1 50%">Reset</auro-button>
        <auro-button id="dropdownCounterExampleSavebutton" fluid style="flex: 1 50%">Save</auro-button>
      </div>
    </auro-counter-group>
  </div>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/dropdown-mobile-properties.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/dropdown-mobile-properties.html -->

```html
<div style="max-width: 350px;">
  <auro-counter-group id="dropdownCouterExample" isDropdown fullscreenBreakpoint="lg">
    <span slot="ariaLabel.bib.close">Close Popup</span>
    <span slot="label">Passengers</span>
    <span slot="bib.fullscreen.headline">Passengers</span>
    <div slot="helpText">This is help text</div>
    <auro-counter>
      Adults
      <span slot="description">18 years or older</span>
    </auro-counter>
    <auro-counter>
      Children
      <span slot="description">Under 17 years old. Restrictions apply if traveling without an adult.</span>
    </auro-counter>
    <auro-counter>
      Lap Infants
      <span slot="description">Under 2 years</span>
    </auro-counter>
    <div slot="bib.fullscreen.footer" style="display:flex; justify-content: stretch; gap: 1.5rem">
      <auro-button id="dropdownCounterExampleResetbutton" fluid variant="secondary" style="flex: 1 50%">Reset</auro-button>
      <auro-button id="dropdownCounterExampleSavebutton" fluid style="flex: 1 50%">Save</auro-button>
    </div>
  </auro-counter-group>
</div>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>
