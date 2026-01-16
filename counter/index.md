<!--
The index.md file is a compiled document. No edits should be made directly to this file.

index.md is created by running `npm run build:markdownDocs`.

This file is generated based on a template fetched from `./docs/partials/index.md`
-->

# Counter

<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../docs/partials/description.md) -->
<!-- The below content is automatically added from ./../docs/partials/description.md -->
The `auro-counter` component is a ui element that enables a way to increment or decrement a single digit value. Common use case is inside the `auro-counter-group` to facilitate a collection of counters to add passenger types to a flight.
<!-- AURO-GENERATED-CONTENT:END -->

## Examples

### Basic Counter

The counter component provides a simple interface for incrementing or decrementing numeric values. It displays a label with increment/decrement buttons and the current value. This is the most basic implementation of a standalone counter:

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/basic-standalone.html) -->
  <!-- The below content is automatically added from ./../apiExamples/basic-standalone.html -->
  <auro-counter>
    Adults
  </auro-counter>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearance.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearance.html -->
  <auro-counter appearance="inverse">
    Adults
  </auro-counter>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/basic-standalone.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/basic-standalone.html -->

```html
<auro-counter>
  Adults
</auro-counter>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearance.html) -->
<!-- The below content is automatically added from ./../apiExamples/inverseAppearance.html -->
<auro-counter appearance="inverse">
  Adults
</auro-counter>
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Counter with Description

Adding a description provides additional context to users. The description appears below the main label and is useful for displaying important information or requirements:

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/basic-description.html) -->
  <!-- The below content is automatically added from ./../apiExamples/basic-description.html -->
  <auro-counter>
    Adults
    <span slot="description">18 years or older</span>
  </auro-counter>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceDescription.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearanceDescription.html -->
  <auro-counter appearance="inverse">
    Adults
    <span slot="description">18 years or older</span>
  </auro-counter>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/basic-description.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/basic-description.html -->

```html
<auro-counter>
  Adults
  <span slot="description">18 years or older</span>
</auro-counter>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceDescription.html) -->
<!-- The below content is automatically added from ./../apiExamples/inverseAppearanceDescription.html -->
<auro-counter appearance="inverse">
  Adults
  <span slot="description">18 years or older</span>
</auro-counter>
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Counter with Help Text

Help text is supported with counters, and can be added by targetting the `helptext` slot.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/counter-helptext.html) -->
  <!-- The below content is automatically added from ./../apiExamples/counter-helptext.html -->
  <auro-counter>
    Adults
    <span slot="helpText">This is help text for the counter</span>
  </auro-counter>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearance-counter-helptext.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearance-counter-helptext.html -->
  <auro-counter appearance="inverse">
    Adults
    <span slot="helpText">This is help text for the counter</span>
  </auro-counter>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/counter-helptext.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/counter-helptext.html -->

```html
<auro-counter>
  Adults
  <span slot="helpText">This is help text for the counter</span>
</auro-counter>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearance-counter-helptext.html) -->
<!-- The below content is automatically added from ./../apiExamples/inverseAppearance-counter-helptext.html -->
<auro-counter appearance="inverse">
  Adults
  <span slot="helpText">This is help text for the counter</span>
</auro-counter>
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Counter with Custom Error

A custom error can be set on the counter by adding the `error` attribute with the desired message.

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

### Basic Counter Group

Counter groups allow you to manage multiple related counters together. This is useful when you need to collect multiple quantities that are related, such as different passenger types:

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/basic.html) -->
  <!-- The below content is automatically added from ./../apiExamples/basic.html -->
  <auro-counter-group>
    <auro-counter>
      Short label
    </auro-counter>
    <auro-counter>
      Another short label
    </auro-counter>
    <auro-counter>
      This is an example of the wrapping behavior for a long label
    </auro-counter>
  </auro-counter-group>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceGroup.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearanceGroup.html -->
  <auro-counter-group appearance="inverse">
    <auro-counter>
      Short label
    </auro-counter>
    <auro-counter>
      Another short label
    </auro-counter>
    <auro-counter>
      This is an example of the wrapping behavior for a long label
    </auro-counter>
  </auro-counter-group>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/basic.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/basic.html -->

```html
<auro-counter-group>
  <auro-counter>
    Short label
  </auro-counter>
  <auro-counter>
    Another short label
  </auro-counter>
  <auro-counter>
    This is an example of the wrapping behavior for a long label
  </auro-counter>
</auro-counter-group>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceGroup.html) -->
<!-- The below content is automatically added from ./../apiExamples/inverseAppearanceGroup.html -->
<auro-counter-group appearance="inverse">
  <auro-counter>
    Short label
  </auro-counter>
  <auro-counter>
    Another short label
  </auro-counter>
  <auro-counter>
    This is an example of the wrapping behavior for a long label
  </auro-counter>
</auro-counter-group>
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Dropdown Counter Group

The dropdown mode provides a more compact interface, ideal for forms where space is limited. It collapses the counters into a dropdown that expands when clicked.

When using a dropdown, an additional layout, `snowflake`, is available for use:

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/dropdown-basic.html) -->
  <!-- The below content is automatically added from ./../apiExamples/dropdown-basic.html -->
  <auro-counter-group isDropdown>
    <span slot="ariaLabel.bib.close">Close Popup</span>
    <div slot="bib.fullscreen.headline">Passengers</div>
    <div slot="label">Passengers</div>
    <auro-counter>
      Adults
      <span slot="description">18 years or older</span>
    </auro-counter>
    <auro-counter>
      Children
      <span slot="description">2-17 years</span>
    </auro-counter>
  </auro-counter-group>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceDropdown.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearanceDropdown.html -->
  <auro-counter-group appearance="inverse" isDropdown>
    <div slot="bib.fullscreen.headline">Passengers</div>
    <div slot="label">Passengers</div>
    <auro-counter>
      Adults
      <span slot="description">18 years or older</span>
    </auro-counter>
    <auro-counter>
      Children
      <span slot="description">2-17 years</span>
    </auro-counter>
  </auro-counter-group>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/dropdown-snowflake.html) -->
  <!-- The below content is automatically added from ./../apiExamples/dropdown-snowflake.html -->
  <!-- Example of counter-group properties -->
  <auro-counter-group max="10" min="2" isDropdown layout="snowflake">
    <span slot="ariaLabel.bib.close">Close Popup</span>
    <div slot="bib.fullscreen.headline">Group fullscreen label</div>
    <auro-icon slot="typeIcon" category="interface" name="account-stroke" customColor></auro-icon>
    <div slot="label">Snowflake Dropdown Group</div>
    <div slot="helpText">Total must be between 2-10</div>
    <auro-counter>
      Counter 1
    </auro-counter>
    <auro-counter>
      Counter 2
    </auro-counter>
  </auro-counter-group>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearance-dropdown-snowflake.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearance-dropdown-snowflake.html -->
  <!-- Example of counter-group properties -->
  <auro-counter-group max="10" min="2" isDropdown layout="snowflake" appearance="inverse">
    <span slot="ariaLabel.bib.close">Close Popup</span>
    <div slot="bib.fullscreen.headline">Group fullscreen label</div>
    <auro-icon slot="typeIcon" category="interface" name="account-stroke" customColor></auro-icon>
    <div slot="label">Snowflake Dropdown Group</div>
    <div slot="helpText">Total must be between 2-10</div>
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
  <!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/dropdown-basic.html) -->
  <!-- The below code snippet is automatically added from ./../apiExamples/dropdown-basic.html -->
  ```html
  <auro-counter-group isDropdown>
    <span slot="ariaLabel.bib.close">Close Popup</span>
    <div slot="bib.fullscreen.headline">Passengers</div>
    <div slot="label">Passengers</div>
    <auro-counter>
      Adults
      <span slot="description">18 years or older</span>
    </auro-counter>
    <auro-counter>
      Children
      <span slot="description">2-17 years</span>
    </auro-counter>
  </auro-counter-group>
  ```
  <!-- AURO-GENERATED-CONTENT:END -->
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceDropdown.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearanceDropdown.html -->
  <auro-counter-group appearance="inverse" isDropdown>
    <div slot="bib.fullscreen.headline">Passengers</div>
    <div slot="label">Passengers</div>
    <auro-counter>
      Adults
      <span slot="description">18 years or older</span>
    </auro-counter>
    <auro-counter>
      Children
      <span slot="description">2-17 years</span>
    </auro-counter>
  </auro-counter-group>
  <!-- AURO-GENERATED-CONTENT:END -->
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/dropdown-snowflake.html) -->
  <!-- The below content is automatically added from ./../apiExamples/dropdown-snowflake.html -->
  <!-- Example of counter-group properties -->
  <auro-counter-group max="10" min="2" isDropdown layout="snowflake">
    <span slot="ariaLabel.bib.close">Close Popup</span>
    <div slot="bib.fullscreen.headline">Group fullscreen label</div>
    <auro-icon slot="typeIcon" category="interface" name="account-stroke" customColor></auro-icon>
    <div slot="label">Snowflake Dropdown Group</div>
    <div slot="helpText">Total must be between 2-10</div>
    <auro-counter>
      Counter 1
    </auro-counter>
    <auro-counter>
      Counter 2
    </auro-counter>
  </auro-counter-group>
  <!-- AURO-GENERATED-CONTENT:END -->
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearance-dropdown-snowflake.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearance-dropdown-snowflake.html -->
  <!-- Example of counter-group properties -->
  <auro-counter-group max="10" min="2" isDropdown layout="snowflake" appearance="inverse">
    <span slot="ariaLabel.bib.close">Close Popup</span>
    <div slot="bib.fullscreen.headline">Group fullscreen label</div>
    <auro-icon slot="typeIcon" category="interface" name="account-stroke" customColor></auro-icon>
    <div slot="label">Snowflake Dropdown Group</div>
    <div slot="helpText">Total must be between 2-10</div>
    <auro-counter>
      Counter 1
    </auro-counter>
    <auro-counter>
      Counter 2
    </auro-counter>
  </auro-counter-group>
  <!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>
