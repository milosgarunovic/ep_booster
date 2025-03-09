# Checklist

## Schematic design

- [x] Setup
    - [x] Set grid
    - [x] Page settings (TODO revise date on date of release)
- [x] Symbols
    - [x] Add symbols to the sheet
    - [x] Create symbols if needed
    - [x] Add values to symbols (Component values)
- [x] Arrange, annotate, associate
    - [x] Arrange symbols in functional blocks
    - [x] Annotate symbols
    - [x] Associate with footprints
- [x] Wire
    - [x] Signals
    - [x] Power (PWR_FLAG)
- [x] Nets
    - [x] Set net names
- [x] Electrical Rules Check
    - [x] Run ERC
    - [x] Fix errors
    - [x] Repeat ERC
- [x] Comments
    - [x] Add text information (group component in boxes, add comments)
    - [x] Add graphics

## Layout design

- [x] Setup
    - [x] Set grid
    - [x] Set design rules (check manufacturer for constraints for minimum values)
    - [x] Import footprints from schematic
- [x] Outline and constrains
    - [x] Define size and shape (Edge.Cuts layer), remember to round the edges at the end
    - [x] Define mounting holes
    - [x] Define cutouts
- [x] Footprints
    - [x] Place components on board
    - [x] Arrange user interface components
    - [x] Arrange in functional blocks
    - [x] Complete placement
- [x] Route
    - [x] Critical traces
    - [x] Power
    - [x] Copper fills
    - [x] Everything else
- [x] Silkscreen (F.Silkscreen and B.Silkscreen layers)
    - [x] Add text information (reference designators, functionality text (boost, gain, bright...))
    - [x] Add graphics (name, personal logo/name, version)
- [x] Design rules check
    - [x] Run DRC
    - [x] Fix errors
    - [x] Repeat DRC
- [ ] Export & Manufacture
    - [ ] Update date of manufacturing variable (${MANUFACTURING_DATE})
    - [ ] Create Gerber files
    - [ ] Verify Gerber files
    - [ ] Upload Gerber files to manufacturer