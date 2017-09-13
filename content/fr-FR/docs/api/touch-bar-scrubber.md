## Classe : TouchBarScrubber

> Create a scrubber (a scrollable selector)

Processus : [Main](../tutorial/quick-start.md#main-process)

### `new TouchBarScrubber(options)` *Experimental*

* `options` Object 
  * `items` [ScrubberItem[]](structures/scrubber-item.md) - An array of items to place in this scrubber
  * `select` Function - Called when the user taps an item that was not the last tapped item 
    * `selectedIndex` Integer - The index of the item the user selected
  * `highlight` Function - Called when the user taps any item 
    * `highlightedIndex` Integer - The index of the item the user touched
  * `selectedStyle` String - Selected item style. Defaults to `null`.
  * `overlayStyle` String - Selected overlay item style. Defaults to `null`.
  * `showArrowButtons` Boolean - Defaults to `false`.
  * `mode` String - Defaults to `free`.
  * `continuous` Boolean - Defaults to `true`.

### Propriétés d'instance

Les propriétés suivantes sont disponibles pour les instances de `TouchBarScrubber` :

#### `touchBarSegmentedControl.items`

A `ScrubberItem[]` array representing the items in this scrubber. Updating this value immediately updates the control in the touch bar. Updating deep properties inside this array **does not update the touch bar**.

#### `touchBarSegmentedControl.selectedStyle`

A `String` representing the style that selected items in the scrubber should have. Updating this value immediately updates the control in the touch bar. Possible values:

* `background` - Maps to `[NSScrubberSelectionStyle roundedBackgroundStyle]`
* `outline` - Maps to `[NSScrubberSelectionStyle outlineOverlayStyle]`
* `null` - Actually null, not a string, removes all styles

#### `touchBarSegmentedControl.overlayStyle`

A `String` representing the style that selected items in the scrubber should have. This style is overlayed on top of the scrubber item instead of being placed behind it. Updating this value immediately updates the control in the touch bar. Possible values:

* `background` - Maps to `[NSScrubberSelectionStyle roundedBackgroundStyle]`
* `outline` - Maps to `[NSScrubberSelectionStyle outlineOverlayStyle]`
* `null` - Actually null, not a string, removes all styles

#### `touchBarSegmentedControl.showArrowButtons`

A `Boolean` representing whether to show the left / right selection arrows in this scrubber. Updating this value immediately updates the control in the touch bar.

#### `touchBarSegmentedControl.mode`

A `String` representing the mode of this scrubber. Updating this value immediately updates the control in the touch bar. Possible values:

* `fixed` - Maps to `NSScrubberModeFixed`
* `free` - Maps to `NSScrubberModeFree`

#### `touchBarSegmentedControl.continuous`

A `Boolean` representing whether this scrubber is continuous or not. Updating this value immediately updates the control in the touch bar.