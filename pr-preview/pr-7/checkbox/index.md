<!--
The index.md file is a compiled document. No edits should be made directly to this file.
README.md is created by running `npm run build:docs`.
This file is generated based on a template fetched from `./docs/partials/index.md`
-->

# Checkbox

<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../docs/partials/description.md) -->
<!-- The below content is automatically added from ./../docs/partials/description.md -->
`<auro-checkbox>` is a [HTML custom element](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_custom_elements) for the purpose of allowing users to select one or more options of a limited number of choices.
<!-- AURO-GENERATED-CONTENT:END -->

## auro-checkbox use cases

<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../docs/partials/useCases.md) -->
<!-- The below content is automatically added from ./../docs/partials/useCases.md -->
The `<auro-checkbox>` element should be used in situations where users may:

* Be filling out a form
* Need to select one or more options
<!-- AURO-GENERATED-CONTENT:END -->

## Additional Information

## Example(s)

### Default

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/basic.html) -->
  <!-- The below content is automatically added from ./../apiExamples/basic.html -->
  <auro-checkbox-group>
    <span slot="legend">Form label goes here</span>
    <auro-checkbox value="value1" name="basic" id="checkbox-basic1">Checkbox option</auro-checkbox>
    <auro-checkbox value="value2" name="basic" id="checkbox-basic2" checked>Checkbox option</auro-checkbox>
    <auro-checkbox value="value3" name="basic" id="checkbox-basic3">Checkbox option that has some extra text that should wrap when rendered in a narrow container</auro-checkbox>
    <auro-checkbox value="value4" name="basic" id="checkbox-basic4">Checkbox option</auro-checkbox>
  </auro-checkbox-group>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearance.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearance.html -->
  <auro-checkbox-group appearance="inverse">
    <span slot="legend">Form label goes here</span>
    <auro-checkbox value="value1" name="basic" id="checkbox-basic1">Checkbox option</auro-checkbox>
    <auro-checkbox value="value2" name="basic" id="checkbox-basic2" checked>Checkbox option</auro-checkbox>
    <auro-checkbox value="value3" name="basic" id="checkbox-basic3">Checkbox option</auro-checkbox>
    <auro-checkbox value="value4" name="basic" id="checkbox-basic4">Checkbox option</auro-checkbox>
  </auro-checkbox-group>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/basic.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/basic.html -->

```html
<auro-checkbox-group>
  <span slot="legend">Form label goes here</span>
  <auro-checkbox value="value1" name="basic" id="checkbox-basic1">Checkbox option</auro-checkbox>
  <auro-checkbox value="value2" name="basic" id="checkbox-basic2" checked>Checkbox option</auro-checkbox>
  <auro-checkbox value="value3" name="basic" id="checkbox-basic3">Checkbox option that has some extra text that should wrap when rendered in a narrow container</auro-checkbox>
  <auro-checkbox value="value4" name="basic" id="checkbox-basic4">Checkbox option</auro-checkbox>
</auro-checkbox-group>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearance.html) -->
<!-- The below content is automatically added from ./../apiExamples/inverseAppearance.html -->
<auro-checkbox-group appearance="inverse">
  <span slot="legend">Form label goes here</span>
  <auro-checkbox value="value1" name="basic" id="checkbox-basic1">Checkbox option</auro-checkbox>
  <auro-checkbox value="value2" name="basic" id="checkbox-basic2" checked>Checkbox option</auro-checkbox>
  <auro-checkbox value="value3" name="basic" id="checkbox-basic3">Checkbox option</auro-checkbox>
  <auro-checkbox value="value4" name="basic" id="checkbox-basic4">Checkbox option</auro-checkbox>
</auro-checkbox-group>
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Disabled

Use the `disabled` attribute to disable individual `<auro-checkbox>` elements or the entire `<auro-checkbox-group>`.

#### Disabled Checkbox within Group

The `disabled` attribute used to disable a single `<auro-checkbox>` element.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/disabled.html) -->
  <!-- The below content is automatically added from ./../apiExamples/disabled.html -->
  <auro-checkbox-group>
    <span slot="legend">Form label goes here</span>
    <auro-checkbox value="disabled-value1" name="disabled" id="checkbox-disabled1">Checkbox option</auro-checkbox>
    <auro-checkbox value="disabled-value2" name="disabled" id="checkbox-disabled2" checked disabled>Disabled checkbox option</auro-checkbox>
    <auro-checkbox value="disabled-value3" name="disabled" id="checkbox-disabled3" disabled>Disabled checkbox option</auro-checkbox>
    <auro-checkbox value="disabled-value4" name="disabled" id="checkbox-disabled4" checked>Checkbox option</auro-checkbox>
  </auro-checkbox-group>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/disabled.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/disabled.html -->

```html
<auro-checkbox-group>
  <span slot="legend">Form label goes here</span>
  <auro-checkbox value="disabled-value1" name="disabled" id="checkbox-disabled1">Checkbox option</auro-checkbox>
  <auro-checkbox value="disabled-value2" name="disabled" id="checkbox-disabled2" checked disabled>Disabled checkbox option</auro-checkbox>
  <auro-checkbox value="disabled-value3" name="disabled" id="checkbox-disabled3" disabled>Disabled checkbox option</auro-checkbox>
  <auro-checkbox value="disabled-value4" name="disabled" id="checkbox-disabled4" checked>Checkbox option</auro-checkbox>
</auro-checkbox-group>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### Disabled Group

The `disabled` attribute used to disable the entire `<auro-checkbox-group>`.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/disabledGroup.html) -->
  <!-- The below content is automatically added from ./../apiExamples/disabledGroup.html -->
  <auro-checkbox-group disabled>
    <span slot="legend">Form label goes here</span>
    <auro-checkbox value="disabled-value1" name="disabledGroup" id="checkbox-disabledGroup1">Disabled checkbox option</auro-checkbox>
    <auro-checkbox value="disabled-value2" name="disabledGroup" id="checkbox-disabledGroup2" checked>Disabled checkbox option</auro-checkbox>
    <auro-checkbox value="disabled-value3" name="disabledGroup" id="checkbox-disabledGroup3">Disabled checkbox option</auro-checkbox>
    <auro-checkbox value="disabled-value4" name="disabledGroup" id="checkbox-disabledGroup4">Disabled checkbox option</auro-checkbox>
  </auro-checkbox-group>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceDisabled.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearanceDisabled.html -->
  <auro-checkbox-group appearance="inverse" disabled>
    <span slot="legend">Form label goes here</span>
    <auro-checkbox value="disabled-value1" name="disabledGroup" id="checkbox-disabledGroup1">Disabled checkbox option</auro-checkbox>
    <auro-checkbox value="disabled-value2" name="disabledGroup" id="checkbox-disabledGroup2" checked>Disabled checkbox option</auro-checkbox>
    <auro-checkbox value="disabled-value3" name="disabledGroup" id="checkbox-disabledGroup3">Disabled checkbox option</auro-checkbox>
    <auro-checkbox value="disabled-value4" name="disabledGroup" id="checkbox-disabledGroup4">Disabled checkbox option</auro-checkbox>
  </auro-checkbox-group>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/disabledGroup.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/disabledGroup.html -->

```html
<auro-checkbox-group disabled>
  <span slot="legend">Form label goes here</span>
  <auro-checkbox value="disabled-value1" name="disabledGroup" id="checkbox-disabledGroup1">Disabled checkbox option</auro-checkbox>
  <auro-checkbox value="disabled-value2" name="disabledGroup" id="checkbox-disabledGroup2" checked>Disabled checkbox option</auro-checkbox>
  <auro-checkbox value="disabled-value3" name="disabledGroup" id="checkbox-disabledGroup3">Disabled checkbox option</auro-checkbox>
  <auro-checkbox value="disabled-value4" name="disabledGroup" id="checkbox-disabledGroup4">Disabled checkbox option</auro-checkbox>
</auro-checkbox-group>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceDisabled.html) -->
<!-- The below content is automatically added from ./../apiExamples/inverseAppearanceDisabled.html -->
<auro-checkbox-group appearance="inverse" disabled>
  <span slot="legend">Form label goes here</span>
  <auro-checkbox value="disabled-value1" name="disabledGroup" id="checkbox-disabledGroup1">Disabled checkbox option</auro-checkbox>
  <auro-checkbox value="disabled-value2" name="disabledGroup" id="checkbox-disabledGroup2" checked>Disabled checkbox option</auro-checkbox>
  <auro-checkbox value="disabled-value3" name="disabledGroup" id="checkbox-disabledGroup3">Disabled checkbox option</auro-checkbox>
  <auro-checkbox value="disabled-value4" name="disabledGroup" id="checkbox-disabledGroup4">Disabled checkbox option</auro-checkbox>
</auro-checkbox-group>
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Error

Use the `error` attribute to force an error state on the element.

#### Checkbox Group with Error

The `error` attribute used to set error state on the entire `<auro-checkbox-group>`. If using the `error` attribute on an `<auro-checkbox-group>`, a string with the error message needs to be passed along with the attribute.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/errorGroup.html) -->
  <!-- The below content is automatically added from ./../apiExamples/errorGroup.html -->
  <auro-checkbox-group error="custom error">
    <span slot="legend">Form label goes here</span>
    <auro-checkbox value="error-value1" name="error" id="checkbox-errorGroup1">Error checkbox option</auro-checkbox>
    <auro-checkbox value="error-value2" name="error" id="checkbox-errorGroup2">Error checkbox option</auro-checkbox>
    <auro-checkbox value="error-value3" name="error" id="checkbox-errorGroup3">Error checkbox option</auro-checkbox>
    <auro-checkbox value="error-value4" name="error" id="checkbox-errorGroup4" checked>Error checkbox option</auro-checkbox>
  </auro-checkbox-group>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceError.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearanceError.html -->
  <auro-checkbox-group appearance="inverse" error="custom error">
    <span slot="legend">Form label goes here</span>
    <auro-checkbox value="error-value1" name="error" id="checkbox-errorGroup1">Error checkbox option</auro-checkbox>
    <auro-checkbox value="error-value2" name="error" id="checkbox-errorGroup2">Error checkbox option</auro-checkbox>
    <auro-checkbox value="error-value3" name="error" id="checkbox-errorGroup3">Error checkbox option</auro-checkbox>
    <auro-checkbox value="error-value4" name="error" id="checkbox-errorGroup4" checked>Error checkbox option</auro-checkbox>
  </auro-checkbox-group>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/errorGroup.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/errorGroup.html -->

```html
<auro-checkbox-group error="custom error">
  <span slot="legend">Form label goes here</span>
  <auro-checkbox value="error-value1" name="error" id="checkbox-errorGroup1">Error checkbox option</auro-checkbox>
  <auro-checkbox value="error-value2" name="error" id="checkbox-errorGroup2">Error checkbox option</auro-checkbox>
  <auro-checkbox value="error-value3" name="error" id="checkbox-errorGroup3">Error checkbox option</auro-checkbox>
  <auro-checkbox value="error-value4" name="error" id="checkbox-errorGroup4" checked>Error checkbox option</auro-checkbox>
</auro-checkbox-group>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceError.html) -->
<!-- The below content is automatically added from ./../apiExamples/inverseAppearanceError.html -->
<auro-checkbox-group appearance="inverse" error="custom error">
  <span slot="legend">Form label goes here</span>
  <auro-checkbox value="error-value1" name="error" id="checkbox-errorGroup1">Error checkbox option</auro-checkbox>
  <auro-checkbox value="error-value2" name="error" id="checkbox-errorGroup2">Error checkbox option</auro-checkbox>
  <auro-checkbox value="error-value3" name="error" id="checkbox-errorGroup3">Error checkbox option</auro-checkbox>
  <auro-checkbox value="error-value4" name="error" id="checkbox-errorGroup4" checked>Error checkbox option</auro-checkbox>
</auro-checkbox-group>
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### Required Group

When present, the `required` attribute specifies that at least one or more `<auro-checkbox>` elements within the `<auro-checkbox-group>` must be checked.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/required.html) -->
  <!-- The below content is automatically added from ./../apiExamples/required.html -->
  <auro-checkbox-group required setCustomValidityValueMissing="Please select an option">
    <span slot="legend">Form label goes here</span>
    <auro-checkbox value="value1" name="required" id="checkbox-required1">Checkbox option</auro-checkbox>
    <auro-checkbox value="value2" name="required" id="checkbox-required2">Checkbox option</auro-checkbox>
    <auro-checkbox value="value3" name="required" id="checkbox-required3">Checkbox option</auro-checkbox>
    <auro-checkbox value="value4" name="required" id="checkbox-required4">Checkbox option</auro-checkbox>
  </auro-checkbox-group>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/required.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/required.html -->

```html
<auro-checkbox-group required setCustomValidityValueMissing="Please select an option">
  <span slot="legend">Form label goes here</span>
  <auro-checkbox value="value1" name="required" id="checkbox-required1">Checkbox option</auro-checkbox>
  <auro-checkbox value="value2" name="required" id="checkbox-required2">Checkbox option</auro-checkbox>
  <auro-checkbox value="value3" name="required" id="checkbox-required3">Checkbox option</auro-checkbox>
  <auro-checkbox value="value4" name="required" id="checkbox-required4">Checkbox option</auro-checkbox>
</auro-checkbox-group>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Horizontal Group

Using the `horizontal` attribute will render the checkbox options on a horizontal line.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/horizontal.html) -->
  <!-- The below content is automatically added from ./../apiExamples/horizontal.html -->
  <auro-checkbox-group horizontal>
    <span slot="legend">Form label goes here</span>
    <auro-checkbox value="yes" name="horizontal" id="checkbox-horizontal1">Yes</auro-checkbox>
    <auro-checkbox value="no" name="horizontal" id="checkbox-horizontal2">No</auro-checkbox>
    <auro-checkbox value="maybe" name="horizontal" id="checkbox-horizontal3">Maybe</auro-checkbox>
  </auro-checkbox-group>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/horizontal.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/horizontal.html -->

```html
<auro-checkbox-group horizontal>
  <span slot="legend">Form label goes here</span>
  <auro-checkbox value="yes" name="horizontal" id="checkbox-horizontal1">Yes</auro-checkbox>
  <auro-checkbox value="no" name="horizontal" id="checkbox-horizontal2">No</auro-checkbox>
  <auro-checkbox value="maybe" name="horizontal" id="checkbox-horizontal3">Maybe</auro-checkbox>
</auro-checkbox-group>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Horizontal Group Limitation

Using the `horizontal` attribute has a limit of 3 options. Beyond three, options will be listed in vertically.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/horizontalLimit.html) -->
  <!-- The below content is automatically added from ./../apiExamples/horizontalLimit.html -->
  <auro-checkbox-group horizontal>
    <span slot="legend">Form label goes here</span>
    <auro-checkbox value="yes" name="horizontalLimit" id="checkbox-horizontalLimit1">Yes</auro-checkbox>
    <auro-checkbox value="no" name="horizontalLimit" id="checkbox-horizontalLimit2">No</auro-checkbox>
    <auro-checkbox value="maybe" name="horizontalLimit" id="checkbox-horizontalLimit3">Maybe</auro-checkbox>
    <auro-checkbox value="not sure" name="horizontalLimit" id="checkbox-horizontalLimit4">Not Sure</auro-checkbox>
  </auro-checkbox-group>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/horizontalLimit.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/horizontalLimit.html -->

```html
<auro-checkbox-group horizontal>
  <span slot="legend">Form label goes here</span>
  <auro-checkbox value="yes" name="horizontalLimit" id="checkbox-horizontalLimit1">Yes</auro-checkbox>
  <auro-checkbox value="no" name="horizontalLimit" id="checkbox-horizontalLimit2">No</auro-checkbox>
  <auro-checkbox value="maybe" name="horizontalLimit" id="checkbox-horizontalLimit3">Maybe</auro-checkbox>
  <auro-checkbox value="not sure" name="horizontalLimit" id="checkbox-horizontalLimit4">Not Sure</auro-checkbox>
</auro-checkbox-group>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>
