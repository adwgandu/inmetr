# inmetr 0.3.0

News
================

<!-- NEWS.md is generated from NEWS.Rmd. Please edit that file -->
inmetr 0.2.8.9999
=================

-   \[ \] add function to compute mean daily data.
-   \[ \] remove stations not available in BDMEP\[\] (although they still are in `bdmep_meta()`).
-   \[ \] check if stations in [climatology 1981-2010](http://www.inmet.gov.br/portal/index.php?r=clima/normaisClimatologicas) are available in BDMEP.

inmetr 0.2.8
============

-   \[x\] improve arguments check for `sdate` and `edate` arguments in `bdmep_import()`. Now, whitespace are removed from start and end of those arguments before building the url string to BDMEP. Thanks to @danielalthoff for reporting your case.

inmetr 0.2.7
============

-   \[x\] fix issue related to station MACAPA - AP (OMM: 82098), thanks to William Barbosa (ESALQ/USP).
-   \[x\] split up bdmep\_import in `bdmep_write_csv()` and `bdmep_data_status()`

inmetr 0.2.6.9999
=================

-   \[x\] fix issue \#3, thanks to @DominickAugustine
-   \[x\] add function to write csv files of station data.
-   \[x\] include `bdmep_meta()`.

inmetr 0.2.5
============

-   \[x\] include metadata of 394 meteorological stations as a dataset named `bdmep_meta`.
-   \[x\] Functions (see below) were renamed to have consistent names. Now all functions have a 'bdmep' prefix. This allows you to type the prefix and see all the members of bdmep's family functions.
    -   `import_bdmep` changes to `bdmep_import`
    -   `data_description` changes to `bdmep_description`
-   \[x\] `bdmep_import()` changes:
    -   supports a vector of stations IDs allowing to data import from multiple meteorological stations.
    -   returned data frame include a new column `request status` (character) to inform on the outcome of the execution of the request on the server.

inmetr 0.0.3
============

-   \[x\] fixed issue (\#1, @sillasgonzaga).

-   \[x\] `import_bmep()` has a new argument `verbose` to print if the status of connection is ok.
