# Notes
* Current project files under `Hardware` folder
* Some resistors and capacitors (imported from the photon) don't have a "box" silkscreen in their footprint - for the final batch, these footprints are better omitted.
* RF components have been placed using the photon as reference
  * (X,Y) coords for RF components have been taken from reference design then moved as a group to maintain relative positioning
* (X,Y) coords for the remaining major components can be referenced from V2
* Make sure to use the 4-layer DRC from spark (under photon\cam-drc\spark-4layer.dru)
* Keep all traces at **12mils** unless absolutely needed

# To-Do
* Change MEMs mic to Condenser mic
* Ground plane vias for RF
* Determine good location for RGB LED
* Copy keepout & fill polygons from V2.2 and photon reference
* Source a SMT LDR?
* All remaining RLC footprints can be replaced with the footprints used by spark, or the master library can be updated

* Possibly shorten overall length of sensor -> if all components fit

# General Guide
* Don't commit library, board and schematic backup files auto generated by Eagle (should be taken care of, by the included .gitignore file, but just fyi)
* Look at V2.2 & photon for reference (Under reference drawings folder)
* Make sure you set your library path to the `Libraries` folder under `Options->Directories` in Eagle
