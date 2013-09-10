# Geologic Map of Arizona at 1:1,000,000-scale

This folder contains

- __GeoJSON Files__ representing geographic features from an NCGMP09-style database:
    - `ContactsAndFaults`
    - `MapUnitPolys`
    - `OtherLines`
    
- __CSV Files__ for a quick look at the attribute tables for the above GeoJSON files

- __A TopoJSON File__: This single file (`AllFeatures.topojson`) encapsulates all of the geographic data from the three GeoJSON files into one, compressed file.

- __CSV Files__ for each of the following tables:
    - `DataSources`
    - `DescriptionOfMapUnits`
    - `ExtendedAttributes`
    - `GeologicEvents`
    - `Glossary`

_Please note:_ while GitHub is capable of visualizing `.csv`, `.geojson` and `.topojson` files, many of the files in this repository are too big for GitHub's system. These files can be viewed in a variety of other applications. 

- __An HTML File__: `index.html` can either be downloaded and opened directly from the file on your computer, or viewed here: http://ncgmp09.github.io/examples/Arizona%20(1000k)/