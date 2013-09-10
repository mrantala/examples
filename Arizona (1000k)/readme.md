# Geologic Map of Arizona at 1:1,000,000-scale

This folder contains

- __GeoJSON Files__ representing geographic features from an NCGMP09-style database:
    - `ContactsAndFaults.geojson`
    - `MapUnitPolys.geojson`
    - `OtherLines.geojson`
    
- __CSV Files__ for a quick look at the attribute tables for the above GeoJSON files

- __TopoJSON Files__ these compressed, topologically aware files can be viewed directly on GitHub
    - `AllFeatures.topojson`: This single file encapsulates all of the geographic data from the three GeoJSON files.
    - `ContactsAndFaults.topojson`
    - `MapUnitPolys.topojson`
    - `DataSources.topojson`

- __CSV Files__ for each of the following tables:
    - `DataSources.csv`
    - `DescriptionOfMapUnits.csv`
    - `ExtendedAttributes.csv`
    - `GeologicEvents.csv`
    - `Glossary.csv`

- __An HTML File__: `index.html` can either be downloaded and opened directly from the file on your computer, or viewed here: http://ncgmp09.github.io/examples/Arizona%20(1000k)/

_Please note:_ while GitHub is capable of visualizing `.csv`, `.geojson` and `.topojson` files, many of the files in this repository are too big for GitHub's system. These files can be viewed in a variety of other applications. 