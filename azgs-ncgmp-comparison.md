# Discrepency between AZGS Tools and NCGMP09 Definition

The AZGS developed tools to assist geologists in the creation of geologic maps in NCGMP09 databases early in the process of the development of that standard. Due to subsequent changes and some minor misinterpretation on the AZGS's part have led to some discrepencies between the databases being developed and populated at the AZGS and the definition of the NCGMP09 database scheme in USGS OFR2010-1335.

## Feature Datasets
OFR2010-1335 has a single feature dataset for all Geologic data related to the map; AZGS scheme puts station-related data in a separate feature dataset. This should have no significant impact?

## Mandatory Tables and feature classes

### MapUnitPolys
- `RuleID` not included in AZGS implementation ("If Cartographic Representations are used, this field is required; otherwise it is not included in the table" OFR2010-1335, p. 109). Instead... 

### ContactsAndFaults
- `Symbol` implemented as Long Integer and functions as RuleID in ESRI geodatabase; ContactAndFaults table in OFR2010-1335 does not specify a data type for the `Symbol` field, so it defaults to type=string (OFR2010-1335, p. 103);
- `RuleID` field not included in AZGS implementation; 
- `IsConcealed` is, according to OFR2010-1335, a text field with domain {'N', 'Y'}. It is implemented in the AZGS tools as a short integer with an ESRI domain that maps 0='No', 1='Yes'. This allows ArcGIS to recognize the field as a "subtype", and therefore, the field can be used to constrain Topology rules.

### DataSourcePoly
- No differences. 

### DescriptionOfMapUnits
- `GeneralLithology` is named `GeneralLithologyTerm`; 
- `Symbol` field is absent.

### DataSources
- No differences.

### Glossary
- No differences.

## AS NEEDED Tables and feature classes

### CartographicLines
- No `RuleID`, see above.

### Point feature class properties

- __Samples__ 
    - Missing `MapUnit`; 
    - Missing `LocationSourceID`, contains `DataSourceID`;
    - No sample fields included (`FieldSampleID`, `AlternateSampleID`, `MaterialAnalyzed`)

- __OrientationPoints__
    - Missing `MapUnit`; 
    - Missing `LocationSourceID`, contains `DataSourceID`;
    - `Symbol` is implemented as Long integer and used as the `RuleID` for ESRI Geodatabase;

- __Stations__
    - Missing `MapUnit`; 
    - `ObservedMapUnit` is not in table but is nilable; 
    - Missing `LocationSourceID`, contains `DataSourceID`;
    - Primary key field called `StationPoint_ID` instead of `Stations_ID`.
    
- __GeologicLines__
    - Table called _OtherLines_ in AZGS tools;
    - Missing `IsConcealed`;
    - `RuleID` is renamed `Symbol`.
    
- __OtherPolys__
    - Table called _OverlayPolys_ in AZGS tools;
    - Primary key change from `OverlayPoly_ID` to `OtherPolys_ID`;
    - Missing `Type` field - instead contains `MapUnit`, a foreign key to DescriptionOfMapUnits.
