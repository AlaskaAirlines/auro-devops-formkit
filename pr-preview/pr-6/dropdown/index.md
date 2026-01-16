<!--
The index.md file is a compiled document. No edits should be made directly to this file.

index.md is created by running `npm run build:markdownDocs`.

This file is generated based on a template fetched from `./docs/partials/index.md`
-->

# Dropdown

<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../docs/partials/description.md) -->
<!-- The below content is automatically added from ./../docs/partials/description.md -->
The `auro-dropdown` component is a trigger and dropdown element combination intended to be used with dropdown content that is interactive. `auro-dropdown` is content agnostic and any valid HTML can be placed in either the trigger or the dropdown.

_Note: if the dropdown content in your implementation is not interactive (e.g. a tooltip) [auro-popover](http://auro.alaskaair.com/components/auro/popover) may better serve your needs._
<!-- AURO-GENERATED-CONTENT:END -->

## Dropdown use cases

<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../docs/partials/useCases.md) -->
<!-- The below content is automatically added from ./../docs/partials/useCases.md -->
The `auro-dropdown` element should be used in situations where users may:

* interact with an element to get clarification on content offering
* provide definition to iconic imagery
* when interactive help is required
<!-- AURO-GENERATED-CONTENT:END -->

## Accessibility support

To meet our accessibility requirement, all uses of `auro-dropdown` should have a valid label. See the following options.

1. Use the `label` content slot
1. Use `aria-label` to insert label content that will only be read by screen readers
1. Use `aria-labeledby` to append a description from another element on the page

Not including one of the above options will result in your UI being non-compliant with Alaska's accessibility policies.

## Layouts

### Classic

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/classic/basic.html) -->
  <!-- The below content is automatically added from ./../apiExamples/classic/basic.html -->
  <auro-dropdown id="classic" layout="classic" shape="classic" size="lg" chevron aria-label="Label content for screen reader">
    <div style="padding: var(--ds-size-150);">
      Lorem ipsum solar
      <br />
      <auro-button onclick="document.querySelector('#classic').hide()">
        Dismiss Dropdown
      </auro-button>
    </div>
    <span slot="helpText">
      Help text
    </span>
    <div slot="trigger">
      Trigger
    </div>
  </auro-dropdown>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/classic/basic.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/classic/basic.html -->

```html
<auro-dropdown id="classic" layout="classic" shape="classic" size="lg" chevron aria-label="Label content for screen reader">
  <div style="padding: var(--ds-size-150);">
    Lorem ipsum solar
    <br />
    <auro-button onclick="document.querySelector('#classic').hide()">
      Dismiss Dropdown
    </auro-button>
  </div>
  <span slot="helpText">
    Help text
  </span>
  <div slot="trigger">
    Trigger
  </div>
</auro-dropdown>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>
<div class="exampleWrapper--ondark">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/classic/basic-inverseAppearance.html) -->
  <!-- The below content is automatically added from ./../apiExamples/classic/basic-inverseAppearance.html -->
  <auro-dropdown appearance="inverse" layout="classic" shape="classic" size="lg" id="classicOnDark" chevron aria-label="Label content for screen reader">
    <div style="padding: var(--ds-size-150);">
      Lorem ipsum solar
      <br />
      <auro-button onclick="document.querySelector('#classicOnDark').hide()">
        Dismiss Dropdown
      </auro-button>
    </div>
    <span slot="helpText">
      Help text
    </span>
    <div slot="trigger">
      Trigger
    </div>
  </auro-dropdown>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/classic/basic-inverseAppearance.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/classic/basic-inverseAppearance.html -->

```html
<auro-dropdown appearance="inverse" layout="classic" shape="classic" size="lg" id="classicOnDark" chevron aria-label="Label content for screen reader">
  <div style="padding: var(--ds-size-150);">
    Lorem ipsum solar
    <br />
    <auro-button onclick="document.querySelector('#classicOnDark').hide()">
      Dismiss Dropdown
    </auro-button>
  </div>
  <span slot="helpText">
    Help text
  </span>
  <div slot="trigger">
    Trigger
  </div>
</auro-dropdown>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Emphasized

Only supports `appearance="inverse"`.

<div class="exampleWrapper--ondark">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/emphasized/basic.html) -->
  <!-- The below content is automatically added from ./../apiExamples/emphasized/basic.html -->
  <auro-dropdown aria-label="custom label" shape="pill" size="xl" layout="emphasized" style="width: 249px;" appearance="inverse">
    Lorem ipsum solar
    <div slot="trigger">
      Trigger
    </div>
    <span slot="helpText">
      Help text - Lorem ipsum solar lorem ipsum solar
    </span>
  </auro-dropdown>
  <auro-dropdown aria-label="custom label" shape="pill-left" size="xl" layout="emphasized" style="width: 249px;" appearance="inverse">
    Lorem ipsum solar
    <div slot="trigger">
      Trigger
    </div>
    <span slot="helpText">
      Help text - Lorem ipsum solar lorem ipsum solar
    </span>
  </auro-dropdown>
  <auro-dropdown aria-label="custom label" shape="pill-right" size="xl" layout="emphasized" style="width: 249px;" appearance="inverse">
    Lorem ipsum solar
    <div slot="trigger">
      Trigger
    </div>
    <span slot="helpText">
      Help text - Lorem ipsum solar lorem ipsum solar
    </span>
  </auro-dropdown>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/emphasized/basic.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/emphasized/basic.html -->

```html
<auro-dropdown aria-label="custom label" shape="pill" size="xl" layout="emphasized" style="width: 249px;" appearance="inverse">
  Lorem ipsum solar
  <div slot="trigger">
    Trigger
  </div>
  <span slot="helpText">
    Help text - Lorem ipsum solar lorem ipsum solar
  </span>
</auro-dropdown>
<auro-dropdown aria-label="custom label" shape="pill-left" size="xl" layout="emphasized" style="width: 249px;" appearance="inverse">
  Lorem ipsum solar
  <div slot="trigger">
    Trigger
  </div>
  <span slot="helpText">
    Help text - Lorem ipsum solar lorem ipsum solar
  </span>
</auro-dropdown>
<auro-dropdown aria-label="custom label" shape="pill-right" size="xl" layout="emphasized" style="width: 249px;" appearance="inverse">
  Lorem ipsum solar
  <div slot="trigger">
    Trigger
  </div>
  <span slot="helpText">
    Help text - Lorem ipsum solar lorem ipsum solar
  </span>
</auro-dropdown>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Snowflake

Only supports `appearance="inverse"`.

<div class="exampleWrapper--ondark">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/snowflake/basic.html) -->
  <!-- The below content is automatically added from ./../apiExamples/snowflake/basic.html -->
  <auro-dropdown aria-label="custom label" shape="snowflake" size="lg" layout="snowflake" style="width: 249px;" appearance="inverse">
    Lorem ipsum solar
    <div slot="trigger">
      Trigger
    </div>
    <span slot="helpText">
      Help text - Lorem ipsum solar lorem ipsum solar
    </span>
  </auro-dropdown>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/snowflake/basic.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/snowflake/basic.html -->

```html
<auro-dropdown aria-label="custom label" shape="snowflake" size="lg" layout="snowflake" style="width: 249px;" appearance="inverse">
  Lorem ipsum solar
  <div slot="trigger">
    Trigger
  </div>
  <span slot="helpText">
    Help text - Lorem ipsum solar lorem ipsum solar
  </span>
</auro-dropdown>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

## Triggering a fullscreen dropdown
This example shows how to set a dropdown fullscreen breakpoint attribute. Most consuming components use `sm` by default, but
dropdown supports `xs`, `sm`, `md`, `lg`, `xl` and `disabled`, with `disabled` ensuring that the dropdown will never be fullscreen.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/fullscreen.html) -->
  <!-- The below content is automatically added from ./../apiExamples/fullscreen.html -->
  <h3>Never fullscreen</h3>
  <auro-dropdown id="common-never-fullscreen" layout="classic" shape="classic" size="lg" aria-label="Label content for screen reader" fullscreenBreakpoint="disabled">
    <div style="padding: var(--ds-size-150);">
      Lorem ipsum solar
      <br />
      <auro-button onclick="document.querySelector('#common-never-fullscreen').hide()">
        Dismiss Dropdown
      </auro-button>
    </div>
    <span slot="helpText">
      Help text
    </span>
    <div slot="trigger">
      Trigger
    </div>
  </auro-dropdown>
  <h3>Always fullscreen</h3>
  <auro-dropdown id="common-always-fullscreen" layout="classic" shape="classic" size="lg" aria-label="Label content for screen reader" fullscreenBreakpoint="xl">
    <div style="padding: var(--ds-size-150);">
      Lorem ipsum solar
      <br />
      <auro-button onclick="document.querySelector('#common-always-fullscreen').hide()">
        Dismiss Dropdown
      </auro-button>
    </div>
    <span slot="helpText">
      Help text
    </span>
    <div slot="trigger">
      Trigger
    </div>
  </auro-dropdown>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/fullscreen.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/fullscreen.html -->

```html
<h3>Never fullscreen</h3>
<auro-dropdown id="common-never-fullscreen" layout="classic" shape="classic" size="lg" aria-label="Label content for screen reader" fullscreenBreakpoint="disabled">
  <div style="padding: var(--ds-size-150);">
    Lorem ipsum solar
    <br />
    <auro-button onclick="document.querySelector('#common-never-fullscreen').hide()">
      Dismiss Dropdown
    </auro-button>
  </div>
  <span slot="helpText">
    Help text
  </span>
  <div slot="trigger">
    Trigger
  </div>
</auro-dropdown>
<h3>Always fullscreen</h3>
<auro-dropdown id="common-always-fullscreen" layout="classic" shape="classic" size="lg" aria-label="Label content for screen reader" fullscreenBreakpoint="xl">
  <div style="padding: var(--ds-size-150);">
    Lorem ipsum solar
    <br />
    <auro-button onclick="document.querySelector('#common-always-fullscreen').hide()">
      Dismiss Dropdown
    </auro-button>
  </div>
  <span slot="helpText">
    Help text
  </span>
  <div slot="trigger">
    Trigger
  </div>
</auro-dropdown>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

## Supported standard and accessible interactions

The dropdown can be opened with the following actions:

1. Clicking/tapping on the trigger.
1. Tabbing to the trigger and using the `enter` or `spacebar` keys.
1. Programmatically via another control in the UI calling the `show()` method (see api).

The dropdown can be closed with the following actions:

1. Clicking anywhere in the view outside of the dropdown.
1. Using the `esc` key.
1. Programmatically via another control in the UI calling the `hide()` method (see api).
