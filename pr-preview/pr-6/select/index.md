<!--
The demo.md file is a compiled document. No edits should be made directly to this file.

demo.md is created by running `npm run build:markdownDocs`.

This file is generated based on a template fetched from `./docs/partials/demo.md`
-->

# Select

<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../docs/partials/description.md) -->
<!-- The below content is automatically added from ./../docs/partials/description.md -->
`<auro-select>` is a combination <auro-hyperlink href="https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_custom_elements">HTML custom element</auro-hyperlink> that consists of a pre-defined trigger element, `<auro-menu>` for the panel content. The `<auro-select>` element presents a menu of options. The options within the menu are represented by `<auro-menu>` and `<auro-menuoption>` elements. You can pre-select options for the user with the `selected` attribute as part of the `<auro-menuoption>` API.
<!-- AURO-GENERATED-CONTENT:END -->

## Default example

A baseline `<auro-select>` using `<auro-menu>` and `<auro-menuoption>` elements. Notice a default `Please select option` placeholder in the trigger.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/basic.html) -->
  <!-- The below content is automatically added from ./../apiExamples/basic.html -->
  <auro-select>
    <span slot="ariaLabel.bib.close">Close Popup</span>
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Select Example</span>
    <auro-menu>
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearance.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearance.html -->
  <auro-select appearance="inverse">
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Select Example</span>
    <auro-menu>
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/basic.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/basic.html -->

```html
<auro-select>
  <span slot="ariaLabel.bib.close">Close Popup</span>
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Select Example</span>
  <auro-menu>
    <auro-menuoption value="stops">Stops</auro-menuoption>
    <auro-menuoption value="price">Price</auro-menuoption>
    <auro-menuoption value="duration">Duration</auro-menuoption>
    <auro-menuoption value="departure">Departure</auro-menuoption>
    <auro-menuoption value="arrival">Arrival</auro-menuoption>
    <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
  </auro-menu>
</auro-select>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearance.html) -->
<!-- The below content is automatically added from ./../apiExamples/inverseAppearance.html -->
<auro-select appearance="inverse">
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Select Example</span>
  <auro-menu>
    <auro-menuoption value="stops">Stops</auro-menuoption>
    <auro-menuoption value="price">Price</auro-menuoption>
    <auro-menuoption value="duration">Duration</auro-menuoption>
    <auro-menuoption value="departure">Departure</auro-menuoption>
    <auro-menuoption value="arrival">Arrival</auro-menuoption>
    <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
  </auro-menu>
</auro-select>
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

## Shape | Size | Layout Support

The `auro-select` component supports the `shape`, `size` and `layout` feature set. The component defaults to the `classic` shape and layout.

### Supported Combinations

#### Classic Layout (Legacy)

The `classic` layout is default for `auro-select`. No customization is needed to achieve this look.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/basic.html) -->
  <!-- The below content is automatically added from ./../apiExamples/basic.html -->
  <auro-select>
    <span slot="ariaLabel.bib.close">Close Popup</span>
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Select Example</span>
    <auro-menu>
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/basic.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/basic.html -->

```html
<auro-select>
  <span slot="ariaLabel.bib.close">Close Popup</span>
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Select Example</span>
  <auro-menu>
    <auro-menuoption value="stops">Stops</auro-menuoption>
    <auro-menuoption value="price">Price</auro-menuoption>
    <auro-menuoption value="duration">Duration</auro-menuoption>
    <auro-menuoption value="departure">Departure</auro-menuoption>
    <auro-menuoption value="arrival">Arrival</auro-menuoption>
    <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
  </auro-menu>
</auro-select>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### Emphasized Layout

The `emphasized` layout only supports `appearance="inverse"` use.

The `emphasized` layout supports the following shapes:
- `pill`
- `pill-left`
- `pill-right`

The `emphasized` layout supports the following sizes:
- `xl`

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/emphasized/basic.html) -->
  <!-- The below content is automatically added from ./../apiExamples/emphasized/basic.html -->
  <div style="display: flex; flex-direction: row; gap: 10px;">
    <auro-select layout="emphasized" shape="pill" size="xl" value="flights" forceDisplayValue style="display:inline-block;">
      <span slot="ariaLabel.bib.close">Close Popup</span>
      <span slot="label">Select Example</span>
      <auro-menu nocheckmark>
        <auro-menuoption value="flights">
          <auro-icon category="terminal" name="plane-diag-stroke" customcolor></auro-icon> Flights
          <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="terminal" name="plane-diag-fill" customcolor></auro-icon>
        </auro-menuoption>
        <auro-menuoption value="cars">
          <auro-icon category="destination" name="car-rental-stroke" customcolor></auro-icon> Cars
          <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="destination" name="car-rental-stroke" customcolor></auro-icon>
        </auro-menuoption>
        <auro-menuoption value="hotels">
          <auro-icon category="destination" name="hotel-stroke" customcolor></auro-icon> Hotels
          <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="destination" name="hotel-filled" customcolor></auro-icon>
        </auro-menuoption>
        <auro-menuoption value="packages">
          <auro-icon category="shop" name="gift-stroke" customcolor></auro-icon> Packages
          <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="shop" name="gift-filled" customcolor></auro-icon>
        </auro-menuoption>
        <auro-menuoption value="cruises">
          <auro-icon category="in-flight" name="boarding" customcolor></auro-icon> Cruises
          <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="in-flight" name="boarding" customcolor></auro-icon>
        </auro-menuoption>
      </auro-menu>
    </auro-select>
    <auro-select layout="emphasized" shape="pill" size="xl" value="flights" style="display:inline-block;">
      <span slot="label">Select Example</span>
      <auro-menu nocheckmark>
        <auro-menuoption value="flights">
          <auro-icon category="terminal" name="plane-diag-stroke" customcolor></auro-icon> Flights
          <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="terminal" name="plane-diag-fill" customcolor></auro-icon>
        </auro-menuoption>
        <auro-menuoption value="cars">
          <auro-icon category="destination" name="car-rental-stroke" customcolor></auro-icon> Cars
          <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="destination" name="car-rental-stroke" customcolor></auro-icon>
        </auro-menuoption>
        <auro-menuoption value="hotels">
          <auro-icon category="destination" name="hotel-stroke" customcolor></auro-icon> Hotels
          <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="destination" name="hotel-filled" customcolor></auro-icon>
        </auro-menuoption>
        <auro-menuoption value="packages">
          <auro-icon category="shop" name="gift-stroke" customcolor></auro-icon> Packages
          <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="shop" name="gift-filled" customcolor></auro-icon>
        </auro-menuoption>
        <auro-menuoption value="cruises">
          <auro-icon category="in-flight" name="boarding" customcolor></auro-icon> Cruises
          <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="in-flight" name="boarding" customcolor></auro-icon>
        </auro-menuoption>
      </auro-menu>
    </auro-select>
    <auro-select layout="emphasized" shape="pill" size="xl" value="flights" required style="display:inline-block;">
      <span slot="label">Select Example</span>
      <span slot="helpText">no displayValue in menuoptions</span>
      <auro-menu nocheckmark>
        <auro-menuoption value="flights">
          <auro-icon category="terminal" name="plane-diag-stroke" customcolor></auro-icon> Flights
        </auro-menuoption>
        <auro-menuoption value="cars">
          <auro-icon category="destination" name="car-rental-stroke" customcolor></auro-icon> Cars
        </auro-menuoption>
        <auro-menuoption value="hotels">
          <auro-icon category="destination" name="hotel-stroke" customcolor></auro-icon> Hotels
        </auro-menuoption>
        <auro-menuoption value="packages">
          <auro-icon category="shop" name="gift-stroke" customcolor></auro-icon> Packages
        </auro-menuoption>
        <auro-menuoption value="cruises">
          <auro-icon category="in-flight" name="boarding" customcolor></auro-icon> Cruises
        </auro-menuoption>
      </auro-menu>
    </auro-select>
  </div>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/emphasized/basic.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/emphasized/basic.html -->

```html
<div style="display: flex; flex-direction: row; gap: 10px;">
  <auro-select layout="emphasized" shape="pill" size="xl" value="flights" forceDisplayValue style="display:inline-block;">
    <span slot="ariaLabel.bib.close">Close Popup</span>
    <span slot="label">Select Example</span>
    <auro-menu nocheckmark>
      <auro-menuoption value="flights">
        <auro-icon category="terminal" name="plane-diag-stroke" customcolor></auro-icon> Flights
        <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="terminal" name="plane-diag-fill" customcolor></auro-icon>
      </auro-menuoption>
      <auro-menuoption value="cars">
        <auro-icon category="destination" name="car-rental-stroke" customcolor></auro-icon> Cars
        <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="destination" name="car-rental-stroke" customcolor></auro-icon>
      </auro-menuoption>
      <auro-menuoption value="hotels">
        <auro-icon category="destination" name="hotel-stroke" customcolor></auro-icon> Hotels
        <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="destination" name="hotel-filled" customcolor></auro-icon>
      </auro-menuoption>
      <auro-menuoption value="packages">
        <auro-icon category="shop" name="gift-stroke" customcolor></auro-icon> Packages
        <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="shop" name="gift-filled" customcolor></auro-icon>
      </auro-menuoption>
      <auro-menuoption value="cruises">
        <auro-icon category="in-flight" name="boarding" customcolor></auro-icon> Cruises
        <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="in-flight" name="boarding" customcolor></auro-icon>
      </auro-menuoption>
    </auro-menu>
  </auro-select>
  <auro-select layout="emphasized" shape="pill" size="xl" value="flights" style="display:inline-block;">
    <span slot="label">Select Example</span>
    <auro-menu nocheckmark>
      <auro-menuoption value="flights">
        <auro-icon category="terminal" name="plane-diag-stroke" customcolor></auro-icon> Flights
        <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="terminal" name="plane-diag-fill" customcolor></auro-icon>
      </auro-menuoption>
      <auro-menuoption value="cars">
        <auro-icon category="destination" name="car-rental-stroke" customcolor></auro-icon> Cars
        <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="destination" name="car-rental-stroke" customcolor></auro-icon>
      </auro-menuoption>
      <auro-menuoption value="hotels">
        <auro-icon category="destination" name="hotel-stroke" customcolor></auro-icon> Hotels
        <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="destination" name="hotel-filled" customcolor></auro-icon>
      </auro-menuoption>
      <auro-menuoption value="packages">
        <auro-icon category="shop" name="gift-stroke" customcolor></auro-icon> Packages
        <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="shop" name="gift-filled" customcolor></auro-icon>
      </auro-menuoption>
      <auro-menuoption value="cruises">
        <auro-icon category="in-flight" name="boarding" customcolor></auro-icon> Cruises
        <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="in-flight" name="boarding" customcolor></auro-icon>
      </auro-menuoption>
    </auro-menu>
  </auro-select>
  <auro-select layout="emphasized" shape="pill" size="xl" value="flights" required style="display:inline-block;">
    <span slot="label">Select Example</span>
    <span slot="helpText">no displayValue in menuoptions</span>
    <auro-menu nocheckmark>
      <auro-menuoption value="flights">
        <auro-icon category="terminal" name="plane-diag-stroke" customcolor></auro-icon> Flights
      </auro-menuoption>
      <auro-menuoption value="cars">
        <auro-icon category="destination" name="car-rental-stroke" customcolor></auro-icon> Cars
      </auro-menuoption>
      <auro-menuoption value="hotels">
        <auro-icon category="destination" name="hotel-stroke" customcolor></auro-icon> Hotels
      </auro-menuoption>
      <auro-menuoption value="packages">
        <auro-icon category="shop" name="gift-stroke" customcolor></auro-icon> Packages
      </auro-menuoption>
      <auro-menuoption value="cruises">
        <auro-icon category="in-flight" name="boarding" customcolor></auro-icon> Cruises
      </auro-menuoption>
    </auro-menu>
  </auro-select>
</div>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### Snowflake Layout

The `snowflake` layout is a unique, one off layout that does not follow the normal pattern. There is only one way to use snowflake as shown in the following example.

<div class="exampleWrapper--ondark">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/snowflake/basic-inverseAppearance.html) -->
  <!-- The below content is automatically added from ./../apiExamples/snowflake/basic-inverseAppearance.html -->
  <auro-select layout="snowflake" shape="snowflake" appearance="inverse" required style="width:300px;">
    <span slot="ariaLabel.bib.close">Close Popup</span>
    <span slot="label">Label</span>
    <span slot="helpText">Help Text</span>
    <auro-menu nocheckmark>
      <auro-menuoption value="flights">
        <auro-icon category="terminal" name="plane-diag-stroke" customColor></auro-icon> Flights
      </auro-menuoption>
      <auro-menuoption value="cars">
        <auro-icon category="destination" name="car-rental-stroke" customColor></auro-icon> Cars
      </auro-menuoption>
      <auro-menuoption value="hotels">
        <auro-icon category="destination" name="hotel-stroke" customColor></auro-icon> Hotels
      </auro-menuoption>
      <auro-menuoption value="packages">
        <auro-icon category="shop" name="gift-stroke" customColor></auro-icon> Packages
      </auro-menuoption>
      <auro-menuoption value="cruises">
        <auro-icon category="in-flight" name="boarding" customColor></auro-icon> Cruises
      </auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/snowflake/basic-inverseAppearance.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/snowflake/basic-inverseAppearance.html -->

```html
<auro-select layout="snowflake" shape="snowflake" appearance="inverse" required style="width:300px;">
  <span slot="ariaLabel.bib.close">Close Popup</span>
  <span slot="label">Label</span>
  <span slot="helpText">Help Text</span>
  <auro-menu nocheckmark>
    <auro-menuoption value="flights">
      <auro-icon category="terminal" name="plane-diag-stroke" customColor></auro-icon> Flights
    </auro-menuoption>
    <auro-menuoption value="cars">
      <auro-icon category="destination" name="car-rental-stroke" customColor></auro-icon> Cars
    </auro-menuoption>
    <auro-menuoption value="hotels">
      <auro-icon category="destination" name="hotel-stroke" customColor></auro-icon> Hotels
    </auro-menuoption>
    <auro-menuoption value="packages">
      <auro-icon category="shop" name="gift-stroke" customColor></auro-icon> Packages
    </auro-menuoption>
    <auro-menuoption value="cruises">
      <auro-icon category="in-flight" name="boarding" customColor></auro-icon> Cruises
    </auro-menuoption>
  </auro-menu>
</auro-select>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

## Custom Value Display

The `auro-select` supports the new formkit feature set enabling customized content displayed when a value is selected.

e.g. You may have a menu option that reads "SeaTac International Airport". However, when that option is selected, you would like the value displayed in the auro-select to just be the airport code "SEA".

The custom display value content is inserted using `slot="displayValue"` on each menu option. The `auro-select` component does not style or restrict the slotted content. It is the responsibility of the implementor to insure the content fits within the auro-select container and is styled appropriately.

The following example demonstrates menu options with an icon and text. When selected, the auro-select renders an icon with no text.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/emphasized/constantDisplayValue.html) -->
  <!-- The below content is automatically added from ./../apiExamples/emphasized/constantDisplayValue.html -->
  <auro-select layout="emphasized" shape="pill" size="xl" value="flights" forceDisplayValue style="display:inline-block;">
    <span slot="label">Select Example</span>
    <auro-menu nocheckmark>
      <auro-menuoption value="flights">
        <auro-icon category="terminal" name="plane-diag-stroke" customcolor></auro-icon> Flights
        <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="terminal" name="plane-diag-fill" customcolor></auro-icon>
      </auro-menuoption>
      <auro-menuoption value="cars">
        <auro-icon category="destination" name="car-rental-stroke" customcolor></auro-icon> Cars
        <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="destination" name="car-rental-stroke" customcolor></auro-icon>
      </auro-menuoption>
      <auro-menuoption value="hotels">
        <auro-icon category="destination" name="hotel-stroke" customcolor></auro-icon> Hotels
        <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="destination" name="hotel-filled" customcolor></auro-icon>
      </auro-menuoption>
      <auro-menuoption value="packages">
        <auro-icon category="shop" name="gift-stroke" customcolor></auro-icon> Packages
        <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="shop" name="gift-filled" customcolor></auro-icon>
      </auro-menuoption>
      <auro-menuoption value="cruises">
        <auro-icon category="in-flight" name="boarding" customcolor></auro-icon> Cruises
        <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="in-flight" name="boarding" customcolor></auro-icon>
      </auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/emphasized/constantDisplayValue.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/emphasized/constantDisplayValue.html -->

```html
<auro-select layout="emphasized" shape="pill" size="xl" value="flights" forceDisplayValue style="display:inline-block;">
  <span slot="label">Select Example</span>
  <auro-menu nocheckmark>
    <auro-menuoption value="flights">
      <auro-icon category="terminal" name="plane-diag-stroke" customcolor></auro-icon> Flights
      <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="terminal" name="plane-diag-fill" customcolor></auro-icon>
    </auro-menuoption>
    <auro-menuoption value="cars">
      <auro-icon category="destination" name="car-rental-stroke" customcolor></auro-icon> Cars
      <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="destination" name="car-rental-stroke" customcolor></auro-icon>
    </auro-menuoption>
    <auro-menuoption value="hotels">
      <auro-icon category="destination" name="hotel-stroke" customcolor></auro-icon> Hotels
      <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="destination" name="hotel-filled" customcolor></auro-icon>
    </auro-menuoption>
    <auro-menuoption value="packages">
      <auro-icon category="shop" name="gift-stroke" customcolor></auro-icon> Packages
      <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="shop" name="gift-filled" customcolor></auro-icon>
    </auro-menuoption>
    <auro-menuoption value="cruises">
      <auro-icon category="in-flight" name="boarding" customcolor></auro-icon> Cruises
      <auro-icon style="--ds-auro-icon-size: 40px;" slot="displayValue" category="in-flight" name="boarding" customcolor></auro-icon>
    </auro-menuoption>
  </auro-menu>
</auro-select>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

## placeholder

Use the `placeholder` slot to inject a custom placeholder option with the select element.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/customPlaceholder.html) -->
  <!-- The below content is automatically added from ./../apiExamples/customPlaceholder.html -->
  <auro-select placeholder="Please select your preferred option">
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Label</span>
    <auro-menu>
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/customPlaceholder.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/customPlaceholder.html -->

```html
<auro-select placeholder="Please select your preferred option">
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Label</span>
  <auro-menu>
    <auro-menuoption value="stops">Stops</auro-menuoption>
    <auro-menuoption value="price">Price</auro-menuoption>
    <auro-menuoption value="duration">Duration</auro-menuoption>
    <auro-menuoption value="departure">Departure</auro-menuoption>
    <auro-menuoption value="arrival">Arrival</auro-menuoption>
    <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
  </auro-menu>
</auro-select>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

## Label, placeholder and help text slots

The following example illustrates the use of the `label`, `placeholder` and `helptext` slots for additional placement of content around the select menu.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/slots.html) -->
  <!-- The below content is automatically added from ./../apiExamples/slots.html -->
  <auro-select placeholder="Placeholder Text">
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Label</span>
    <span slot="helpText">Help Text</span>
    <auro-menu>
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/slots.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/slots.html -->

```html
<auro-select placeholder="Placeholder Text">
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Label</span>
  <span slot="helpText">Help Text</span>
  <auro-menu>
    <auro-menuoption value="stops">Stops</auro-menuoption>
    <auro-menuoption value="price">Price</auro-menuoption>
    <auro-menuoption value="duration">Duration</auro-menuoption>
    <auro-menuoption value="departure">Departure</auro-menuoption>
    <auro-menuoption value="arrival">Arrival</auro-menuoption>
    <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
  </auro-menu>
</auro-select>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

## Autofill/Autocomplete Support

Use the `autocomplete` attribute to let browser's know what information to use to fill out the form.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/autocomplete.html) -->
  <!-- The below content is automatically added from ./../apiExamples/autocomplete.html -->
  <div class="autofill-example-form">
    <div class="input-row">
      <auro-input autocomplete="given-name">
        <span slot="label">First Name</span>
        <span slot="bib.fullscreen.headline">First Name</span>
      </auro-input>
      <auro-input autocomplete="family-name">
        <span slot="label">Last Name</span>
        <span slot="bib.fullscreen.headline">Last Name</span>
      </auro-input>
    </div>
    <div class="input-row">
      <auro-input autocomplete="address-line1">
        <span slot="label">Street Address</span>
        <span slot="bib.fullscreen.headline">Street Address</span>
      </auro-input>
      <auro-input autocomplete="address-level2">
        <span slot="label">City</span>
        <span slot="bib.fullscreen.headline">City</span>
      </auro-input>
      <auro-select autocomplete="address-level1">
        <span slot="bib.fullscreen.headline">Select Your State</span>
        <span slot="label">Select Your State</span>
        <auro-menu>
          <auro-menuoption value="AL">Alabama</auro-menuoption>
          <auro-menuoption value="AK">Alaska</auro-menuoption>
          <auro-menuoption value="AZ">Arizona</auro-menuoption>
          <auro-menuoption value="AR">Arkansas</auro-menuoption>
          <auro-menuoption value="CA">California</auro-menuoption>
          <auro-menuoption value="CO">Colorado</auro-menuoption>
          <auro-menuoption value="CT">Connecticut</auro-menuoption>
          <auro-menuoption value="DE">Delaware</auro-menuoption>
          <auro-menuoption value="DC">District of Columbia</auro-menuoption>
          <auro-menuoption value="FL">Florida</auro-menuoption>
          <auro-menuoption value="GA">Georgia</auro-menuoption>
          <auro-menuoption value="HI">Hawaii</auro-menuoption>
          <auro-menuoption value="ID">Idaho</auro-menuoption>
          <auro-menuoption value="IL">Illinois</auro-menuoption>
          <auro-menuoption value="IN">Indiana</auro-menuoption>
          <auro-menuoption value="IA">Iowa</auro-menuoption>
          <auro-menuoption value="KS">Kansas</auro-menuoption>
          <auro-menuoption value="KY">Kentucky</auro-menuoption>
          <auro-menuoption value="LA">Louisiana</auro-menuoption>
          <auro-menuoption value="ME">Maine</auro-menuoption>
          <auro-menuoption value="MD">Maryland</auro-menuoption>
          <auro-menuoption value="MA">Massachusetts</auro-menuoption>
          <auro-menuoption value="MI">Michigan</auro-menuoption>
          <auro-menuoption value="MN">Minnesota</auro-menuoption>
          <auro-menuoption value="MS">Mississippi</auro-menuoption>
          <auro-menuoption value="MO">Missouri</auro-menuoption>
          <auro-menuoption value="MT">Montana</auro-menuoption>
          <auro-menuoption value="NE">Nebraska</auro-menuoption>
          <auro-menuoption value="NV">Nevada</auro-menuoption>
          <auro-menuoption value="NH">New Hampshire</auro-menuoption>
          <auro-menuoption value="NJ">New Jersey</auro-menuoption>
          <auro-menuoption value="NM">New Mexico</auro-menuoption>
          <auro-menuoption value="NY">New York</auro-menuoption>
          <auro-menuoption value="NC">North Carolina</auro-menuoption>
          <auro-menuoption value="ND">North Dakota</auro-menuoption>
          <auro-menuoption value="OH">Ohio</auro-menuoption>
          <auro-menuoption value="OK">Oklahoma</auro-menuoption>
          <auro-menuoption value="OR">Oregon</auro-menuoption>
          <auro-menuoption value="PA">Pennsylvania</auro-menuoption>
          <auro-menuoption value="RI">Rhode Island</auro-menuoption>
          <auro-menuoption value="SC">South Carolina</auro-menuoption>
          <auro-menuoption value="SD">South Dakota</auro-menuoption>
          <auro-menuoption value="TN">Tennessee</auro-menuoption>
          <auro-menuoption value="TX">Texas</auro-menuoption>
          <auro-menuoption value="UT">Utah</auro-menuoption>
          <auro-menuoption value="VT">Vermont</auro-menuoption>
          <auro-menuoption value="VA">Virginia</auro-menuoption>
          <auro-menuoption value="WA">Washington</auro-menuoption>
          <auro-menuoption value="WV">West Virginia</auro-menuoption>
          <auro-menuoption value="WI">Wisconsin</auro-menuoption>
          <auro-menuoption value="WY">Wyoming</auro-menuoption>
        </auro-menu>
      </auro-select>
    </div>
  </div>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/autocomplete.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/autocomplete.html -->

```html
<div class="autofill-example-form">
  <div class="input-row">
    <auro-input autocomplete="given-name">
      <span slot="label">First Name</span>
      <span slot="bib.fullscreen.headline">First Name</span>
    </auro-input>
    <auro-input autocomplete="family-name">
      <span slot="label">Last Name</span>
      <span slot="bib.fullscreen.headline">Last Name</span>
    </auro-input>
  </div>
  <div class="input-row">
    <auro-input autocomplete="address-line1">
      <span slot="label">Street Address</span>
      <span slot="bib.fullscreen.headline">Street Address</span>
    </auro-input>
    <auro-input autocomplete="address-level2">
      <span slot="label">City</span>
      <span slot="bib.fullscreen.headline">City</span>
    </auro-input>
    <auro-select autocomplete="address-level1">
      <span slot="bib.fullscreen.headline">Select Your State</span>
      <span slot="label">Select Your State</span>
      <auro-menu>
        <auro-menuoption value="AL">Alabama</auro-menuoption>
        <auro-menuoption value="AK">Alaska</auro-menuoption>
        <auro-menuoption value="AZ">Arizona</auro-menuoption>
        <auro-menuoption value="AR">Arkansas</auro-menuoption>
        <auro-menuoption value="CA">California</auro-menuoption>
        <auro-menuoption value="CO">Colorado</auro-menuoption>
        <auro-menuoption value="CT">Connecticut</auro-menuoption>
        <auro-menuoption value="DE">Delaware</auro-menuoption>
        <auro-menuoption value="DC">District of Columbia</auro-menuoption>
        <auro-menuoption value="FL">Florida</auro-menuoption>
        <auro-menuoption value="GA">Georgia</auro-menuoption>
        <auro-menuoption value="HI">Hawaii</auro-menuoption>
        <auro-menuoption value="ID">Idaho</auro-menuoption>
        <auro-menuoption value="IL">Illinois</auro-menuoption>
        <auro-menuoption value="IN">Indiana</auro-menuoption>
        <auro-menuoption value="IA">Iowa</auro-menuoption>
        <auro-menuoption value="KS">Kansas</auro-menuoption>
        <auro-menuoption value="KY">Kentucky</auro-menuoption>
        <auro-menuoption value="LA">Louisiana</auro-menuoption>
        <auro-menuoption value="ME">Maine</auro-menuoption>
        <auro-menuoption value="MD">Maryland</auro-menuoption>
        <auro-menuoption value="MA">Massachusetts</auro-menuoption>
        <auro-menuoption value="MI">Michigan</auro-menuoption>
        <auro-menuoption value="MN">Minnesota</auro-menuoption>
        <auro-menuoption value="MS">Mississippi</auro-menuoption>
        <auro-menuoption value="MO">Missouri</auro-menuoption>
        <auro-menuoption value="MT">Montana</auro-menuoption>
        <auro-menuoption value="NE">Nebraska</auro-menuoption>
        <auro-menuoption value="NV">Nevada</auro-menuoption>
        <auro-menuoption value="NH">New Hampshire</auro-menuoption>
        <auro-menuoption value="NJ">New Jersey</auro-menuoption>
        <auro-menuoption value="NM">New Mexico</auro-menuoption>
        <auro-menuoption value="NY">New York</auro-menuoption>
        <auro-menuoption value="NC">North Carolina</auro-menuoption>
        <auro-menuoption value="ND">North Dakota</auro-menuoption>
        <auro-menuoption value="OH">Ohio</auro-menuoption>
        <auro-menuoption value="OK">Oklahoma</auro-menuoption>
        <auro-menuoption value="OR">Oregon</auro-menuoption>
        <auro-menuoption value="PA">Pennsylvania</auro-menuoption>
        <auro-menuoption value="RI">Rhode Island</auro-menuoption>
        <auro-menuoption value="SC">South Carolina</auro-menuoption>
        <auro-menuoption value="SD">South Dakota</auro-menuoption>
        <auro-menuoption value="TN">Tennessee</auro-menuoption>
        <auro-menuoption value="TX">Texas</auro-menuoption>
        <auro-menuoption value="UT">Utah</auro-menuoption>
        <auro-menuoption value="VT">Vermont</auro-menuoption>
        <auro-menuoption value="VA">Virginia</auro-menuoption>
        <auro-menuoption value="WA">Washington</auro-menuoption>
        <auro-menuoption value="WV">West Virginia</auro-menuoption>
        <auro-menuoption value="WI">Wisconsin</auro-menuoption>
        <auro-menuoption value="WY">Wyoming</auro-menuoption>
      </auro-menu>
    </auro-select>
  </div>
</div>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

## Example with auro-icons in options

Displays an `<auro-select>` element with `<auro-icon>` elements in each option.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/withIcons.html) -->
  <!-- The below content is automatically added from ./../apiExamples/withIcons.html -->
  <auro-select placeholder="Placeholder Text">
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Label</span>
    <auro-menu>
      <auro-menuoption value="air">
        <auro-icon label customColor category="health" name="air">Air</auro-icon>
      </auro-menuoption>
      <auro-menuoption value="covidtest">
        <auro-icon label customColor category="health" name="covid-test">Covid Test</auro-icon>
      </auro-menuoption>
      <auro-menuoption value="health">
        <auro-icon label customColor category="health" name="health">Health</auro-icon>
      </auro-menuoption>
      <auro-menuoption value="mask">
        <auro-icon label customColor category="health" name="mask">Mask</auro-icon>
      </auro-menuoption>
      <auro-menuoption value="spraybottle">
        <auro-icon label customColor category="health" name="spraybottle">Spray Bottle</auro-icon>
      </auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/withIcons.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/withIcons.html -->

```html
<auro-select placeholder="Placeholder Text">
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Label</span>
  <auro-menu>
    <auro-menuoption value="air">
      <auro-icon label customColor category="health" name="air">Air</auro-icon>
    </auro-menuoption>
    <auro-menuoption value="covidtest">
      <auro-icon label customColor category="health" name="covid-test">Covid Test</auro-icon>
    </auro-menuoption>
    <auro-menuoption value="health">
      <auro-icon label customColor category="health" name="health">Health</auro-icon>
    </auro-menuoption>
    <auro-menuoption value="mask">
      <auro-icon label customColor category="health" name="mask">Mask</auro-icon>
    </auro-menuoption>
    <auro-menuoption value="spraybottle">
      <auro-icon label customColor category="health" name="spraybottle">Spray Bottle</auro-icon>
    </auro-menuoption>
  </auro-menu>
</auro-select>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

## Example with nested menus

This example shows nesting `<auro-menu>` elements to create submenus.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/withSubmenus.html) -->
  <!-- The below content is automatically added from ./../apiExamples/withSubmenus.html -->
  <auro-select placeholder="Placeholder Text">
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Label</span>
    <auro-menu>
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <hr>
      <auro-menu>
        <auro-menuoption value="apples">Apples</auro-menuoption>
        <auro-menuoption value="oranges">Oranges</auro-menuoption>
        <auro-menuoption value="pears">Pears</auro-menuoption>
        <auro-menuoption value="grapes">Grapes</auro-menuoption>
        <auro-menuoption value="kiwi">Kiwi</auro-menuoption>
        <hr>
        <auro-menu>
          <auro-menuoption value="person">Person</auro-menuoption>
          <auro-menuoption value="woman">Woman</auro-menuoption>
          <auro-menuoption value="man">Man</auro-menuoption>
          <auro-menuoption value="camera">Camera</auro-menuoption>
          <auro-menuoption value="tv">TV</auro-menuoption>
        </auro-menu>
      </auro-menu>
      <hr>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <hr>
      <auro-menu>
        <auro-menuoption value="cars">Cars</auro-menuoption>
        <auro-menuoption value="trucks">Trucks</auro-menuoption>
        <auro-menuoption value="boats">Boats</auro-menuoption>
        <auro-menuoption value="planes">Planes</auro-menuoption>
        <auro-menuoption value="motorcycles">Motorcycles</auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/withSubmenus.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/withSubmenus.html -->

```html
<auro-select placeholder="Placeholder Text">
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Label</span>
  <auro-menu>
    <auro-menuoption value="stops">Stops</auro-menuoption>
    <auro-menuoption value="price">Price</auro-menuoption>
    <auro-menuoption value="duration">Duration</auro-menuoption>
    <hr>
    <auro-menu>
      <auro-menuoption value="apples">Apples</auro-menuoption>
      <auro-menuoption value="oranges">Oranges</auro-menuoption>
      <auro-menuoption value="pears">Pears</auro-menuoption>
      <auro-menuoption value="grapes">Grapes</auro-menuoption>
      <auro-menuoption value="kiwi">Kiwi</auro-menuoption>
      <hr>
      <auro-menu>
        <auro-menuoption value="person">Person</auro-menuoption>
        <auro-menuoption value="woman">Woman</auro-menuoption>
        <auro-menuoption value="man">Man</auro-menuoption>
        <auro-menuoption value="camera">Camera</auro-menuoption>
        <auro-menuoption value="tv">TV</auro-menuoption>
      </auro-menu>
    </auro-menu>
    <hr>
    <auro-menuoption value="departure">Departure</auro-menuoption>
    <auro-menuoption value="arrival">Arrival</auro-menuoption>
    <hr>
    <auro-menu>
      <auro-menuoption value="cars">Cars</auro-menuoption>
      <auro-menuoption value="trucks">Trucks</auro-menuoption>
      <auro-menuoption value="boats">Boats</auro-menuoption>
      <auro-menuoption value="planes">Planes</auro-menuoption>
      <auro-menuoption value="motorcycles">Motorcycles</auro-menuoption>
  </auro-menu>
</auro-select>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

## Example with no checkmark

Applying the `noCheckmark` attribute will prevent the checkmark icon from being shown on the selected option. The left padding to reserve space for the checkmark will not be shown.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/noCheckmark.html) -->
  <!-- The below content is automatically added from ./../apiExamples/noCheckmark.html -->
  <auro-select nocheckmark placeholder="Placeholder Text">
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Label</span>
      <auro-menu>
          <auro-menuoption value="stops">Stops</auro-menuoption>
          <auro-menuoption value="price">Price</auro-menuoption>
          <auro-menuoption value="duration">Duration</auro-menuoption>
          <auro-menuoption value="departure">Departure</auro-menuoption>
          <auro-menuoption value="arrival">Arrival</auro-menuoption>
          <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
      </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/noCheckmark.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/noCheckmark.html -->

```html
<auro-select nocheckmark placeholder="Placeholder Text">
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Label</span>
    <auro-menu>
        <auro-menuoption value="stops">Stops</auro-menuoption>
        <auro-menuoption value="price">Price</auro-menuoption>
        <auro-menuoption value="duration">Duration</auro-menuoption>
        <auro-menuoption value="departure">Departure</auro-menuoption>
        <auro-menuoption value="arrival">Arrival</auro-menuoption>
        <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
</auro-select>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

## Example with custom bib height

This example shows how to set a custom height for the bib from `<auro-dropdown>`.

Custom height dimensions are set by using the `dropdownSize` CSS Part and then applying a `max-height` rule and value.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=../apiExamples/customBibHeight.html) -->
  <!-- The below content is automatically added from ../apiExamples/customBibHeight.html -->
  <auro-select id="customBibHeightExample" placeholder="Placeholder Text">
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Label</span>
    <auro-menu>
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
  <style>
    #customBibHeightExample::part(dropdownSize) {
      max-height: 100px;
    }
  </style>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=../apiExamples/customBibHeight.html) -->
<!-- The below code snippet is automatically added from ../apiExamples/customBibHeight.html -->

```html
<auro-select id="customBibHeightExample" placeholder="Placeholder Text">
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Label</span>
  <auro-menu>
    <auro-menuoption value="stops">Stops</auro-menuoption>
    <auro-menuoption value="price">Price</auro-menuoption>
    <auro-menuoption value="duration">Duration</auro-menuoption>
    <auro-menuoption value="departure">Departure</auro-menuoption>
    <auro-menuoption value="arrival">Arrival</auro-menuoption>
    <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
  </auro-menu>
</auro-select>
<style>
  #customBibHeightExample::part(dropdownSize) {
    max-height: 100px;
  }
</style>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

## Example with fullscreen dropdown breakpoint override

This example overrides the default dropdown behavior to force a non-fullscreen view on any screen size. `disabled`
ensures that the dropdown will never be fullscreen.
Please use `xl` if you want the opposite behavior, where a dropdown is always fullscreen.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/forcedFullscreenDisabled.html) -->
  <!-- The below content is automatically added from ./../apiExamples/forcedFullscreenDisabled.html -->
  <auro-select fullscreenBreakpoint="disabled">
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Select Example</span>
    <auro-menu>
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/forcedFullscreenDisabled.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/forcedFullscreenDisabled.html -->

```html
<auro-select fullscreenBreakpoint="disabled">
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Select Example</span>
  <auro-menu>
    <auro-menuoption value="stops">Stops</auro-menuoption>
    <auro-menuoption value="price">Price</auro-menuoption>
    <auro-menuoption value="duration">Duration</auro-menuoption>
    <auro-menuoption value="departure">Departure</auro-menuoption>
    <auro-menuoption value="arrival">Arrival</auro-menuoption>
    <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
  </auro-menu>
</auro-select>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

## Error State

Use the `error` boolean attribute to toggle the error UI.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/error.html) -->
  <!-- The below content is automatically added from ./../apiExamples/error.html -->
  <auro-select error="Custom error message" placeholder="Placeholder Text">
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Label</span>
    <auro-menu>
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceError.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearanceError.html -->
  <auro-select appearance="inverse" error="Custom error message" placeholder="Placeholder Text">
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Label</span>
    <auro-menu>
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/error.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/error.html -->

```html
<auro-select error="Custom error message" placeholder="Placeholder Text">
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Label</span>
  <auro-menu>
    <auro-menuoption value="stops">Stops</auro-menuoption>
    <auro-menuoption value="price">Price</auro-menuoption>
    <auro-menuoption value="duration">Duration</auro-menuoption>
    <auro-menuoption value="departure">Departure</auro-menuoption>
    <auro-menuoption value="arrival">Arrival</auro-menuoption>
    <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
  </auro-menu>
</auro-select>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceError.html) -->
<!-- The below content is automatically added from ./../apiExamples/inverseAppearanceError.html -->
<auro-select appearance="inverse" error="Custom error message" placeholder="Placeholder Text">
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Label</span>
  <auro-menu>
    <auro-menuoption value="stops">Stops</auro-menuoption>
    <auro-menuoption value="price">Price</auro-menuoption>
    <auro-menuoption value="duration">Duration</auro-menuoption>
    <auro-menuoption value="departure">Departure</auro-menuoption>
    <auro-menuoption value="arrival">Arrival</auro-menuoption>
    <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
  </auro-menu>
</auro-select>
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

## Disabled state

Use the `disabled` boolean attribute to toggle the disabled UI.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/disabled.html) -->
  <!-- The below content is automatically added from ./../apiExamples/disabled.html -->
  <auro-select disabled placeholder="Placeholder Text">
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Label</span>
    <auro-menu>
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceDisabled.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearanceDisabled.html -->
  <auro-select appearance="inverse" disabled placeholder="Placeholder Text">
    <span slot="bib.fullscreen.headline">Bib Headline</span>
    <span slot="label">Label</span>
    <auro-menu>
      <auro-menuoption value="stops">Stops</auro-menuoption>
      <auro-menuoption value="price">Price</auro-menuoption>
      <auro-menuoption value="duration">Duration</auro-menuoption>
      <auro-menuoption value="departure">Departure</auro-menuoption>
      <auro-menuoption value="arrival">Arrival</auro-menuoption>
      <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
    </auro-menu>
  </auro-select>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/disabled.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/disabled.html -->

```html
<auro-select disabled placeholder="Placeholder Text">
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Label</span>
  <auro-menu>
    <auro-menuoption value="stops">Stops</auro-menuoption>
    <auro-menuoption value="price">Price</auro-menuoption>
    <auro-menuoption value="duration">Duration</auro-menuoption>
    <auro-menuoption value="departure">Departure</auro-menuoption>
    <auro-menuoption value="arrival">Arrival</auro-menuoption>
    <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
  </auro-menu>
</auro-select>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearanceDisabled.html) -->
<!-- The below content is automatically added from ./../apiExamples/inverseAppearanceDisabled.html -->
<auro-select appearance="inverse" disabled placeholder="Placeholder Text">
  <span slot="bib.fullscreen.headline">Bib Headline</span>
  <span slot="label">Label</span>
  <auro-menu>
    <auro-menuoption value="stops">Stops</auro-menuoption>
    <auro-menuoption value="price">Price</auro-menuoption>
    <auro-menuoption value="duration">Duration</auro-menuoption>
    <auro-menuoption value="departure">Departure</auro-menuoption>
    <auro-menuoption value="arrival">Arrival</auro-menuoption>
    <auro-menuoption value="prefer alaska">Prefer Alaska</auro-menuoption>
  </auro-menu>
</auro-select>
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>
