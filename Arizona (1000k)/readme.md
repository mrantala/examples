# Geologic Map of Arizona at 1:1,000,000-scale

This folder contains

- __GeoJSON Files__ representing geologic features in an [NCGMP09](http://ncgmp09.github.io)-style format:
    - __ContactsAndFaults.geojson__ [_view_](ContactsAndFaults.geojson) | [_download_](http://ncgmp09.github.io/examples/Arizona-1000k/ContactsAndFaults.geojson)
    - __MapUnitPolys.geojson__ [_view_](MapUnitPolys.geojson) | [_download_](http://ncgmp09.github.io/examples/Arizona-1000k/MapUnitPolys.geojson)
    - __OtherLines.geojson__ [_view_](OtherLines.geojson) | [_download_](http://ncgmp09.github.io/examples/Arizona-1000k/OtherLines.geojson)
    
- __CSV Files__ for a quick look at the attribute tables for the above GeoJSON files
    - __ContactsAndFaults.csv__ [_view_](ContactsAndFaults.csv) | [_download_](http://ncgmp09.github.io/examples/Arizona-1000k/ContactsAndFaults.csv)
    - __MapUnitPolys.csv__ [_view_](MapUnitPolys.csv) | [_download_](http://ncgmp09.github.io/examples/Arizona-1000k/MapUnitPolys.csv)
    - __OtherLines.csv__ [_view_](OtherLines.csv) | [_download_](http://ncgmp09.github.io/examples/Arizona-1000k/OtherLines.csv)

- __TopoJSON Files__ these compressed, topologically aware files can be viewed directly on GitHub
    - __AllFeatures.topojson__ [_view_](AllFeatures.topojson) | [_download_](http://ncgmp09.github.io/examples/Arizona-1000k/AllFeatures.topojson): This single file encapsulates all of the geographic data from the three GeoJSON files.
    - __ContactsAndFaults.topojson__ [_view_](ContactsAndFaults.topojson) | [_download_](http://ncgmp09.github.io/examples/Arizona-1000k/ContactsAndFaults.topojson)
    - __MapUnitPolys.topojson__ [_view_](MapUnitPolys.topojson) | [_download_](http://ncgmp09.github.io/examples/Arizona-1000k/MapUnitPolys.topojson)
    - __OtherLines.topojson__ [_view_](OtherLines.topojson) | [_download_](http://ncgmp09.github.io/examples/Arizona-1000k/OtherLines.topojson)

- __CSV Files__ for each of the following tables which contain information related to the above features:
    - __DataSources.csv__ [_view_](DataSources.csv) | [_download_](http://ncgmp09.github.io/examples/Arizona-1000k/DataSources.csv)
    - __DescriptionOfMapUnits.csv__ [_view_](DescriptionOfMapUnits.csv) | [_download_](http://ncgmp09.github.io/examples/Arizona-1000k/DescriptionOfMapUnits.csv)
    - __ExtendedAttributes.csv__ [_view_](ExtendedAttributes.csv) | [_download_](http://ncgmp09.github.io/examples/Arizona-1000k/ExtendedAttributes.csv)
    - __GeologicEvents.csv__ [_view_](GeologicEvents.csv) | [_download_](http://ncgmp09.github.io/examples/Arizona-1000k/GeologicEvents.csv)
    - __Glossary.csv__ [_view_](Glossary.csv) | [_download_](http://ncgmp09.github.io/examples/Arizona-1000k/Glossary.csv)

- __An HTML File__: 
    - __index.html__ [_view_](http://ncgmp09.github.io/examples/Arizona-1000k/): presents a browsable map of the data contained in this folder.
    
_Please note:_ while GitHub is capable of visualizing `.csv`, `.geojson` and `.topojson` files, many of the files in this repository are too big for GitHub's system. These files can be viewed in a variety of other applications. Generally, you will be able to look at the `.topojson` files, but not the `.geojson` ones. Some of the `.csv` files are too large to view as well.

_Also_: while these files roughly obey the [NCGMP09 database standard](http://ncgmp09.github.io), they are not perfect, and are under-construction. For more information about what the attributes of the data mean, please read [the documentation available online](http://ncgmp09.github.io/core-content.html)
