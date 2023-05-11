
# Sample metadata submission sheets

Sample metada submission file (Sample_metadata_submission/Sample_submission_sheet.xlsx)

Contains:
- Metadata sheets for sample types: `Soil`, `Sediment`, `Fresh Water`, `Coastal Water`, `Pelagic Water` and `Host`. 
- A sheet containing a copy of the Controlled Vocab used in specific fields is provided for reference, the controlling version of this document is found at https://github.com/AusMicrobiome/contextualdb_doc/tree/main/db_schema_definitions/db_schema_definitions.xlsx
- A README_vx.x.x sheet contains instructions on how to use the submission sheets.

**Version history**

**3.1.0**
- New fields added to `Coastal Water` and `Pelagic Water` sheets
    - `Part_org_carb_(μmol/L)`

    - `Part_org_carb_method`

**3.0.0**
- Submission sheets are compatible with version 4.0.0 of the contextual database:
https://github.com/AusMicrobiome/contextualdb_doc/raw/4.0.0/db_schema_definitions/db_schema_definitions.xlsx
- `Fresh Water` sheet modified to align the units of some columns with Marine database fields. Added information on unit conversion factors for data obtained from CSBP lab analysis to column headers. Note: `\n` in field name represents a Line Feed/Newline.

    - New fields added to `Fresh Water` sheet:
        - `Bicarbonate_(mg/L)`
        - `Bicarbonate_method`
        - `Carbonate_(mg/L)`
        - `Carbonate_method`
        - `Ammonium_nitrogen_(umol/l N)\n*CSBP conversion: (CSBP_value*1000)/14.006720`
        - `Ammonium_nitrogen_(umol/l N)_method`

   - Changed field names on `Fresh Water` sheet
     - `Nitrate_nitrogen_(mg/kg)` to `Nitrate_nitrogen_(umol/l N)\n*CSBP conversion: (CSBP_value*1000)/14.006720`
     - `Nitrate_nitrogen_method` to `Nitrate_nitrogen_(umol/l N)_method`
     - `Conductivity_(dS/m)` to `Conductivity_(S/m)\n*CSBP conversion: CSBP_value*10`
     - `Conductivity_method(dS/m)` to `Conductivity_(S/m)_method`

   - Deleted fields from `Fresh Water` analysis sheet
     - `Carbonate/bicarbonate_(mg/L)`
     - `Carbonate/bicarbonate_method`

 - New fields added to `Coastal Water` and `Pelagic Water` sheets
    - `Picoeukaryotes_(cells_per_ml)`
    - `Picoeukaryotes_method`
    - `Prochlorococcus_(cells_per_ml)`
    - `Prochlorococcus_method`
    - `Synechococcus_(cells_per_ml)`
    - `Synechococcus_method`

- Added information to the `README_v3.0.0` sheet describing the process for submitting CSBP analysis sheets directly to the AM.

**2.0.0**
  - Added fields for:
    - `Hyperspectral_analysis`
    - `Hyperspectral_analysis_method`

**1.0.0**

Initial commit of Sample_submission_sheet.xlsx
- Submission sheets are compatible with version 3.1 of the contextual database: https://github.com/AusMicrobiome/contextualdb_doc/raw/3.1.2/db_schema_definitions/db_schema_definitions.xlsx
- An additional field ` Collection_permit` has been included for forward compatibility to meet upcoming contextual database updates.
