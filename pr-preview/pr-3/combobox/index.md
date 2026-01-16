# Combobox

<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../docs/partials/description.md) -->
<!-- The below content is automatically added from ./../docs/partials/description.md -->
`<auro-combobox>` is the combination of [dropdown](http://auro.alaskaair.com/components/auro/dropdown), [input](http://auro.alaskaair.com/components/auro/input), and [menu](http://auro.alaskaair.com/components/auro/menu) and allows users to filter search results from a predefined list as they type. When the user starts typing in the text input, a dropdown of a menu shows up to display options that match the user’s search.

By default, `auro-combobox` behaves as a suggestion list. This means any value may be typed into the combobox and the menu list presented effectively provides sample or suggestion options. With the use of the `persistInput` attribute the `auro-combobox` behaves as a filter of menu options. In this mode. typing into the input field will execute the filter but will not set the `value` of the combobox. The combobox value is set by selecting a menu option. Clicking the `X` clear button in the input will remove the current value of the HTML5 input causing the menu filter to reset as well as remove the current value of the combobox.
<!-- AURO-GENERATED-CONTENT:END -->

## auro-combobox use cases

<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../docs/partials/useCases.md) -->
<!-- The below content is automatically added from ./../docs/partials/useCases.md -->
The `<auro-combobox>` element should be used in situations where users may:

* Search
  * Airports: user looks for a specific airport by searching for the city name or airport code
  * Site wide: user searches for a topic site wide and combobox makes suggestions on searchable results
* Filter
  * Options: user chooses filters for their search by using combobox
* Select
  * Quantity: user types a quantity to select an option within a range (for example, the user may be limited to 2-34)
<!-- AURO-GENERATED-CONTENT:END -->

## Example(s)

## Default

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/basic.html) -->
  <!-- The below content is automatically added from ./../apiExamples/basic.html -->
  <auro-combobox>
    <span slot="ariaLabel.bib.close">Close combobox</span>
    <span slot="ariaLabel.input.clear">Clear All</span>
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/basic.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/basic.html -->

```html
<auro-combobox>
  <span slot="ariaLabel.bib.close">Close combobox</span>
  <span slot="ariaLabel.input.clear">Clear All</span>
  <span slot="bib.fullscreen.headline">Bib Header</span>
  <span slot="label">Name</span>
  <auro-menu>
    <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
    <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
    <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
    <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
    <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
    <auro-menuoption static nomatch>No matching option</auro-menuoption>
  </auro-menu>
</auro-combobox>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

## Layouts

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/classic/basic.html) -->
  <!-- The below content is automatically added from ./../apiExamples/classic/basic.html -->
  <auro-combobox layout="classic" shape="classic" size="lg" placeholder="Placeholder content" required style="width: 249px;">
    <span slot="ariaLabel.bib.close">Close combobox</span>
    <span slot="ariaLabel.input.clear">Clear All</span>
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
    <span slot="helpText">
      Help text - Lorem ipsum solar lorem ipsum solar
    </span>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/classic/inverseAppearance.html) -->
  <!-- The below content is automatically added from ./../apiExamples/classic/inverseAppearance.html -->
  <auro-combobox layout="classic" shape="classic" size="lg" placeholder="Placeholder content" appearance="inverse" required style="width: 249px;">
    <span slot="ariaLabel.bib.close">Close combobox</span>
    <span slot="ariaLabel.input.clear">Clear All</span>
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
    <span slot="helpText">
      Help text - Lorem ipsum solar lorem ipsum solar
    </span>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>

### Emphasized

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/emphasized/basic.html) -->
  <!-- The below content is automatically added from ./../apiExamples/emphasized/basic.html -->
  <auro-combobox layout="emphasized" value="Oranges" shape="pill" size="xl" placeholder="Placeholder content" required style="width: 249px;">
    <span slot="ariaLabel.bib.close">Close combobox</span>
    <span slot="ariaLabel.input.clear">Clear All</span>
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
    <span slot="helpText">
      Help text - Lorem ipsum solar lorem ipsum solar
    </span>
    <span slot="displayValue">
      <div>
        <div class="mainText">Apples</div>
        <div class="subText">Fruit</div>
      </div>
    </span>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>

### Snowflake

<div class="exampleWrapper--ondark">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/snowflake/basic.html) -->
  <!-- The below content is automatically added from ./../apiExamples/snowflake/basic.html -->
  <auro-combobox layout="snowflake" shape="snowflake" size="lg" placeholder="Placeholder content" required appearance="inverse" style="width: 249px;">
    <span slot="ariaLabel.bib.close">Close combobox</span>
    <span slot="ariaLabel.input.clear">Clear All</span>
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
    <span slot="helpText">
      Help text - Lorem ipsum solar lorem ipsum solar
    </span>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>

### Classic

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/basic.html) -->
  <!-- The below content is automatically added from ./../apiExamples/basic.html -->
  <auro-combobox>
    <span slot="ariaLabel.bib.close">Close combobox</span>
    <span slot="ariaLabel.input.clear">Clear All</span>
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<div class="exampleWrapper--ondark" aria-hidden>
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearance.html) -->
  <!-- The below content is automatically added from ./../apiExamples/inverseAppearance.html -->
  <auro-combobox appearance="inverse">
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/basic.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/basic.html -->

```html
<auro-combobox>
  <span slot="ariaLabel.bib.close">Close combobox</span>
  <span slot="ariaLabel.input.clear">Clear All</span>
  <span slot="bib.fullscreen.headline">Bib Header</span>
  <span slot="label">Name</span>
  <auro-menu>
    <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
    <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
    <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
    <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
    <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
    <auro-menuoption static nomatch>No matching option</auro-menuoption>
  </auro-menu>
</auro-combobox>
```
<!-- AURO-GENERATED-CONTENT:END -->
<!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/inverseAppearance.html) -->
<!-- The below content is automatically added from ./../apiExamples/inverseAppearance.html -->
<auro-combobox appearance="inverse">
  <span slot="bib.fullscreen.headline">Bib Header</span>
  <span slot="label">Name</span>
  <auro-menu>
    <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
    <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
    <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
    <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
    <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
    <auro-menuoption static nomatch>No matching option</auro-menuoption>
  </auro-menu>
</auro-combobox>
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Behavior

There are two behaviors available for the combo box: suggestion and filter.
The default behavior is "suggestion".

#### Suggestion

With the suggestion behavior, the menu options are displayed to the user as suggestions, but the user may enter whatever value they like into the input

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/suggestion.html) -->
  <!-- The below content is automatically added from ./../apiExamples/suggestion.html -->
  <auro-combobox behavior="suggestion">
    <span slot="ariaLabel.bib.close">Close combobox</span>
    <span slot="ariaLabel.input.clear">Clear All</span>
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/suggestion.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/suggestion.html -->

```html
<auro-combobox behavior="suggestion">
  <span slot="ariaLabel.bib.close">Close combobox</span>
  <span slot="ariaLabel.input.clear">Clear All</span>
  <span slot="bib.fullscreen.headline">Bib Header</span>
  <span slot="label">Name</span>
  <auro-menu>
    <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
    <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
    <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
    <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
    <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
    <auro-menuoption static nomatch>No matching option</auro-menuoption>
  </auro-menu>
</auro-combobox>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

#### Filter

With the filter behavior, the menu options are displayed to the user, and the user is required to choose one of the menu options in order for the input to be considered valid.

The `setCustomValidityValueMissingFilter` attribute is also available to display a custom message to the user when this validation check fails.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/filter.html) -->
  <!-- The below content is automatically added from ./../apiExamples/filter.html -->
  <auro-combobox behavior="filter" setCustomValidityValueMissingFilter="Please select an option from the list">
    <span slot="ariaLabel.bib.close">Close combobox</span>
    <span slot="ariaLabel.input.clear">Clear All</span>
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/filter.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/filter.html -->

```html
<auro-combobox behavior="filter" setCustomValidityValueMissingFilter="Please select an option from the list">
  <span slot="ariaLabel.bib.close">Close combobox</span>
  <span slot="ariaLabel.input.clear">Clear All</span>
  <span slot="bib.fullscreen.headline">Bib Header</span>
  <span slot="label">Name</span>
  <auro-menu>
    <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
    <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
    <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
    <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
    <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
    <auro-menuoption static nomatch>No matching option</auro-menuoption>
  </auro-menu>
</auro-combobox>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Airports example

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/airports.html) -->
  <!-- The below content is automatically added from ./../apiExamples/airports.html -->
  <auro-combobox>
    <span slot="bib.fullscreen.headline">Airports</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="fca" id="airport-fca" suggest="fca montana kalispell">glacier park international</auro-menuoption>
      <auro-menuoption value="sfo" id="airport-sfo" suggest="sfo california san francisco">san francisco international</auro-menuoption>
      <auro-menuoption value="boi" id="airport-boi" suggest="boi idaho boise">gowen field</auro-menuoption>
      <auro-menuoption value="stl" id="airport-stl" suggest="stl missouri st louis">lambert st louis international</auro-menuoption>
      <auro-menuoption value="ylw" id="airport-ylw" suggest="ylw british columbia kelowna">kelowna international</auro-menuoption>
      <auro-menuoption value="ykm" id="airport-ykm" suggest="ykm washington yakima">yakima air terminal</auro-menuoption>
      <auro-menuoption value="puw" id="airport-puw" suggest="puw washington pullman">pullman moscow regional</auro-menuoption>
      <auro-menuoption value="yeg" id="airport-yeg" suggest="yeg alberta edmonton">edmonton international</auro-menuoption>
      <auro-menuoption value="tpa" id="airport-tpa" suggest="tpa florida tampa">tampa international</auro-menuoption>
      <auro-menuoption value="msp" id="airport-msp" suggest="msp minnesota minneapolis">minneapolis st paul international</auro-menuoption>
      <auro-menuoption value="ida" id="airport-ida" suggest="ida idaho idaho falls">idaho falls regional airport</auro-menuoption>
      <auro-menuoption value="mfr" id="airport-mfr" suggest="mfr oregon medford">rogue valley international</auro-menuoption>
      <auro-menuoption value="psp" id="airport-psp" suggest="psp california palm springs">palm springs international</auro-menuoption>
      <auro-menuoption value="lir" id="airport-lir" suggest="lir guanacaste liberia">guanacaste airport</auro-menuoption>
      <auro-menuoption value="oak" id="airport-oak" suggest="oak california oakland">oakland international</auro-menuoption>
      <auro-menuoption value="bos" id="airport-bos" suggest="bos massachusetts boston">logan international</auro-menuoption>
      <auro-menuoption value="bwi" id="airport-bwi" suggest="bwi maryland baltimore">thurgood marshall international</auro-menuoption>
      <auro-menuoption value="dal" id="airport-dal" suggest="dal texas dallas">dallas love field</auro-menuoption>
      <auro-menuoption value="sba" id="airport-sba" suggest="sba california santa barbara">santa barbara municipal</auro-menuoption>
      <auro-menuoption value="mci" id="airport-mci" suggest="mci missouri kansas city">kansas city international</auro-menuoption>
      <auro-menuoption value="koa" id="airport-koa" suggest="koa hawaii kona">kona international</auro-menuoption>
      <auro-menuoption value="pvr" id="airport-pvr" suggest="pvr jalisco puerto vallarta">licenciado gustavo diaz ordaz international</auro-menuoption>
      <auro-menuoption value="wrg" id="airport-wrg" suggest="wrg alaska wrangell">wrangell</auro-menuoption>
      <auro-menuoption value="scc" id="airport-scc" suggest="scc alaska prudhoe bay">deadhorse</auro-menuoption>
      <auro-menuoption value="lto" id="airport-lto" suggest="lto baja california loreto">loreto international</auro-menuoption>
      <auro-menuoption value="ome" id="airport-ome" suggest="ome alaska nome">nome</auro-menuoption>
      <auro-menuoption value="ict" id="airport-ict" suggest="ict kansas wichita">dwight d eisenhower national</auro-menuoption>
      <auro-menuoption value="phl" id="airport-phl" suggest="phl pennsylvania philadelphia">philadelphia international</auro-menuoption>
      <auro-menuoption value="dfw" id="airport-dfw" suggest="dfw texas dallas">dallas fort worth international</auro-menuoption>
      <auro-menuoption value="ind" id="airport-ind" suggest="ind indiana indianapolis">indianapolis international</auro-menuoption>
      <auro-menuoption value="smf" id="airport-smf" suggest="smf california sacramento">sacramento international</auro-menuoption>
      <auro-menuoption value="sit" id="airport-sit" suggest="sit alaska sitka">rocky gutierrez</auro-menuoption>
      <auro-menuoption value="dut" id="airport-dut" suggest="dut alaska dutch harbor">unalaska</auro-menuoption>
      <auro-menuoption value="cdv" id="airport-cdv" suggest="cdv alaska cordova">merle mudhole smith</auro-menuoption>
      <auro-menuoption value="psg" id="airport-psg" suggest="psg alaska petersburg">james a johnson</auro-menuoption>
      <auro-menuoption value="bna" id="airport-bna" suggest="bna tennessee nashville">nashville international</auro-menuoption>
      <auro-menuoption value="geg" id="airport-geg" suggest="geg washington spokane">spokane international</auro-menuoption>
      <auro-menuoption value="ktn" id="airport-ktn" suggest="ktn alaska ketchikan">ketchikan international</auro-menuoption>
      <auro-menuoption value="pit" id="airport-pit" suggest="pit pennsylvania pittsburgh">pittsburgh international</auro-menuoption>
      <auro-menuoption value="sbp" id="airport-sbp" suggest="sbp california san luis obispo">san luis obispo regional</auro-menuoption>
      <auro-menuoption value="bur" id="airport-bur" suggest="bur california burbank">hollywood burbank</auro-menuoption>
      <auro-menuoption value="msy" id="airport-msy" suggest="msy louisiana new orleans">louis armstrong international</auro-menuoption>
      <auro-menuoption value="pae" id="airport-pae" suggest="pae washington everett">paine field</auro-menuoption>
      <auro-menuoption value="cvg" id="airport-cvg" suggest="cvg ohio cincinnati">cincinnati northern kentucky international</auro-menuoption>
      <auro-menuoption value="yak" id="airport-yak" suggest="yak alaska yakutat">yakutat</auro-menuoption>
      <auro-menuoption value="pdx" id="airport-pdx" suggest="pdx oregon portland">portland international</auro-menuoption>
      <auro-menuoption value="anc" id="airport-anc" suggest="anc alaska anchorage">ted stevens</auro-menuoption>
      <auro-menuoption value="sea" id="airport-sea" suggest="sea washington seattle">seattle tacoma international</auro-menuoption>
      <auro-menuoption value="san" id="airport-san" suggest="san california san diego">san diego international</auro-menuoption>
      <auro-menuoption value="sat" id="airport-sat" suggest="sat texas san antonio">san antonio international</auro-menuoption>
      <auro-menuoption value="fat" id="airport-fat" suggest="fat california fresno">fresno yosemite international</auro-menuoption>
      <auro-menuoption value="aus" id="airport-aus" suggest="aus texas austin">austin bergstrom international</auro-menuoption>
      <auro-menuoption value="ord" id="airport-ord" suggest="ord illinois chicago">ohare international</auro-menuoption>
      <auro-menuoption value="gdl" id="airport-gdl" suggest="gdl jalisco guadalajara">guadalajara international</auro-menuoption>
      <auro-menuoption value="sjc" id="airport-sjc" suggest="sjc california san jose">san jose international</auro-menuoption>
      <auro-menuoption value="jnu" id="airport-jnu" suggest="jnu alaska juneau">juneau international</auro-menuoption>
      <auro-menuoption value="rdm" id="airport-rdm" suggest="rdm oregon redmond">roberts field</auro-menuoption>
      <auro-menuoption value="sts" id="airport-sts" suggest="sts california sonoma">charles m schulz</auro-menuoption>
      <auro-menuoption value="fai" id="airport-fai" suggest="fai alaska fairbanks">fairbanks international</auro-menuoption>
      <auro-menuoption value="rdu" id="airport-rdu" suggest="rdu north carolina raleigh">raleigh durham international</auro-menuoption>
      <auro-menuoption value="oma" id="airport-oma" suggest="oma nebraska omaha">eppley airfield</auro-menuoption>
      <auro-menuoption value="bzn" id="airport-bzn" suggest="bzn montana bozeman">bozeman yellowstone international</auro-menuoption>
      <auro-menuoption value="ont" id="airport-ont" suggest="ont california ontario">ontario international</auro-menuoption>
      <auro-menuoption value="ogg" id="airport-ogg" suggest="ogg hawaii maui">kahului international</auro-menuoption>
      <auro-menuoption value="sun" id="airport-sun" suggest="sun idaho sun valley">friedman memorial</auro-menuoption>
      <auro-menuoption value="mzt" id="airport-mzt" suggest="mzt sinaloa mazatlan">general rafael buelna international</auro-menuoption>
      <auro-menuoption value="dlg" id="airport-dlg" suggest="dlg alaska dillingham">dillingham</auro-menuoption>
      <auro-menuoption value="adq" id="airport-adq" suggest="adq alaska kodiak">kodiak</auro-menuoption>
      <auro-menuoption value="den" id="airport-den" suggest="den colorado denver">denver international</auro-menuoption>
      <auro-menuoption value="zlo" id="airport-zlo" suggest="zlo colima manzanillo">manzanillo international</auro-menuoption>
      <auro-menuoption value="sjd" id="airport-sjd" suggest="sjd baja california los cabos">los cabos international</auro-menuoption>
      <auro-menuoption value="elp" id="airport-elp" suggest="elp texas el paso">el paso international airport</auro-menuoption>
      <auro-menuoption value="atl" id="airport-atl" suggest="atl georgia atlanta">hartsfield jackson international</auro-menuoption>
      <auro-menuoption value="lax" id="airport-lax" suggest="lax california los angeles">los angeles international</auro-menuoption>
      <auro-menuoption value="rsw" id="airport-rsw" suggest="rsw florida fort myers">southwest florida international</auro-menuoption>
      <auro-menuoption value="cle" id="airport-cle" suggest="cle ohio cleveland">cleveland hopkins international airport</auro-menuoption>
      <auro-menuoption value="otz" id="airport-otz" suggest="otz alaska kotzebue">ralph wien memorial</auro-menuoption>
      <auro-menuoption value="bze" id="airport-bze" suggest="bze belize belize city">philip sw goldson international airport</auro-menuoption>
      <auro-menuoption value="eat" id="airport-eat" suggest="eat washington wenatchee">pangborn memorial</auro-menuoption>
      <auro-menuoption value="dtw" id="airport-dtw" suggest="dtw michigan detroit">detroit metropolitan</auro-menuoption>
      <auro-menuoption value="bet" id="airport-bet" suggest="bet alaska bethel">bethel</auro-menuoption>
      <auro-menuoption value="dca" id="airport-dca" suggest="dca district of columbia washington">ronald reagan national</auro-menuoption>
      <auro-menuoption value="rno" id="airport-rno" suggest="rno nevada reno">reno tahoe international</auro-menuoption>
      <auro-menuoption value="brw" id="airport-brw" suggest="brw alaska barrow">wiley post will rogers</auro-menuoption>
      <auro-menuoption value="mry" id="airport-mry" suggest="mry california monterey">monterey regional</auro-menuoption>
      <auro-menuoption value="hnl" id="airport-hnl" suggest="hnl hawaii oahu">honolulu international</auro-menuoption>
      <auro-menuoption value="okc" id="airport-okc" suggest="okc oklahoma oklahoma city">will rogers world</auro-menuoption>
      <auro-menuoption value="iad" id="airport-iad" suggest="iad virginia dulles">washington dulles international</auro-menuoption>
      <auro-menuoption value="mia" id="airport-mia" suggest="mia florida miami">miami international</auro-menuoption>
      <auro-menuoption value="bli" id="airport-bli" suggest="bli washington bellingham">bellingham international</auro-menuoption>
      <auro-menuoption value="hln" id="airport-hln" suggest="hln montana helena">helena regional</auro-menuoption>
      <auro-menuoption value="gtf" id="airport-gtf" suggest="gtf montana great falls">great falls international</auro-menuoption>
      <auro-menuoption value="zih" id="airport-zih" suggest="zih guerrero zihuatanejo">ixtapa zihuatanejo international</auro-menuoption>
      <auro-menuoption value="yyc" id="airport-yyc" suggest="yyc alberta calgary">calgary international</auro-menuoption>
      <auro-menuoption value="sna" id="airport-sna" suggest="sna california santa ana">john wayne</auro-menuoption>
      <auro-menuoption value="fll" id="airport-fll" suggest="fll florida fort lauderdale">fort lauderdale hollywood international</auro-menuoption>
      <auro-menuoption value="ewr" id="airport-ewr" suggest="ewr new jersey newark">newark liberty international</auro-menuoption>
      <auro-menuoption value="hdn" id="airport-hdn" suggest="hdn colorado steamboat springs">yampa valley regional</auro-menuoption>
      <auro-menuoption value="psc" id="airport-psc" suggest="psc washington pasco">tri cities</auro-menuoption>
      <auro-menuoption value="tus" id="airport-tus" suggest="tus arizona tucson">tucson international</auro-menuoption>
      <auro-menuoption value="abq" id="airport-abq" suggest="abq new mexico albuquerque">albuquerque international sunport</auro-menuoption>
      <auro-menuoption value="jfk" id="airport-jfk" suggest="jfk new york new york">john f kennedy international</auro-menuoption>
      <auro-menuoption value="yvr" id="airport-yvr" suggest="yvr british columbia vancouver">vancouver international</auro-menuoption>
      <auro-menuoption value="sjo" id="airport-sjo" suggest="sjo san jose alajuela province">juan santamaria international</auro-menuoption>
      <auro-menuoption value="las" id="airport-las" suggest="las nevada las vegas">harry reid international airport</auro-menuoption>
      <auro-menuoption value="lih" id="airport-lih" suggest="lih hawaii kauai">lihue international</auro-menuoption>
      <auro-menuoption value="mso" id="airport-mso" suggest="mso montana missoula">missoula international</auro-menuoption>
      <auro-menuoption value="alw" id="airport-alw" suggest="alw washington walla walla">walla walla regional</auro-menuoption>
      <auro-menuoption value="mke" id="airport-mke" suggest="mke wisconsin milwaukee">milwaukee mitchell international</auro-menuoption>
      <auro-menuoption value="eug" id="airport-eug" suggest="eug oregon eugene">mahlon sweet field</auro-menuoption>
      <auro-menuoption value="akn" id="airport-akn" suggest="akn alaska king salmon">king salmon</auro-menuoption>
      <auro-menuoption value="cun" id="airport-cun" suggest="cun quintana roo cancun">cancun international</auro-menuoption>
      <auro-menuoption value="rdd" id="airport-rdd" suggest="rdd california redding">redding municipal airport</auro-menuoption>
      <auro-menuoption value="mco" id="airport-mco" suggest="mco florida orlando">orlando international</auro-menuoption>
      <auro-menuoption value="slc" id="airport-slc" suggest="slc utah salt lake city">salt lake city international</auro-menuoption>
      <auro-menuoption value="phx" id="airport-phx" suggest="phx arizona phoenix">sky harbor international</auro-menuoption>
      <auro-menuoption value="bil" id="airport-bil" suggest="bil montana billings">billings logan international</auro-menuoption>
      <auro-menuoption value="gst" id="airport-gst" suggest="gst alaska gustavus">gustavus</auro-menuoption>
      <auro-menuoption value="adk" id="airport-adk" suggest="adk alaska adak">adak</auro-menuoption>
      <auro-menuoption value="cvg" id="airport-cvg" suggest="cvg kentucky hebron">cincinnati northern kentucky international</auro-menuoption>
      <auro-menuoption value="jac" id="airport-jac" suggest="jac wyoming jackson">jackson hole airport</auro-menuoption>
      <auro-menuoption value="cmh" id="airport-cmh" suggest="cmh ohio columbus">john glenn columbus international</auro-menuoption>
      <auro-menuoption value="yyj" id="airport-yyj" suggest="yyj british columbia victoria">victoria international</auro-menuoption>
      <auro-menuoption value="chs" id="airport-chs" suggest="chs south carolina charleston">charleston international</auro-menuoption>
      <auro-menuoption value="iah" id="airport-iah" suggest="iah texas houston">george bush intercontinental</auro-menuoption>
      <auro-menuoption static nomatch>Unknown airport... </auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/airports.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/airports.html -->

```html
<auro-combobox>
  <span slot="bib.fullscreen.headline">Airports</span>
  <span slot="label">Name</span>
  <auro-menu>
    <auro-menuoption value="fca" id="airport-fca" suggest="fca montana kalispell">glacier park international</auro-menuoption>
    <auro-menuoption value="sfo" id="airport-sfo" suggest="sfo california san francisco">san francisco international</auro-menuoption>
    <auro-menuoption value="boi" id="airport-boi" suggest="boi idaho boise">gowen field</auro-menuoption>
    <auro-menuoption value="stl" id="airport-stl" suggest="stl missouri st louis">lambert st louis international</auro-menuoption>
    <auro-menuoption value="ylw" id="airport-ylw" suggest="ylw british columbia kelowna">kelowna international</auro-menuoption>
    <auro-menuoption value="ykm" id="airport-ykm" suggest="ykm washington yakima">yakima air terminal</auro-menuoption>
    <auro-menuoption value="puw" id="airport-puw" suggest="puw washington pullman">pullman moscow regional</auro-menuoption>
    <auro-menuoption value="yeg" id="airport-yeg" suggest="yeg alberta edmonton">edmonton international</auro-menuoption>
    <auro-menuoption value="tpa" id="airport-tpa" suggest="tpa florida tampa">tampa international</auro-menuoption>
    <auro-menuoption value="msp" id="airport-msp" suggest="msp minnesota minneapolis">minneapolis st paul international</auro-menuoption>
    <auro-menuoption value="ida" id="airport-ida" suggest="ida idaho idaho falls">idaho falls regional airport</auro-menuoption>
    <auro-menuoption value="mfr" id="airport-mfr" suggest="mfr oregon medford">rogue valley international</auro-menuoption>
    <auro-menuoption value="psp" id="airport-psp" suggest="psp california palm springs">palm springs international</auro-menuoption>
    <auro-menuoption value="lir" id="airport-lir" suggest="lir guanacaste liberia">guanacaste airport</auro-menuoption>
    <auro-menuoption value="oak" id="airport-oak" suggest="oak california oakland">oakland international</auro-menuoption>
    <auro-menuoption value="bos" id="airport-bos" suggest="bos massachusetts boston">logan international</auro-menuoption>
    <auro-menuoption value="bwi" id="airport-bwi" suggest="bwi maryland baltimore">thurgood marshall international</auro-menuoption>
    <auro-menuoption value="dal" id="airport-dal" suggest="dal texas dallas">dallas love field</auro-menuoption>
    <auro-menuoption value="sba" id="airport-sba" suggest="sba california santa barbara">santa barbara municipal</auro-menuoption>
    <auro-menuoption value="mci" id="airport-mci" suggest="mci missouri kansas city">kansas city international</auro-menuoption>
    <auro-menuoption value="koa" id="airport-koa" suggest="koa hawaii kona">kona international</auro-menuoption>
    <auro-menuoption value="pvr" id="airport-pvr" suggest="pvr jalisco puerto vallarta">licenciado gustavo diaz ordaz international</auro-menuoption>
    <auro-menuoption value="wrg" id="airport-wrg" suggest="wrg alaska wrangell">wrangell</auro-menuoption>
    <auro-menuoption value="scc" id="airport-scc" suggest="scc alaska prudhoe bay">deadhorse</auro-menuoption>
    <auro-menuoption value="lto" id="airport-lto" suggest="lto baja california loreto">loreto international</auro-menuoption>
    <auro-menuoption value="ome" id="airport-ome" suggest="ome alaska nome">nome</auro-menuoption>
    <auro-menuoption value="ict" id="airport-ict" suggest="ict kansas wichita">dwight d eisenhower national</auro-menuoption>
    <auro-menuoption value="phl" id="airport-phl" suggest="phl pennsylvania philadelphia">philadelphia international</auro-menuoption>
    <auro-menuoption value="dfw" id="airport-dfw" suggest="dfw texas dallas">dallas fort worth international</auro-menuoption>
    <auro-menuoption value="ind" id="airport-ind" suggest="ind indiana indianapolis">indianapolis international</auro-menuoption>
    <auro-menuoption value="smf" id="airport-smf" suggest="smf california sacramento">sacramento international</auro-menuoption>
    <auro-menuoption value="sit" id="airport-sit" suggest="sit alaska sitka">rocky gutierrez</auro-menuoption>
    <auro-menuoption value="dut" id="airport-dut" suggest="dut alaska dutch harbor">unalaska</auro-menuoption>
    <auro-menuoption value="cdv" id="airport-cdv" suggest="cdv alaska cordova">merle mudhole smith</auro-menuoption>
    <auro-menuoption value="psg" id="airport-psg" suggest="psg alaska petersburg">james a johnson</auro-menuoption>
    <auro-menuoption value="bna" id="airport-bna" suggest="bna tennessee nashville">nashville international</auro-menuoption>
    <auro-menuoption value="geg" id="airport-geg" suggest="geg washington spokane">spokane international</auro-menuoption>
    <auro-menuoption value="ktn" id="airport-ktn" suggest="ktn alaska ketchikan">ketchikan international</auro-menuoption>
    <auro-menuoption value="pit" id="airport-pit" suggest="pit pennsylvania pittsburgh">pittsburgh international</auro-menuoption>
    <auro-menuoption value="sbp" id="airport-sbp" suggest="sbp california san luis obispo">san luis obispo regional</auro-menuoption>
    <auro-menuoption value="bur" id="airport-bur" suggest="bur california burbank">hollywood burbank</auro-menuoption>
    <auro-menuoption value="msy" id="airport-msy" suggest="msy louisiana new orleans">louis armstrong international</auro-menuoption>
    <auro-menuoption value="pae" id="airport-pae" suggest="pae washington everett">paine field</auro-menuoption>
    <auro-menuoption value="cvg" id="airport-cvg" suggest="cvg ohio cincinnati">cincinnati northern kentucky international</auro-menuoption>
    <auro-menuoption value="yak" id="airport-yak" suggest="yak alaska yakutat">yakutat</auro-menuoption>
    <auro-menuoption value="pdx" id="airport-pdx" suggest="pdx oregon portland">portland international</auro-menuoption>
    <auro-menuoption value="anc" id="airport-anc" suggest="anc alaska anchorage">ted stevens</auro-menuoption>
    <auro-menuoption value="sea" id="airport-sea" suggest="sea washington seattle">seattle tacoma international</auro-menuoption>
    <auro-menuoption value="san" id="airport-san" suggest="san california san diego">san diego international</auro-menuoption>
    <auro-menuoption value="sat" id="airport-sat" suggest="sat texas san antonio">san antonio international</auro-menuoption>
    <auro-menuoption value="fat" id="airport-fat" suggest="fat california fresno">fresno yosemite international</auro-menuoption>
    <auro-menuoption value="aus" id="airport-aus" suggest="aus texas austin">austin bergstrom international</auro-menuoption>
    <auro-menuoption value="ord" id="airport-ord" suggest="ord illinois chicago">ohare international</auro-menuoption>
    <auro-menuoption value="gdl" id="airport-gdl" suggest="gdl jalisco guadalajara">guadalajara international</auro-menuoption>
    <auro-menuoption value="sjc" id="airport-sjc" suggest="sjc california san jose">san jose international</auro-menuoption>
    <auro-menuoption value="jnu" id="airport-jnu" suggest="jnu alaska juneau">juneau international</auro-menuoption>
    <auro-menuoption value="rdm" id="airport-rdm" suggest="rdm oregon redmond">roberts field</auro-menuoption>
    <auro-menuoption value="sts" id="airport-sts" suggest="sts california sonoma">charles m schulz</auro-menuoption>
    <auro-menuoption value="fai" id="airport-fai" suggest="fai alaska fairbanks">fairbanks international</auro-menuoption>
    <auro-menuoption value="rdu" id="airport-rdu" suggest="rdu north carolina raleigh">raleigh durham international</auro-menuoption>
    <auro-menuoption value="oma" id="airport-oma" suggest="oma nebraska omaha">eppley airfield</auro-menuoption>
    <auro-menuoption value="bzn" id="airport-bzn" suggest="bzn montana bozeman">bozeman yellowstone international</auro-menuoption>
    <auro-menuoption value="ont" id="airport-ont" suggest="ont california ontario">ontario international</auro-menuoption>
    <auro-menuoption value="ogg" id="airport-ogg" suggest="ogg hawaii maui">kahului international</auro-menuoption>
    <auro-menuoption value="sun" id="airport-sun" suggest="sun idaho sun valley">friedman memorial</auro-menuoption>
    <auro-menuoption value="mzt" id="airport-mzt" suggest="mzt sinaloa mazatlan">general rafael buelna international</auro-menuoption>
    <auro-menuoption value="dlg" id="airport-dlg" suggest="dlg alaska dillingham">dillingham</auro-menuoption>
    <auro-menuoption value="adq" id="airport-adq" suggest="adq alaska kodiak">kodiak</auro-menuoption>
    <auro-menuoption value="den" id="airport-den" suggest="den colorado denver">denver international</auro-menuoption>
    <auro-menuoption value="zlo" id="airport-zlo" suggest="zlo colima manzanillo">manzanillo international</auro-menuoption>
    <auro-menuoption value="sjd" id="airport-sjd" suggest="sjd baja california los cabos">los cabos international</auro-menuoption>
    <auro-menuoption value="elp" id="airport-elp" suggest="elp texas el paso">el paso international airport</auro-menuoption>
    <auro-menuoption value="atl" id="airport-atl" suggest="atl georgia atlanta">hartsfield jackson international</auro-menuoption>
    <auro-menuoption value="lax" id="airport-lax" suggest="lax california los angeles">los angeles international</auro-menuoption>
    <auro-menuoption value="rsw" id="airport-rsw" suggest="rsw florida fort myers">southwest florida international</auro-menuoption>
    <auro-menuoption value="cle" id="airport-cle" suggest="cle ohio cleveland">cleveland hopkins international airport</auro-menuoption>
    <auro-menuoption value="otz" id="airport-otz" suggest="otz alaska kotzebue">ralph wien memorial</auro-menuoption>
    <auro-menuoption value="bze" id="airport-bze" suggest="bze belize belize city">philip sw goldson international airport</auro-menuoption>
    <auro-menuoption value="eat" id="airport-eat" suggest="eat washington wenatchee">pangborn memorial</auro-menuoption>
    <auro-menuoption value="dtw" id="airport-dtw" suggest="dtw michigan detroit">detroit metropolitan</auro-menuoption>
    <auro-menuoption value="bet" id="airport-bet" suggest="bet alaska bethel">bethel</auro-menuoption>
    <auro-menuoption value="dca" id="airport-dca" suggest="dca district of columbia washington">ronald reagan national</auro-menuoption>
    <auro-menuoption value="rno" id="airport-rno" suggest="rno nevada reno">reno tahoe international</auro-menuoption>
    <auro-menuoption value="brw" id="airport-brw" suggest="brw alaska barrow">wiley post will rogers</auro-menuoption>
    <auro-menuoption value="mry" id="airport-mry" suggest="mry california monterey">monterey regional</auro-menuoption>
    <auro-menuoption value="hnl" id="airport-hnl" suggest="hnl hawaii oahu">honolulu international</auro-menuoption>
    <auro-menuoption value="okc" id="airport-okc" suggest="okc oklahoma oklahoma city">will rogers world</auro-menuoption>
    <auro-menuoption value="iad" id="airport-iad" suggest="iad virginia dulles">washington dulles international</auro-menuoption>
    <auro-menuoption value="mia" id="airport-mia" suggest="mia florida miami">miami international</auro-menuoption>
    <auro-menuoption value="bli" id="airport-bli" suggest="bli washington bellingham">bellingham international</auro-menuoption>
    <auro-menuoption value="hln" id="airport-hln" suggest="hln montana helena">helena regional</auro-menuoption>
    <auro-menuoption value="gtf" id="airport-gtf" suggest="gtf montana great falls">great falls international</auro-menuoption>
    <auro-menuoption value="zih" id="airport-zih" suggest="zih guerrero zihuatanejo">ixtapa zihuatanejo international</auro-menuoption>
    <auro-menuoption value="yyc" id="airport-yyc" suggest="yyc alberta calgary">calgary international</auro-menuoption>
    <auro-menuoption value="sna" id="airport-sna" suggest="sna california santa ana">john wayne</auro-menuoption>
    <auro-menuoption value="fll" id="airport-fll" suggest="fll florida fort lauderdale">fort lauderdale hollywood international</auro-menuoption>
    <auro-menuoption value="ewr" id="airport-ewr" suggest="ewr new jersey newark">newark liberty international</auro-menuoption>
    <auro-menuoption value="hdn" id="airport-hdn" suggest="hdn colorado steamboat springs">yampa valley regional</auro-menuoption>
    <auro-menuoption value="psc" id="airport-psc" suggest="psc washington pasco">tri cities</auro-menuoption>
    <auro-menuoption value="tus" id="airport-tus" suggest="tus arizona tucson">tucson international</auro-menuoption>
    <auro-menuoption value="abq" id="airport-abq" suggest="abq new mexico albuquerque">albuquerque international sunport</auro-menuoption>
    <auro-menuoption value="jfk" id="airport-jfk" suggest="jfk new york new york">john f kennedy international</auro-menuoption>
    <auro-menuoption value="yvr" id="airport-yvr" suggest="yvr british columbia vancouver">vancouver international</auro-menuoption>
    <auro-menuoption value="sjo" id="airport-sjo" suggest="sjo san jose alajuela province">juan santamaria international</auro-menuoption>
    <auro-menuoption value="las" id="airport-las" suggest="las nevada las vegas">harry reid international airport</auro-menuoption>
    <auro-menuoption value="lih" id="airport-lih" suggest="lih hawaii kauai">lihue international</auro-menuoption>
    <auro-menuoption value="mso" id="airport-mso" suggest="mso montana missoula">missoula international</auro-menuoption>
    <auro-menuoption value="alw" id="airport-alw" suggest="alw washington walla walla">walla walla regional</auro-menuoption>
    <auro-menuoption value="mke" id="airport-mke" suggest="mke wisconsin milwaukee">milwaukee mitchell international</auro-menuoption>
    <auro-menuoption value="eug" id="airport-eug" suggest="eug oregon eugene">mahlon sweet field</auro-menuoption>
    <auro-menuoption value="akn" id="airport-akn" suggest="akn alaska king salmon">king salmon</auro-menuoption>
    <auro-menuoption value="cun" id="airport-cun" suggest="cun quintana roo cancun">cancun international</auro-menuoption>
    <auro-menuoption value="rdd" id="airport-rdd" suggest="rdd california redding">redding municipal airport</auro-menuoption>
    <auro-menuoption value="mco" id="airport-mco" suggest="mco florida orlando">orlando international</auro-menuoption>
    <auro-menuoption value="slc" id="airport-slc" suggest="slc utah salt lake city">salt lake city international</auro-menuoption>
    <auro-menuoption value="phx" id="airport-phx" suggest="phx arizona phoenix">sky harbor international</auro-menuoption>
    <auro-menuoption value="bil" id="airport-bil" suggest="bil montana billings">billings logan international</auro-menuoption>
    <auro-menuoption value="gst" id="airport-gst" suggest="gst alaska gustavus">gustavus</auro-menuoption>
    <auro-menuoption value="adk" id="airport-adk" suggest="adk alaska adak">adak</auro-menuoption>
    <auro-menuoption value="cvg" id="airport-cvg" suggest="cvg kentucky hebron">cincinnati northern kentucky international</auro-menuoption>
    <auro-menuoption value="jac" id="airport-jac" suggest="jac wyoming jackson">jackson hole airport</auro-menuoption>
    <auro-menuoption value="cmh" id="airport-cmh" suggest="cmh ohio columbus">john glenn columbus international</auro-menuoption>
    <auro-menuoption value="yyj" id="airport-yyj" suggest="yyj british columbia victoria">victoria international</auro-menuoption>
    <auro-menuoption value="chs" id="airport-chs" suggest="chs south carolina charleston">charleston international</auro-menuoption>
    <auro-menuoption value="iah" id="airport-iah" suggest="iah texas houston">george bush intercontinental</auro-menuoption>
    <auro-menuoption static nomatch>Unknown airport... </auro-menuoption>
  </auro-menu>
</auro-combobox>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Example with checkmark for selected option

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/withCheckmark.html) -->
  <!-- The below content is automatically added from ./../apiExamples/withCheckmark.html -->
  <auro-combobox checkmark>
      <span slot="bib.fullscreen.headline">Bib Header</span>
      <span slot="label">Name</span>
      <auro-menu>
          <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
          <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
          <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
          <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
          <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
          <auro-menuoption static nomatch>No matching option</auro-menuoption>
      </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/withCheckmark.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/withCheckmark.html -->

```html
<auro-combobox checkmark>
    <span slot="bib.fullscreen.headline">Bib Header</span>
    <span slot="label">Name</span>
    <auro-menu>
        <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
        <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
        <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
        <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
        <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
        <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
</auro-combobox>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Using the type attribute

The `type` attribute may be used to apply the corresponding `type` attribute on [auro-input](http://auro.alaskaair.com/components/auro/input/api).

`type="credit-card"` is not currently supported.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/typeMonthDayYear.html) -->
  <!-- The below content is automatically added from ./../apiExamples/typeMonthDayYear.html -->
  <auro-combobox type="date" triggerIcon>
    <span slot="bib.fullscreen.headline">Date Combobox Header</span>
    <span slot="label">Date</span>
    <auro-menu>
      <auro-menuoption value="01/02/2020" id="option-date-0">
        01/02/2020
      </auro-menuoption>
      <auro-menuoption value="05/16/2022" id="option-date-1">
        05/16/2022
      </auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/typeMonthDayYear.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/typeMonthDayYear.html -->

```html
<auro-combobox type="date" triggerIcon>
  <span slot="bib.fullscreen.headline">Date Combobox Header</span>
  <span slot="label">Date</span>
  <auro-menu>
    <auro-menuoption value="01/02/2020" id="option-date-0">
      01/02/2020
    </auro-menuoption>
    <auro-menuoption value="05/16/2022" id="option-date-1">
      05/16/2022
    </auro-menuoption>
  </auro-menu>
</auro-combobox>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Persistent menu option with a custom event

This example demonstrates a static menu option that will always appears regardless of the suggestion filtering performed. In this example "Add new address" will always be a displayed menu option.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/persistent.html) -->
  <!-- The below content is automatically added from ./../apiExamples/persistent.html -->
  <auro-combobox id="persistent">
    <span slot="bib.fullscreen.headline">Address Combobox</span>
    <span slot="label">Address</span>
    <auro-menu id="customEvent">
      <auro-menuoption value="555 Address Way Seattle, WA 99999">555 Address Way Seattle, WA 99999</auro-menuoption>
      <auro-menuoption value="333 Some Street Seattle, WA 99999">333 Some Street Seattle, WA 99999</auro-menuoption>
      <auro-menuoption event="addNewAddress" persistent>Add new address</auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/persistent.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/persistent.html -->

```html
<auro-combobox id="persistent">
  <span slot="bib.fullscreen.headline">Address Combobox</span>
  <span slot="label">Address</span>
  <auro-menu id="customEvent">
    <auro-menuoption value="555 Address Way Seattle, WA 99999">555 Address Way Seattle, WA 99999</auro-menuoption>
    <auro-menuoption value="333 Some Street Seattle, WA 99999">333 Some Street Seattle, WA 99999</auro-menuoption>
    <auro-menuoption event="addNewAddress" persistent>Add new address</auro-menuoption>
  </auro-menu>
</auro-combobox>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>

### Additional Use Case Examples

#### Swapping Values Between Comboboxes

This example illustrates using a JavaScript function attached to an auro-button component click event to swap the values of two `auro-combobox` elements. An example of this use case would be swapping the departure and arrival airports in a flight search form.

<div class="exampleWrapper">
  <!-- AURO-GENERATED-CONTENT:START (FILE:src=./../apiExamples/swapValue.html) -->
  <!-- The below content is automatically added from ./../apiExamples/swapValue.html -->
  <div id="swapExample">
    <auro-combobox id="swapExampleLeft">
      <span slot="bib.fullscreen.headline">Left Combobox Header</span>
      <span slot="label">Name</span>
      <auro-menu>
        <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
        <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
        <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
        <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
        <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
        <auro-menuoption static nomatch>No matching option</auro-menuoption>
      </auro-menu>
    </auro-combobox>
    <auro-button id="swapExampleBtn" iconOnly>
      <auro-icon
        customColor
        category="terminal" 
        name="round-trip-arrows">
      </auro-icon>
    </auro-button>
    <auro-combobox id="swapExampleRight">
      <span slot="bib.fullscreen.headline">Right Combobox Header</span>
      <span slot="label">Name</span>
      <auro-menu>
        <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
        <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
        <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
        <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
        <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
        <auro-menuoption static nomatch>No matching option</auro-menuoption>
      </auro-menu>
    </auro-combobox>
  </div>
  <style>
    #swapExample {
      display: flex;
      flex-direction: row;

      align-items: center;
    }

    #swapExampleLeft,
    #swapExampleRight {
      flex: 1;
    }

    #swapExampleBtn {
      margin: 0 5px;
    }
  </style>
  <!-- AURO-GENERATED-CONTENT:END -->
</div>
<auro-accordion alignRight>
  <span slot="trigger">See code</span>
<!-- AURO-GENERATED-CONTENT:START (CODE:src=./../apiExamples/swapValue.html) -->
<!-- The below code snippet is automatically added from ./../apiExamples/swapValue.html -->

```html
<div id="swapExample">
  <auro-combobox id="swapExampleLeft">
    <span slot="bib.fullscreen.headline">Left Combobox Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
  <auro-button id="swapExampleBtn" iconOnly>
    <auro-icon
      customColor
      category="terminal" 
      name="round-trip-arrows">
    </auro-icon>
  </auro-button>
  <auro-combobox id="swapExampleRight">
    <span slot="bib.fullscreen.headline">Right Combobox Header</span>
    <span slot="label">Name</span>
    <auro-menu>
      <auro-menuoption value="Apples" id="option-0">Apples</auro-menuoption>
      <auro-menuoption value="Oranges" id="option-1">Oranges</auro-menuoption>
      <auro-menuoption value="Peaches" id="option-2">Peaches</auro-menuoption>
      <auro-menuoption value="Grapes" id="option-3">Grapes</auro-menuoption>
      <auro-menuoption value="Cherries" id="option-4">Cherries</auro-menuoption>
      <auro-menuoption static nomatch>No matching option</auro-menuoption>
    </auro-menu>
  </auro-combobox>
</div>
<style>
  #swapExample {
    display: flex;
    flex-direction: row;

    align-items: center;
  }

  #swapExampleLeft,
  #swapExampleRight {
    flex: 1;
  }

  #swapExampleBtn {
    margin: 0 5px;
  }
</style>
```
<!-- AURO-GENERATED-CONTENT:END -->
</auro-accordion>
