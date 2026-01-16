<!--
The index.md file is a compiled document. No edits should be made directly to this file.
README.md is created by running `npm run build:docs`.
This file is generated based on a template fetched from `./docs/partials/index.md`
-->

# Radio

<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../docs/partials/description.md) -->
<!-- The below content is automatically added from ./../docs/partials/description.md -->
`<auro-radio>` is a [HTML custom element](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_custom_elements) that is rendered as a small circle, which is filled or highlighted when selected. Only one `<auro-radio>` component in a given `<auro-radio-group>` can be selected at the same time.
<!-- AURO-GENERATED-CONTENT:END -->

## auro-radio use cases

<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../docs/partials/useCases.md) -->
<!-- The below content is automatically added from ./../docs/partials/useCases.md -->
The `<auro-radio>` element is designed to be a single component for the use of creating an input `type="radio"` with an associated `<label>` that meets all use case and accessibility standards.

The following examples illustrate fully functional `<auro-radio>` elements wrapped with the `<auro-radio-group>` element. The `<auro-radio-group>` element is REQUIRED in order to mantain the relationship between individual `<auro-radio>` elements for functional radio button actions.

**Note**: The `<auro-radio>` element is only for to for use as a set of two or more `<auro-radio>` elements within an `<auro-radio-group>` element.
<!-- AURO-GENERATED-CONTENT:END -->

## Example(s)

### Default

This is a default configuration of `<auro-radio>`.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/basic.html) -->
  <!-- The below content is automatically added from ./../apiExamples/basic.html -->
  <auro-radio id="basicRadio1" label="Yes" name="radioDemo" value="yes"></auro-radio>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearance.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearance.html -->
  <auro-radio id="basicRadio1" label="Yes" name="radioDemo" value="yes" appearance="inverse"></auro-radio>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/basic.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/basic.html -->

```html
<auro-radio id="basicRadio1" label="Yes" name="radioDemo" value="yes"></auro-radio>
```
<!-- AURO-GENERATED-CONTENT:END -->
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearance.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearance.html -->
  <auro-radio id="basicRadio1" label="Yes" name="radioDemo" value="yes" appearance="inverse"></auro-radio>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
</auro-accordion>

### Default Group

This is a default configuration using the `<auro-radio-group>` and `<auro-radio>` elements. Notice the use of the `slot` attribute to set the group title of the `<auro-radio-group>`.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/basicGroup.html) -->
  <!-- The below content is automatically added from ./../apiExamples/basicGroup.html -->
  <auro-radio-group>
    <span slot="legend">Form label goes here</span>
    <auro-radio id="basicGroupRadio1" label="Yes" name="radioDemo" value="yes"></auro-radio>
    <auro-radio id="basicGroupRadio2" label="No" name="radioDemo" value="no"></auro-radio>
    <auro-radio id="basicGroupRadio3" label="Maybe" name="radioDemo" value="maybe"></auro-radio>
  </auro-radio-group>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceGroup.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearanceGroup.html -->
  <auro-radio-group appearance="inverse">
    <span slot="legend">Form label goes here</span>
    <auro-radio id="basicGroupRadio1" label="Yes" name="radioDemo" value="yes"></auro-radio>
    <auro-radio id="basicGroupRadio2" label="No" name="radioDemo" value="no"></auro-radio>
    <auro-radio id="basicGroupRadio3" label="Maybe" name="radioDemo" value="maybe"></auro-radio>
  </auro-radio-group>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
  <!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/basicGroup.html) -->
  <!-- The below code snippet is automatically added from ./../apiExamples/basicGroup.html -->
  ```html
  <auro-radio-group>
    <span slot="legend">Form label goes here</span>
    <auro-radio id="basicGroupRadio1" label="Yes" name="radioDemo" value="yes"></auro-radio>
    <auro-radio id="basicGroupRadio2" label="No" name="radioDemo" value="no"></auro-radio>
    <auro-radio id="basicGroupRadio3" label="Maybe" name="radioDemo" value="maybe"></auro-radio>
  </auro-radio-group>
  ```
  <!-- AURO-GENERATED-CONTENT:END -->
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceGroup.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearanceGroup.html -->
  <auro-radio-group appearance="inverse">
    <span slot="legend">Form label goes here</span>
    <auro-radio id="basicGroupRadio1" label="Yes" name="radioDemo" value="yes"></auro-radio>
    <auro-radio id="basicGroupRadio2" label="No" name="radioDemo" value="no"></auro-radio>
    <auro-radio id="basicGroupRadio3" label="Maybe" name="radioDemo" value="maybe"></auro-radio>
  </auro-radio-group>
  <!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Accordion Nested Group

This example shows how to use `<auro-accordion>` with the `<auro-radio-group>` and `<auro-radio>` elements for
nested/optional groups (such as a "More Options" section in a payment processor).

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/accordionExample.html) -->
  <!-- The below content is automatically added from ./../apiExamples/accordionExample.html -->
  <auro-radio-group>
    <span slot="legend">Accordion Test</span>
    <auro-radio id="basicGroupRadio1" label="Credit or debit card" name="creditordebit" value="credit"></auro-radio>
    <auro-radio id="basicGroupRadio2" label="Apple Pay" name="applePay" value="applePay"></auro-radio>
    <auro-radio id="basicGroupRadio3" label="Alaska Airlines Commercial Account" name="alaskaCommercial" value="alaskaCommercial"></auro-radio>
    <auro-accordion>
      <span slot="trigger">More payment options</span>
      <auro-radio id="basicGroupRadio4" label="Click to pay" name="manualCredit" value="manualCredit"></auro-radio>
      <auro-radio id="basicGroupRadio5" label="Google Pay" name="googlePay" value="googlePay"></auro-radio>
    </auro-accordion>
  </auro-radio-group>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/accordionExample.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/accordionExample.html -->

```html
<auro-radio-group>
  <span slot="legend">Accordion Test</span>
  <auro-radio id="basicGroupRadio1" label="Credit or debit card" name="creditordebit" value="credit"></auro-radio>
  <auro-radio id="basicGroupRadio2" label="Apple Pay" name="applePay" value="applePay"></auro-radio>
  <auro-radio id="basicGroupRadio3" label="Alaska Airlines Commercial Account" name="alaskaCommercial" value="alaskaCommercial"></auro-radio>
  <auro-accordion>
    <span slot="trigger">More payment options</span>
    <auro-radio id="basicGroupRadio4" label="Click to pay" name="manualCredit" value="manualCredit"></auro-radio>
    <auro-radio id="basicGroupRadio5" label="Google Pay" name="googlePay" value="googlePay"></auro-radio>
  </auro-accordion>
</auro-radio-group>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>
