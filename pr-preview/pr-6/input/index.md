# Input

<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../docs/partials/description.md) -->
<!-- The below content is automatically added from ./../docs/partials/description.md -->
Use the `<auro-input>` custom element to create basic single-line text fields. Supports type `text`, `password`, and `email` with validation, required input, error states and a secondary `bordered` theme. Use the slots `label` and `helpText` for additional content support.
<!-- AURO-GENERATED-CONTENT:END -->

## auro-input use cases

<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../docs/partials/useCases.md) -->
<!-- The below content is automatically added from ./../docs/partials/useCases.md -->
The `<auro-input>` element should be used in situations where users may:

* needs to enter information
* be filling out a form
<!-- AURO-GENERATED-CONTENT:END -->

## Emphasized Layout

<div class="exampleWrapper--ondark">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/emphasized/basic.html) -->
  <!-- The below content is automatically added from ./../apiExamples/emphasized/basic.html -->
  <!-- <auro-input layout="default" shape="rounded" size="xl" placeholder="Departure">
    <label slot="label">From</label>
  </auro-input> -->
  <auro-input dvInputOnly id="alpha" value="lax" layout="emphasized" shape="pill" size="xl" placeholder="Departure" style="width: 249px;" appearance="inverse" required>
    <span slot="ariaLabel.clear">Clear All</span>
    <label slot="label">From</label>
    <span slot="helpText">Example help text</span>
    <span slot="displayValue">
      <div>
        <div class="subText">Los Angeles</div>
      </div>
    </span>
  </auro-input>
  <auro-input id="beta" layout="emphasized" shape="pill" size="xl" placeholder="Departure" style="width: 249px;" appearance="inverse" required>
    <span slot="ariaLabel.clear">Clear All</span>
    <label slot="label">From</label>
    <span slot="helpText">Example help text</span>
  </auro-input>
  <auro-input id="charlie" layout="emphasized-left" shape="pill-left" size="xl" placeholder="Departure" style="width: 249px;" appearance="inverse" required>
    <span slot="ariaLabel.clear">Clear All</span>
    <label slot="label">From</label>
    <span slot="helpText">Example help text</span>
  </auro-input>
  <auro-input id="delta" layout="emphasized-right" shape="pill-right" size="xl" placeholder="Departure" style="width: 249px;" appearance="inverse" required>
    <span slot="ariaLabel.clear">Clear All</span>
    <label slot="label">From</label>
    <span slot="helpText">Example help text</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>

## Snowflake Layout

<div class="exampleWrapper--ondark">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/snowflake/basic.html) -->
  <!-- The below content is automatically added from ./../apiExamples/snowflake/basic.html -->
  <auro-input dvInputOnly value="lax" id="snowflakePill" layout="snowflake" shape="snowflake" size="lg" placeholder="Departure" style="width: 249px;" appearance="inverse" required>
    <span slot="ariaLabel.clear">Clear All</span>
    <label slot="label">From</label>
    <span slot="helpText">Example help text</span>
    <span slot="displayValue">
      <div>
        <div class="subText">Los Angeles</div>
      </div>
    </span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>

## Default component

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

## Placeholder

Use the `placeholder` attribute to add a custom placeholder message within the element.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/placeholder.html) -->
  <!-- The below content is automatically added from ./../apiExamples/placeholder.html -->
  <auro-input placeholder="John Doe" required>
    <span slot="label">Full name</span>
    <span slot="helpText">Please enter your full name.</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/placeholder.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/placeholder.html -->

```html
<auro-input placeholder="John Doe" required>
  <span slot="label">Full name</span>
  <span slot="helpText">Please enter your full name.</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

## Disabled

Use the `disabled` attribute to prevent the user from interacting with the input.

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

## Active Label

Example use cases for auro-input support the `activeLabel` attribute. If set, the label will stay fixed in the active position.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/activeLabel.html) -->
  <!-- The below content is automatically added from ./../apiExamples/activeLabel.html -->
  <auro-input activeLabel>
    <span slot="label">Address</span>
    <span slot="helpText">Please enter your home address.</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/activeLabel.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/activeLabel.html -->

```html
<auro-input activeLabel>
  <span slot="label">Address</span>
  <span slot="helpText">Please enter your home address.</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

## Value

Use the `value` attribute to preset the value of the element.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/programmaticValue.html) -->
  <!-- The below content is automatically added from ./../apiExamples/programmaticValue.html -->
  <auro-input value="Alaska Airlines is the best!">
    <span slot="label">Name</span>
    <span slot="helpText">Please enter your full name.</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/programmaticValue.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/programmaticValue.html -->

```html
<auro-input value="Alaska Airlines is the best!">
  <span slot="label">Name</span>
  <span slot="helpText">Please enter your full name.</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

## Pattern

Use the `pattern` attribute to set custom input validation. This example also uses the `spellcheck` attribute set to `false` which in turn sets `autocorrect` to `off` and `autocapitalize` to `none`. Additionally the `maxlength` attribute sets the maximum length of characters that can be entered.

The `<auro-input>` component supports setting a custom validity message specific to the pattern validation by using the `setCustomValidityPatternMismatch` attribute.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/pattern.html) -->
  <!-- The below content is automatically added from ./../apiExamples/pattern.html -->
  <auro-input pattern="[a-z]{1,15}" spellcheck="false" setCustomValidityPatternMismatch="Only contain lowercase letters w/no spaces">
    <span slot="label">Username</span>
    <span slot="helpText">Please enter a username.</span>
  </auro-input>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/pattern.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/pattern.html -->

```html
<auro-input pattern="[a-z]{1,15}" spellcheck="false" setCustomValidityPatternMismatch="Only contain lowercase letters w/no spaces">
  <span slot="label">Username</span>
  <span slot="helpText">Please enter a username.</span>
</auro-input>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>
