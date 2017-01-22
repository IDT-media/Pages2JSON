# Pages2JSON
Module for ProcessWire that adds capability to output pages as JSON

# Changelog
Lisa Simpson (0.0.4)
* Removed template tab and added section under Basic tab for template spesific JSON attribute output selection.
* Crawler is now targeting Pages and WireArrays based on instance type, not className like it was previously. This should give more flexibility to developers around different types of objects that are derived from either of.
* Added only public method it most likely ever will have: encode($value, $options = 0). Usage example: $modules('Pages2JSON')->encode($toJSON);
* Added new hookable method: getFields($page). Gives capability to inject and manipulate runtime fields to be crawled. Useful especially if you need to inject field that dosen't exists, but you still need crawler to notice it.

Montgomery Burns (0.0.3)
* Kind of forgot to release this, so this remains ghots release that never happen. And to be honest, no one really likes Mr. Burns anyways.

Homer Simpson (0.0.2)
* Allows user define global data output in module options + individual data based on template.
* Added forum user Manol's feature request regarding PageImage and PageFile fields.

Bart Simpson (0.0.1)
* Initial release
