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

- [ ] Setup
    - [ ] Set grid
    - [ ] Set design rules (check manufacturer for constraints for minimum values)
    - [ ] Import footprints from schematic
- [ ] Outline and constrains
    - [ ] Define size and shape (Edge.Cuts layer)
    - [ ] Define mounting holes
    - [ ] Define cutouts
- [ ] Footprints
    - [ ] Place components on board
    - [ ] Arrange user interface components
    - [ ] Arrange in functional blocks
    - [ ] Complete placement
- [ ] Route
    - [ ] Critical traces
    - [ ] Power
    - [ ] Copper fills
    - [ ] Everything else
- [ ] Silkscreen
    - [ ] Add text information
    - [ ] Add graphics
- [ ] Design rules check
    - [ ] Run DRC
    - [ ] Fix errors
    - [ ] Repeat DRC
- [ ] Export & Manufacture
    - [ ] Create Gerber files
    - [ ] Verify Gerber files
    - [ ] Upload Gerber files to manufacturer