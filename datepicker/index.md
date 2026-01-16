# Datepicker

<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../docs/partials/description.md) -->
<!-- The below content is automatically added from ./../docs/partials/description.md -->
The `<auro-datepicker>` element allows users to select a date, or a pair of dates identifying a range, either with text input or by making a section in a calendar. The `<auro-datepicker>` element is the combination of [auro-dropdown](http://auro.alaskaair.com/components/auro/dropdown), [auro-input](http://auro.alaskaair.com/components/auro/input), and Auro's extension of [wc-range-datepicker](https://www.npmjs.com/package/wc-range-datepicker).
<!-- AURO-GENERATED-CONTENT:END -->

## auro-datepicker use cases

<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../docs/partials/useCases.md) -->
<!-- The below content is automatically added from ./../docs/partials/useCases.md -->
The `<auro-datepicker>` element should be used in situations where users may:

* select a single date
* select a pair of dates which identify a calendar range
<!-- AURO-GENERATED-CONTENT:END -->

## Examples

### Snowflake layout

#### Single date
<div class="exampleWrapper--ondark" style="width: 306px">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/snowflake/inverseAppearance.html) -->
  <!-- The below content is automatically added from ./../apiExamples/snowflake/inverseAppearance.html -->
  <auro-datepicker layout="snowflake" shape="snowflake" appearance="inverse" placeholder="MM/DD/YYYY">
    <span slot="ariaLabel.bib.close">Close Calendar</span>
    <span slot="label">Date</span>
    <span slot="bib.fullscreen.headline">Datepicker Headline</span>
    <span slot="fromLabel">Choose a date</span>
    <span slot="bib.fullscreen.dateLabel">Choose a date</span>
  </auro-datepicker>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/snowflake/inverseAppearance.html) -->
  <!-- The below content is automatically added from ./../apiExamples/snowflake/inverseAppearance.html -->
  <auro-datepicker layout="snowflake" shape="snowflake" appearance="inverse" placeholder="MM/DD/YYYY">
    <span slot="ariaLabel.bib.close">Close Calendar</span>
    <span slot="label">Date</span>
    <span slot="bib.fullscreen.headline">Datepicker Headline</span>
    <span slot="fromLabel">Choose a date</span>
    <span slot="bib.fullscreen.dateLabel">Choose a date</span>
  </auro-datepicker>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/snowflake/inverseAppearance.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/snowflake/inverseAppearance.html -->

```html
<auro-datepicker layout="snowflake" shape="snowflake" appearance="inverse" placeholder="MM/DD/YYYY">
  <span slot="ariaLabel.bib.close">Close Calendar</span>
  <span slot="label">Date</span>
  <span slot="bib.fullscreen.headline">Datepicker Headline</span>
  <span slot="fromLabel">Choose a date</span>
  <span slot="bib.fullscreen.dateLabel">Choose a date</span>
</auro-datepicker>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### Range
<div class="exampleWrapper--ondark" style="width: 306px">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/snowflake/inverseAppearance-range.html) -->
  <!-- The below content is automatically added from ./../apiExamples/snowflake/inverseAppearance-range.html -->
  <auro-datepicker range layout="snowflake" shape="snowflake" appearance="inverse" placeholder="MM/DD/YYYY" dvInputOnly>
    <span slot="ariaLabel.bib.close">Close Calendar</span>
    <span slot="label">Dates</span>
    <span slot="bib.fullscreen.headline">Datepicker Headline</span>
    <span slot="fromLabel">Choose a date</span>
    <span slot="bib.fullscreen.dateLabel">Choose a date</span>
  </auro-datepicker>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/snowflake/inverseAppearance-range.html) -->
  <!-- The below content is automatically added from ./../apiExamples/snowflake/inverseAppearance-range.html -->
  <auro-datepicker range layout="snowflake" shape="snowflake" appearance="inverse" placeholder="MM/DD/YYYY" dvInputOnly>
    <span slot="ariaLabel.bib.close">Close Calendar</span>
    <span slot="label">Dates</span>
    <span slot="bib.fullscreen.headline">Datepicker Headline</span>
    <span slot="fromLabel">Choose a date</span>
    <span slot="bib.fullscreen.dateLabel">Choose a date</span>
  </auro-datepicker>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/snowflake/inverseAppearance-range.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/snowflake/inverseAppearance-range.html -->

```html
<auro-datepicker range layout="snowflake" shape="snowflake" appearance="inverse" placeholder="MM/DD/YYYY" dvInputOnly>
  <span slot="ariaLabel.bib.close">Close Calendar</span>
  <span slot="label">Dates</span>
  <span slot="bib.fullscreen.headline">Datepicker Headline</span>
  <span slot="fromLabel">Choose a date</span>
  <span slot="bib.fullscreen.dateLabel">Choose a date</span>
</auro-datepicker>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Basic

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/basic.html) -->
  <!-- The below content is automatically added from ./../apiExamples/basic.html -->
  <auro-datepicker required="">
    <span slot="ariaLabel.bib.close">Close Calendar</span>
    <span slot="bib.fullscreen.headline">Datepicker Headline</span>
    <span slot="fromLabel">Choose a date</span>
    <span slot="bib.fullscreen.dateLabel">Choose a date</span>
  </auro-datepicker>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearance.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearance.html -->
  <auro-datepicker appearance="inverse">
    <span slot="ariaLabel.bib.close">Close Calendar</span>
    <span slot="bib.fullscreen.headline">Datepicker Headline</span>
    <span slot="fromLabel">Choose a date</span>
    <span slot="bib.fullscreen.dateLabel">Choose a date</span>
  </auro-datepicker>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/basic.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/basic.html -->

```html
<auro-datepicker required="">
  <span slot="ariaLabel.bib.close">Close Calendar</span>
  <span slot="bib.fullscreen.headline">Datepicker Headline</span>
  <span slot="fromLabel">Choose a date</span>
  <span slot="bib.fullscreen.dateLabel">Choose a date</span>
</auro-datepicker>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearance.html) -->
<!-- The below content is automatically added from ./../apiExamples/inverseAppearance.html -->
<auro-datepicker appearance="inverse">
  <span slot="ariaLabel.bib.close">Close Calendar</span>
  <span slot="bib.fullscreen.headline">Datepicker Headline</span>
  <span slot="fromLabel">Choose a date</span>
  <span slot="bib.fullscreen.dateLabel">Choose a date</span>
</auro-datepicker>
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Range

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/basicRange.html) -->
  <!-- The below content is automatically added from ./../apiExamples/basicRange.html -->
  <auro-datepicker range minDate="07/08/2025">
    <span slot="ariaLabel.bib.close">Close Calendar</span>
    <span slot="bib.fullscreen.headline">Datepicker Range Headline</span>
    <span slot="fromLabel">Departure</span>
    <span slot="toLabel">Return</span>
    <span slot="bib.fullscreen.dateLabel">Roundtrip</span>
  </auro-datepicker>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceRange.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearanceRange.html -->
  <auro-datepicker appearance="inverse" range>
    <span slot="bib.fullscreen.headline">Datepicker Range Headline</span>
    <span slot="fromLabel">Departure</span>
    <span slot="toLabel">Return</span>
    <span slot="bib.fullscreen.dateLabel">Roundtrip</span>
  </auro-datepicker>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/basicRange.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/basicRange.html -->

```html
<auro-datepicker range minDate="07/08/2025">
  <span slot="ariaLabel.bib.close">Close Calendar</span>
  <span slot="bib.fullscreen.headline">Datepicker Range Headline</span>
  <span slot="fromLabel">Departure</span>
  <span slot="toLabel">Return</span>
  <span slot="bib.fullscreen.dateLabel">Roundtrip</span>
</auro-datepicker>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceRange.html) -->
<!-- The below content is automatically added from ./../apiExamples/inverseAppearanceRange.html -->
<auro-datepicker appearance="inverse" range>
  <span slot="bib.fullscreen.headline">Datepicker Range Headline</span>
  <span slot="fromLabel">Departure</span>
  <span slot="toLabel">Return</span>
  <span slot="bib.fullscreen.dateLabel">Roundtrip</span>
</auro-datepicker>
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>
