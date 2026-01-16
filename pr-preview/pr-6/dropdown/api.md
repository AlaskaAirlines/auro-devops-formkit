<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../docs/api.md) -->
<!-- The below content is automatically added from ./../docs/api.md -->

# auro-dropdown

## Properties

| Property                | Attribute               | Type        | Default        | Description                                      |
|-------------------------|-------------------------|-------------|----------------|--------------------------------------------------|
| `a11yRole`              |                         |             |                | The value for the role attribute of the trigger element. |
| [appearance](#appearance)            | `appearance`            | `string`    | "'default'"    | Defines whether the component will be on lighter or darker backgrounds. |
| [autoPlacement](#autoPlacement)         | `autoPlacement`         | `boolean`   | "false"        | If declared, bib's position will be automatically calculated where to appear. |
| [chevron](#chevron)               | `chevron`               | ` Boolean ` |                | If declared, the dropdown displays a chevron on the right. |
| [disableEventShow](#disableEventShow)      | `disableEventShow`      | ` Boolean ` | "false"        | If declared, the dropdown will only show by calling the API .show() public method. |
| [disableFocusTrap](#disableFocusTrap)      | `disableFocusTrap`      | `boolean`   |                | If declared, the focus trap inside of bib will be turned off. |
| [disabled](#disabled)              | `disabled`              | ` Boolean ` |                | If declared, the dropdown is not interactive.    |
| [error](#error)                 | `error`                 | ` Boolean ` |                | If declared in combination with not using the `simple` property or `helpText` slot content, will apply red color to both. |
| [errorMessage](#errorMessage)          | `errorMessage`          | `string`    | "undefined"    | Contains the help text message for the current validity error. |
| [focusShow](#focusShow)             | `focusShow`             | ` Boolean ` |                | If declared, the bib will display when focus is applied to the trigger. |
| [fullscreenBreakpoint](#fullscreenBreakpoint)  | `fullscreenBreakpoint`  | ` String `  | "sm"           | Defines the screen size breakpoint (`xs`, `sm`, `md`, `lg`, `xl`, `disabled`)<br />at which the dropdown switches to fullscreen mode on mobile. `disabled` indicates a dropdown should _never_ enter fullscreen.<br /><br />When expanded, the dropdown will automatically display in fullscreen mode<br />if the screen size is equal to or smaller than the selected breakpoint. |
| [hoverToggle](#hoverToggle)           | `hoverToggle`           | ` Boolean ` |                | If declared, the trigger will toggle the dropdown on mouseover/mouseout. |
| [isBibFullscreen](#isBibFullscreen)       | `isBibFullscreen`       | `boolean`   | false          | If true, the dropdown bib is taking the fullscreen when it's open. |
| [isPopoverVisible](#isPopoverVisible)      | `open`                  | ` Boolean ` | false          | If true, the dropdown bib is displayed.          |
| [layout](#layout)                |                         |             | "undefined"    |                                                  |
| [matchWidth](#matchWidth)            | `matchWidth`            | ` Boolean ` | false          | If declared, the popover and trigger will be set to the same width. |
| [noFlip](#noFlip)                | `noFlip`                | `boolean`   | "false"        | If declared, the bib will NOT flip to an alternate position<br />when there isn't enough space in the specified `placement`. |
| [noHideOnThisFocusLoss](#noHideOnThisFocusLoss) | `noHideOnThisFocusLoss` | ` Boolean ` | false          | If declared, the dropdown will not hide when moving focus outside the element. |
| [noToggle](#noToggle)              | `noToggle`              | ` Boolean ` |                | If declared, the trigger will only show the dropdown bib. |
| [offset](#offset)                | `offset`                | `number`    | "0"            | Gap between the trigger element and bib.         |
| [onDark](#onDark)                | `onDark`                | `boolean`   |                | DEPRECATED - use `appearance` instead.           |
| [onSlotChange](#onSlotChange)          | `onSlotChange`          |             |                | If declared, and a function is set, that function will execute when the slot content is updated. |
| [placement](#placement)             | `placement`             | `string`    | "bottom-start" | Position where the bib should appear relative to the trigger. |
| [shape](#shape)                 |                         |             | "undefined"    |                                                  |
| [shift](#shift)                 | `shift`                 | `boolean`   | "false"        | If declared, the dropdown will shift its position to avoid being cut off by the viewport. |
| [simple](#simple)                | `simple`                | `boolean`   |                | If declared, applies a border around the trigger slot. |
| [size](#size)                  |                         |             | "undefined"    |                                                  |

## Methods

| Method           | Type       | Description                                      |
|------------------|------------|--------------------------------------------------|
| [exposeCssParts](#exposeCssParts) | `(): void` | Exposes CSS parts for styling from parent components. |
| [focus](#focus)          | `(): void` | When bib is open, focus on the first element inside of bib.<br />If not, trigger element will get focus. |
| [hide](#hide)           | `(): void` | Public method to hide the dropdown.              |
| [show](#show)           | `(): void` | Public method to show the dropdown.              |

## Events

| Event                       | Type                                 | Description                                      |
|-----------------------------|--------------------------------------|--------------------------------------------------|
| `auroDropdown-idAdded`      | `Object<key  : 'id', value: string>` |                                                  |
| `auroDropdown-toggled`      |                                      | Notifies that the visibility of the dropdown bib has changed. |
| `auroDropdown-triggerClick` | `CustomEvent<any>`                   | Notifies that the trigger has been clicked.      |

## Slots

| Name       | Description                           |
|------------|---------------------------------------|
|            | Default slot for the popover content. |
| [helpText](#helpText) | Defines the content of the helpText.  |
| [trigger](#trigger)  | Defines the content of the trigger.   |

## CSS Shadow Parts

| Part       | Description                                      |
|------------|--------------------------------------------------|
| [chevron](#chevron)  | The collapsed/expanded state icon container.     |
| [helpText](#helpText) | The helpText content container.                  |
| [popover](#popover)  | The bib content container.                       |
| [size](#size)     | The size of the dropdown bib. (height, width, maxHeight, maxWidth only) |
| [trigger](#trigger)  | The trigger content container.                   |
<!-- AURO-GENERATED-CONTENT:END -->

## API Examples

### Basic

The most basic, simple version of `auro-dropdown`.

#### Text content in trigger

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/basic.html) -->
  <!-- The below content is automatically added from ./../apiExamples/basic.html -->
  <auro-dropdown aria-label="custom label">
    Lorem ipsum solar
    <div slot="trigger">
      Trigger
    </div>
  </auro-dropdown>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearance.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearance.html -->
  <auro-dropdown appearance="inverse" aria-label="custom label">
    Lorem ipsum solar
    <div slot="trigger">
      Trigger
    </div>
  </auro-dropdown>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/basic.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/basic.html -->

```html
<auro-dropdown aria-label="custom label">
  Lorem ipsum solar
  <div slot="trigger">
    Trigger
  </div>
</auro-dropdown>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearance.html) -->
<!-- The below content is automatically added from ./../apiExamples/inverseAppearance.html -->
<auro-dropdown appearance="inverse" aria-label="custom label">
  Lorem ipsum solar
  <div slot="trigger">
    Trigger
  </div>
</auro-dropdown>
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### Icon content in trigger

<div class="exampleWrapper">
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/basicIcon.html) -->
<!-- The below content is automatically added from ./../apiExamples/basicIcon.html -->
<auro-dropdown aria-label="custom label">
  Lorem ipsum solar
  <div slot="trigger">
    <auro-icon
      category="interface"
      name="arrow-down"></auro-icon>
  </div>
</auro-dropdown>
<!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/basicIcon.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/basicIcon.html -->

```html
<auro-dropdown aria-label="custom label">
  Lorem ipsum solar
  <div slot="trigger">
    <auro-icon
      category="interface"
      name="arrow-down"></auro-icon>
  </div>
</auro-dropdown>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>
<div class="exampleWrapper">
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/basicButton.html) -->
<!-- The below content is automatically added from ./../apiExamples/basicButton.html -->
<auro-dropdown aria-label="custom label">
  Lorem ipsum solar
  <div slot="trigger">
    <auro-button slot="trigger">
      Dropdown
    </auro-button>
  </div>
</auro-dropdown>
<!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/basicButton.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/basicButton.html -->

```html
<auro-dropdown aria-label="custom label">
  Lorem ipsum solar
  <div slot="trigger">
    <auro-button slot="trigger">
      Dropdown
    </auro-button>
  </div>
</auro-dropdown>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Property Examples

#### bordered

Adds the border style around the dropdown trigger.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/bordered.html) -->
  <!-- The below content is automatically added from ./../apiExamples/bordered.html -->
  <auro-dropdown aria-label="custom label" bordered>
    Lorem ipsum solar
    <div slot="trigger">
      Trigger
    </div>
  </auro-dropdown>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceBordered.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearanceBordered.html -->
  <auro-dropdown appearance="inverse" aria-label="custom label" layout="classic" shape="classic" size="lg">
    Lorem ipsum solar
    <div slot="trigger">
      Trigger
    </div>
  </auro-dropdown>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/bordered.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/bordered.html -->

```html
<auro-dropdown aria-label="custom label" bordered>
  Lorem ipsum solar
  <div slot="trigger">
    Trigger
  </div>
</auro-dropdown>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceBordered.html) -->
<!-- The below content is automatically added from ./../apiExamples/inverseAppearanceBordered.html -->
<auro-dropdown appearance="inverse" aria-label="custom label" layout="classic" shape="classic" size="lg">
  Lorem ipsum solar
  <div slot="trigger">
    Trigger
  </div>
</auro-dropdown>
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### chevron

Adds the bib visibility state chevron to the right side of the trigger content.

<div class="exampleWrapper">
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/chevron.html) -->
<!-- The below content is automatically added from ./../apiExamples/chevron.html -->
<auro-dropdown aria-label="custom label" chevron>
  Lorem ipsum solar
  <div slot="trigger">
    Trigger
  </div>
</auro-dropdown>
<!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/chevron.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/chevron.html -->

```html
<auro-dropdown aria-label="custom label" chevron>
  Lorem ipsum solar
  <div slot="trigger">
    Trigger
  </div>
</auro-dropdown>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>
<div class="exampleWrapper">
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/chevronIcon.html) -->
<!-- The below content is automatically added from ./../apiExamples/chevronIcon.html -->
<auro-dropdown aria-label="custom label" chevron>
  Lorem ipsum solar
  <div slot="trigger">
    <auro-icon
      category="interface"
      name="arrow-down"></auro-icon>
  </div>
</auro-dropdown>
<!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/chevronIcon.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/chevronIcon.html -->

```html
<auro-dropdown aria-label="custom label" chevron>
  Lorem ipsum solar
  <div slot="trigger">
    <auro-icon
      category="interface"
      name="arrow-down"></auro-icon>
  </div>
</auro-dropdown>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>
<div class="exampleWrapper">
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/chevronButton.html) -->
<!-- The below content is automatically added from ./../apiExamples/chevronButton.html -->
<auro-dropdown aria-label="custom label" chevron>
  Lorem ipsum solar
  <div slot="trigger">
    <auro-button slot="trigger">
      Dropdown
    </auro-button>
  </div>
</auro-dropdown>
<!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/chevronButton.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/chevronButton.html -->

```html
<auro-dropdown aria-label="custom label" chevron>
  Lorem ipsum solar
  <div slot="trigger">
    <auro-button slot="trigger">
      Dropdown
    </auro-button>
  </div>
</auro-dropdown>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>
<div class="exampleWrapper">
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/chevronInput.html) -->
<!-- The below content is automatically added from ./../apiExamples/chevronInput.html -->
<auro-dropdown aria-label="custom label" chevron>
  Lorem ipsum solar
  <div slot="trigger">
    <auro-input
      slot="trigger"
      id="inputExampleTrigger">
    </auro-input>
  </div>
</auro-dropdown>
<!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/chevronInput.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/chevronInput.html -->

```html
<auro-dropdown aria-label="custom label" chevron>
  Lorem ipsum solar
  <div slot="trigger">
    <auro-input
      slot="trigger"
      id="inputExampleTrigger">
    </auro-input>
  </div>
</auro-dropdown>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### disabled

Disables the trigger preventing the dropdown bib from being shown.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/disabled.html) -->
  <!-- The below content is automatically added from ./../apiExamples/disabled.html -->
  <auro-dropdown
    aria-label="custom label"
    disabled
    chevron
    rounded
    inset
    bordered>
    Lorem ipsum solar
    <div slot="trigger">
      Trigger
    </div>
    <span slot="helpText">
      Helper text
    </span>
    <span slot="label">
      Name
    </span>
  </auro-dropdown>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceDisabled.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearanceDisabled.html -->
  <auro-dropdown
    aria-label="custom label"
    disabled
    appearance="inverse"
    chevron
    layout="classic" shape="classic" size="lg">
    Lorem ipsum solar
    <div slot="trigger">
      Trigger
    </div>
    <span slot="helpText">
      Helper text
    </span>
    <span slot="label">
      Name
    </span>
  </auro-dropdown>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/disabled.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/disabled.html -->

```html
<auro-dropdown
  aria-label="custom label"
  disabled
  chevron
  rounded
  inset
  bordered>
  Lorem ipsum solar
  <div slot="trigger">
    Trigger
  </div>
  <span slot="helpText">
    Helper text
  </span>
  <span slot="label">
    Name
  </span>
</auro-dropdown>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/inverseAppearanceDisabled.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/inverseAppearanceDisabled.html -->

```html
<auro-dropdown
  aria-label="custom label"
  disabled
  appearance="inverse"
  chevron
  layout="classic" shape="classic" size="lg">
  Lorem ipsum solar
  <div slot="trigger">
    Trigger
  </div>
  <span slot="helpText">
    Helper text
  </span>
  <span slot="label">
    Name
  </span>
</auro-dropdown>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### error

Adds the error state UI to the trigger.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/error.html) -->
  <!-- The below content is automatically added from ./../apiExamples/error.html -->
  <auro-dropdown common error id="commonSlotError">
    <div style="padding: var(--ds-size-150);">
      Lorem ipsum solar
      <br />
      <auro-button onclick="document.querySelector('#commonSlotError').hide()">
        Dismiss Dropdown
      </auro-button>
    </div>
    <span slot="helpText">
      Help text
    </span>
    <span slot="label">
      Element label (default text will be read by screen reader)
    </span>
    <div slot="trigger">
      Trigger
    </div>
  </auro-dropdown>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceError.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearanceError.html -->
  <auro-dropdown appearance="inverse" layout="classic" shape="classic" size="lg" error id="commonSlotErrorOnDark">
    <div style="padding: var(--ds-size-150);">
      Lorem ipsum solar
      <br />
      <auro-button onclick="document.querySelector('#commonSlotErrorOnDark').hide()">
        Dismiss Dropdown
      </auro-button>
    </div>
    <span slot="helpText">
      Help text
    </span>
    <span slot="label">
      Element label (default text will be read by screen reader)
    </span>
    <div slot="trigger">
      Trigger
    </div>
  </auro-dropdown>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/error.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/error.html -->

```html
<auro-dropdown common error id="commonSlotError">
  <div style="padding: var(--ds-size-150);">
    Lorem ipsum solar
    <br />
    <auro-button onclick="document.querySelector('#commonSlotError').hide()">
      Dismiss Dropdown
    </auro-button>
  </div>
  <span slot="helpText">
    Help text
  </span>
  <span slot="label">
    Element label (default text will be read by screen reader)
  </span>
  <div slot="trigger">
    Trigger
  </div>
</auro-dropdown>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/inverseAppearanceError.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/inverseAppearanceError.html -->

```html
<auro-dropdown appearance="inverse" layout="classic" shape="classic" size="lg" error id="commonSlotErrorOnDark">
  <div style="padding: var(--ds-size-150);">
    Lorem ipsum solar
    <br />
    <auro-button onclick="document.querySelector('#commonSlotErrorOnDark').hide()">
      Dismiss Dropdown
    </auro-button>
  </div>
  <span slot="helpText">
    Help text
  </span>
  <span slot="label">
    Element label (default text will be read by screen reader)
  </span>
  <div slot="trigger">
    Trigger
  </div>
</auro-dropdown>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### noToggle

In cases where it is desired behavior for `auro-dropdown` to only show, not toggle, the bib content when activating the trigger the `noToggle` attribute must be applied.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/noToggle.html) -->
  <!-- The below content is automatically added from ./../apiExamples/noToggle.html -->
  <auro-dropdown aria-label="custom label" noToggle>
    Lorem ipsum solar
    <div slot="trigger">
      Trigger
    </div>
  </auro-dropdown>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/noToggle.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/noToggle.html -->

```html
<auro-dropdown aria-label="custom label" noToggle>
  Lorem ipsum solar
  <div slot="trigger">
    Trigger
  </div>
</auro-dropdown>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### fullscreenBreakpoint

On mobile view, adding the `fullscreenBreakpoint="{breakpoint-token}"` will switch the dropdown to fullscreen mode. 

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/customDimensions300.html) -->
  <!-- The below content is automatically added from ./../apiExamples/customDimensions300.html -->
  <style>
    #customDropdown300::part(size) {
      width: 300px;
      max-height: 200px;
    }
    </style>
  <div style="width: 300px;" aria-label="custom label">
    <auro-dropdown id="customDropdown300" layout="classic" shape="classic" size="lg" chevron fullscreenBreakpoint="sm">
      <div>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>
      </div>
      <div slot="trigger">
        Trigger
      </div>
    </auro-dropdown>
  </div>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/customDimensions300.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/customDimensions300.html -->

```html
<style>
  #customDropdown300::part(size) {
    width: 300px;
    max-height: 200px;
  }
  </style>
<div style="width: 300px;" aria-label="custom label">
  <auro-dropdown id="customDropdown300" layout="classic" shape="classic" size="lg" chevron fullscreenBreakpoint="sm">
    <div>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
      </p>
    </div>
    <div slot="trigger">
      Trigger
    </div>
  </auro-dropdown>
</div>
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
  <style>
    .floaterConfigDropdown::part(size) {
      width: 300px;
      max-height: 200px;
    }
  </style>
  <div aria-label="custom label">
    <auro-dropdown class="floaterConfigDropdown" layout="classic" shape="classic" size="lg" chevron placement="bottom-end" offset="20" noFlip>
      <div>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>
      </div>
      <div slot="trigger">
        Trigger
      </div>
      <span slot="helpText">Trigger for bottom-end bib with 20px offset and noFlip</span>
    </auro-dropdown>
  </div>
  <div aria-label="custom label">
    <auro-dropdown class="floaterConfigDropdown" layout="classic" shape="classic" size="lg" chevron placement="bottom-end" offset="20">
      <div>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>
      </div>
      <div slot="trigger">
        Trigger
      </div>
      <div slot="helpText">
        Trigger for bottom-end bib with 20px offset and flip
      </div>
    </auro-dropdown>
  </div>
  <div aria-label="custom label">
    <auro-dropdown class="floaterConfigDropdown" layout="classic" shape="classic" size="lg" chevron autoPlacement noFlip placement="right" offset="20">
      <div>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>
      </div>
      <div slot="trigger">
        Trigger
      </div>
      <div slot="helpText">
        Trigger for right bib with 20px offset, autoPlacement and noFlip
      </div>
    </auro-dropdown>
  </div>
  <div aria-label="custom label">
    <auro-dropdown width="350px" class="floaterConfigDropdown" layout="classic" shape="classic" size="lg" chevron noFlip placement="bottom-start" shift offset="20">
      <div width="500px">
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>
      </div>
      <div slot="trigger">
        Trigger
      </div>
      <div slot="helpText">
        Trigger for bottom-start bib with 20px offset, shift and noFlip
      </div>
    </auro-dropdown>
  </div>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/floaterConfig.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/floaterConfig.html -->

```html
<style>
  .floaterConfigDropdown::part(size) {
    width: 300px;
    max-height: 200px;
  }
</style>
<div aria-label="custom label">
  <auro-dropdown class="floaterConfigDropdown" layout="classic" shape="classic" size="lg" chevron placement="bottom-end" offset="20" noFlip>
    <div>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
      </p>
    </div>
    <div slot="trigger">
      Trigger
    </div>
    <span slot="helpText">Trigger for bottom-end bib with 20px offset and noFlip</span>
  </auro-dropdown>
</div>
<div aria-label="custom label">
  <auro-dropdown class="floaterConfigDropdown" layout="classic" shape="classic" size="lg" chevron placement="bottom-end" offset="20">
    <div>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
      </p>
    </div>
    <div slot="trigger">
      Trigger
    </div>
    <div slot="helpText">
      Trigger for bottom-end bib with 20px offset and flip
    </div>
  </auro-dropdown>
</div>
<div aria-label="custom label">
  <auro-dropdown class="floaterConfigDropdown" layout="classic" shape="classic" size="lg" chevron autoPlacement noFlip placement="right" offset="20">
    <div>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
      </p>
    </div>
    <div slot="trigger">
      Trigger
    </div>
    <div slot="helpText">
      Trigger for right bib with 20px offset, autoPlacement and noFlip
    </div>
  </auro-dropdown>
</div>
<div aria-label="custom label">
  <auro-dropdown width="350px" class="floaterConfigDropdown" layout="classic" shape="classic" size="lg" chevron noFlip placement="bottom-start" shift offset="20">
    <div width="500px">
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
      </p>
    </div>
    <div slot="trigger">
      Trigger
    </div>
    <div slot="helpText">
      Trigger for bottom-start bib with 20px offset, shift and noFlip
    </div>
  </auro-dropdown>
</div>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Slot Examples

#### default

All examples shown on this page include default slot content.

#### trigger

Content defined in the `trigger` slot will be rendered in the clickable trigger of the dropdown that is used to display the bib. Focus state visual effects will be disabled on the trigger when it contains a focusable element other than `<auro-input>`.

This slot may contain any static content (e.g. plain text) and/or no more than one of the following elements:
- `<a>`
- `<auro-hyperlink>`
- `<button>`
- `<auro-button>`
- `<input>`
- `<auro-input>`

#### label

Content defined in the `label` slot will be rendered left aligned inside the trigger above all other defined trigger slot content.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/label.html) -->
  <!-- The below content is automatically added from ./../apiExamples/label.html -->
  <auro-dropdown
    bordered
    rounded
    inset
    chevron>
    Lorem ipsum solar
    <span slot="label">Name</span>
    <div slot="trigger">
      Trigger
    </div>
  </auro-dropdown>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/label.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/label.html -->

```html
<auro-dropdown
  bordered
  rounded
  inset
  chevron>
  Lorem ipsum solar
  <span slot="label">Name</span>
  <div slot="trigger">
    Trigger
  </div>
</auro-dropdown>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### helpText

Content defined in the `helpText` slot will be rendered left aligned below the trigger. This slot requires the `auro-helptext` component be used as slot content for the helptext to render with the same styles as other form elements.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/helpText.html) -->
  <!-- The below content is automatically added from ./../apiExamples/helpText.html -->
  <auro-dropdown
    aria-label="custom label"
    inset
    bordered
    rounded>
    Lorem ipsum solar
    <span slot="helpText">
      Helper text
    </span>
    <div slot="trigger">
      Trigger
    </div>
  </auro-dropdown>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/helpText.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/helpText.html -->

```html
<auro-dropdown
  aria-label="custom label"
  inset
  bordered
  rounded>
  Lorem ipsum solar
  <span slot="helpText">
    Helper text
  </span>
  <div slot="trigger">
    Trigger
  </div>
</auro-dropdown>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#####

When combined with the `error` property the `helpText` slot content is colored red.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/helpTextError.html) -->
  <!-- The below content is automatically added from ./../apiExamples/helpTextError.html -->
  <auro-dropdown
    aria-label="custom label"
    inset
    bordered
    rounded
    error>
    Lorem ipsum solar
    <span slot="helpText">
      Helper text
    </span>
    <div slot="trigger">
      Trigger
    </div>
  </auro-dropdown>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/helpTextError.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/helpTextError.html -->

```html
<auro-dropdown
  aria-label="custom label"
  inset
  bordered
  rounded
  error>
  Lorem ipsum solar
  <span slot="helpText">
    Helper text
  </span>
  <div slot="trigger">
    Trigger
  </div>
</auro-dropdown>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Method Examples

#### show

The `show` method may also be called from anywhere in your code by executing `document.querySelector('#idOfTheDropdownElement').show()`. This example will execute the `show` method on a `keydown` event with focus in the input element.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/programmaticallyShow.html) -->
  <!-- The below content is automatically added from ./../apiExamples/programmaticallyShow.html -->
  <auro-input id="showExampleTriggerInput" required>
    <span slot="label">Enter a value to show the dropdown</span>
  </auro-input>
  <auro-dropdown id="showMethodExample" aria-label="custom label" layout="classic" shape="classic" size="lg">
    <p>
      Lorem ipsum solar
    </p>
    <span slot="trigger">Trigger Label</span>
  </auro-dropdown>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/programmaticallyShow.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/programmaticallyShow.html -->

```html
<auro-input id="showExampleTriggerInput" required>
  <span slot="label">Enter a value to show the dropdown</span>
</auro-input>
<auro-dropdown id="showMethodExample" aria-label="custom label" layout="classic" shape="classic" size="lg">
  <p>
    Lorem ipsum solar
  </p>
  <span slot="trigger">Trigger Label</span>
</auro-dropdown>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/programmaticallyShow.js) -->
<!-- The below code snippet is automatically added from ./../apiExamples/programmaticallyShow.js -->

```js
export function showExample() {
  const triggerInput = document.querySelector('#showExampleTriggerInput');
  const dropdownElem = document.querySelector('#showMethodExample');

  triggerInput.addEventListener('keydown', () => {
    dropdownElem.show();
  });
}
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### hide

The `hide` method can be called from within the default slot content. This is useful for cases such as `auro-select` when the dropdown should be collapsed after making a selection.

The `hide` method may also be called from anywhere in your code by executing `document.querySelector('#idOfTheDropdownElement').hide()`.

This example demonstrations collapsing the dropdown by clicking a button within the dropdown bib content.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/programmaticallyHide.html) -->
  <!-- The below content is automatically added from ./../apiExamples/programmaticallyHide.html -->
  <auro-dropdown id="hideExample" aria-label="custom label" layout="classic" shape="classic" size="lg">
    <p>
      Lorem ipsum solar
    </p>
    <auro-button id="hideExampleBtn">
      Dismiss Dropdown
    </auro-button>
    <auro-input
      slot="trigger"
      id="hideExampleTrigger">
    </auro-input>
  </auro-dropdown>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/programmaticallyHide.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/programmaticallyHide.html -->

```html
<auro-dropdown id="hideExample" aria-label="custom label" layout="classic" shape="classic" size="lg">
  <p>
    Lorem ipsum solar
  </p>
  <auro-button id="hideExampleBtn">
    Dismiss Dropdown
  </auro-button>
  <auro-input
    slot="trigger"
    id="hideExampleTrigger">
  </auro-input>
</auro-dropdown>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>
</auro-accordion>

### Other Examples

#### Width and Sizing Behavior

- **Width:** The `auro-dropdown` component will automatically consume the full width of its parent container. To make it narrower, you can style the `size` part.

- **Styling Options:** Only the following styles can be applied to the `size` part:
  - `width`
  - `height`
  - `maxWidth`
  - `maxHeight`

- **Scroll Behavior:** When the content exceeds the specified size, the browser will provide a scroll for the overflow.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/customDimensions100.html) -->
  <!-- The below content is automatically added from ./../apiExamples/customDimensions100.html -->
  <style>
    #customDropdown100::part(size) {
      width: 100px;
      max-height: 200px;
    }
  </style>
  <div style="width: 100px;" aria-label="custom label">
    <auro-dropdown id="customDropdown100" layout="classic" shape="classic" size="lg" chevron>
      <div>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
        </p>
      </div>
      <div slot="trigger">
        Trigger
      </div>
    </auro-dropdown>
  </div>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/customDimensions100.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/customDimensions100.html -->

```html
<style>
  #customDropdown100::part(size) {
    width: 100px;
    max-height: 200px;
  }
</style>
<div style="width: 100px;" aria-label="custom label">
  <auro-dropdown id="customDropdown100" layout="classic" shape="classic" size="lg" chevron>
    <div>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
      </p>
      <p>
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
      </p>
    </div>
    <div slot="trigger">
      Trigger
    </div>
  </auro-dropdown>
</div>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### In Auro Dialog

The component can be in a dialog.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inDialog.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inDialog.html -->
  <div>
    <auro-button id="dropdown-dialog-opener">Dropdown in Dialog</auro-button>
    <auro-dialog id="dropdown-dialog">
      <span slot="header">Dropdown in Dialog</span>
      <div slot="content">
        <auro-dropdown id="commonSlot" common bordered rounded inset chevron>
          <div style="padding: var(--ds-size-150);">
            Lorem ipsum solar
            <br />
            <auro-button onclick="document.querySelector('#commonSlot').hide()">
              Dismiss Dropdown
            </auro-button>
          </div>
          <span slot="helpText">
            Help text
          </span>
          <span slot="label">
            Element label (default text will be read by screen reader)
          </span>
          <div slot="trigger">
            Dropdown Trigger in Dialog
          </div>
        </auro-dropdown>
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
  <auro-button id="dropdown-dialog-opener">Dropdown in Dialog</auro-button>
  <auro-dialog id="dropdown-dialog">
    <span slot="header">Dropdown in Dialog</span>
    <div slot="content">
      <auro-dropdown id="commonSlot" common bordered rounded inset chevron>
        <div style="padding: var(--ds-size-150);">
          Lorem ipsum solar
          <br />
          <auro-button onclick="document.querySelector('#commonSlot').hide()">
            Dismiss Dropdown
          </auro-button>
        </div>
        <span slot="helpText">
          Help text
        </span>
        <span slot="label">
          Element label (default text will be read by screen reader)
        </span>
        <div slot="trigger">
          Dropdown Trigger in Dialog
        </div>
      </auro-dropdown>
    </div>
  </auro-dialog>
</div>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/inDialog.js) -->
<!-- The below code snippet is automatically added from ./../apiExamples/inDialog.js -->

```js
export function inDialogExample() {
  document.querySelector("#dropdown-dialog-opener").addEventListener("click", () => {
    const dialog = document.querySelector("#dropdown-dialog");
    dialog.open = true;
  });
};
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Theme Support

The component may be restyled using the following code sample and changing the values of the following token(s).

<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../src/styles/tokens.scss) -->
<!-- The below code snippet is automatically added from ./../src/styles/tokens.scss -->

```scss
@use "@aurodesignsystem/design-tokens/dist/themes/alaska/SCSSVariables--alaska" as v;
@use "@aurodesignsystem/design-tokens/dist/legacy/auro-classic/SCSSVariables" as vac;

:host(:not([ondark])),
:host(:not([appearance="inverse"])) {
  --ds-auro-dropdown-label-text-color: var(--ds-basic-color-texticon-muted, #{v.$ds-basic-color-texticon-muted});
  --ds-auro-dropdown-trigger-background-color: var(--ds-basic-color-surface-default, #{v.$ds-basic-color-surface-default});
  --ds-auro-dropdown-trigger-hover-background-color: var(--ds-basic-color-surface-default, #{v.$ds-basic-color-surface-default});
  --ds-auro-dropdown-trigger-container-color: var(--ds-basic-color-surface-default, #{v.$ds-basic-color-surface-default});
  --ds-auro-dropdown-trigger-border-color: var(--ds-basic-color-border-bold, #{v.$ds-basic-color-border-bold});
  --ds-auro-dropdown-trigger-outline-color: transparent;
  --ds-auro-dropdown-trigger-text-color: var(--ds-basic-color-texticon-default, #{v.$ds-basic-color-texticon-default});
  --ds-auro-dropdownbib-boxshadow-color: var(--ds-elevation-200, #{vac.$ds-elevation-200});
  --ds-auro-dropdownbib-background-color: var(--ds-basic-color-surface-default, #{v.$ds-basic-color-surface-default});
  --ds-auro-dropdownbib-container-color: var(--ds-basic-color-surface-default, #{v.$ds-basic-color-surface-default});
  --ds-auro-dropdownbib-text-color: var(--ds-basic-color-texticon-default, #{v.$ds-basic-color-texticon-default});
}

:host([ondark]),
:host([appearance="inverse"]) {
  --ds-auro-dropdown-label-text-color: var(--ds-basic-color-texticon-inverse-muted, #{v.$ds-basic-color-texticon-inverse-muted});
  --ds-auro-dropdown-trigger-background-color: var(--ds-advanced-color-shared-background-inverse, #{v.$ds-advanced-color-shared-background-inverse});
  --ds-auro-dropdown-trigger-hover-background-color: var(--ds-advanced-color-shared-background-inverse, #{v.$ds-advanced-color-shared-background-inverse});
  --ds-auro-dropdown-trigger-container-color: var(--ds-advanced-color-shared-background-inverse, #{v.$ds-advanced-color-shared-background-inverse});
  --ds-auro-dropdown-trigger-border-color: var(--ds-basic-color-border-inverse, #{v.$ds-basic-color-border-inverse});
  --ds-auro-dropdown-trigger-outline-color: transparent;
  --ds-auro-dropdown-trigger-text-color: var(--ds-basic-color-texticon-inverse, #{v.$ds-basic-color-texticon-inverse});
  --ds-auro-dropdownbib-boxshadow-color: var(--ds-elevation-200, #{vac.$ds-elevation-200});
  --ds-auro-dropdownbib-background-color: var(--ds-advanced-color-shared-background-inverse, #{v.$ds-advanced-color-shared-background-inverse});
  --ds-auro-dropdownbib-container-color: var(--ds-advanced-color-shared-background-inverse, #{v.$ds-advanced-color-shared-background-inverse});
  --ds-auro-dropdownbib-text-color: var(--ds-basic-color-texticon-inverse, #{v.$ds-basic-color-texticon-inverse});
}
```
<!-- AURO-GENERATED-CONTENT:END -->
