This export contains the following U.S. General Soil Map data:

Spatial Extent:         Virginia
SSA Symbol:             US
SSA Name:               United States
SSA Version:            2
SSA Version Est.:       7/6/2006 8:49:17 AM
Spatial Format:         ArcView Shapefile
Coordinate System:      Geographic Coordinate System (NAD83)


The export also contains the following MS Access SSURGO template 
database:

Template DB Name:       soildb_US_2002.mdb
Template DB Version:    33.1
Template DB State:      US
MS Access Version:      Access 2002


U.S. GENERAL SOIL MAP DATA PACKAGING AND ORGANIZATION

When U.S. General Soil Map data is exported from the Soil Data Mart, 
the end result is always a single zip file whose name is in the form 
gsmsoil_spatialextentabbreviation.zip.  Although the survey area symbol 
for U.S. General Soil Map data will always be "US", you can request 
U.S. General Soil Map data for either the entire US or for only a 
particular US state or territory.  The spatial extent of an order is 
reflected in the spatial extent abbreviation, which will always be 
either "US" or a U.S. state or territory code.

The export file can be unzipped using WinZip or an equivalent 
application.  When an export file is unzipped, the following directory 
hierarchy is produced in the directory to which the export file was 
unzipped:

gsmsoil_spatialextentabbreviation
    tabular
    spatial

where spatialextentabbreviation will always be either "US" or a U.S. 
state or territory code.

The top level directory contains the following files:

soil_metadata_spatialextentabbreviation.txt - Federal Geographic Data 
Committee (FGDC) metadata in plain ASCII format.

soil_metadata_spatialextentabbreviation.xml - the same FGDC metadata in 
XML format.

readme.txt - this file

For orders placed via the Soil Data Mart, the root directory will also 
contain a zipped, empty MS Access SSURGO template database.  This will 
be a copy of the most current national SSURGO template database, for a 
relatively current version of MS Access.  The name of this zip file 
will be something like "soildb_US_2002.zip".  The number in this file 
name reflects the MS Access version of the embedded MS Access database.  
For orders placed via the Geospatial Data Gateway, no SSURGO template 
database will be automatically included.

Directory "tabular" contains the tabular data for this order.

Directory "spatial" contains the spatial data for this order.

An order for U.S. General Soil Map data will always include both 
tabular and spatial data.

U.S GENERAL SOIL MAP TABULAR DATA

Tabular data is provided as a set of ASCII delimited files.  Each file 
corresponds to table in the SSURGO data model.  The tabular data isn't 
particularly useful until it has been imported into an MS Access SSURGO 
template database.  For orders placed via the Soil Data Mart, a copy of 
the most current national SSURGO template database, for a relatively 
current version of MS Access, is automatically included in every export 
of U.S. General Soil Map data.  For orders placed via the Geospatial 
Data Gateway, or if you need to obtain a SSURGO template database for a 
different MS Access version, or for a particular state, SSURGO template 
databases can be downloaded on demand from the following URL:

http://soildatamart.nrcs.usda.gov/templates.aspx

A brief aside:  U.S. General Soil Map data is not the same as SSURGO 
data.  U.S. General Soil Map data is mapped at a much smaller scale 
then SSURGO data, but both of datasets are delivered in the same 
format, which is referred to as "SSURGO format", and both datasets can 
be imported into a SSURGO template database because both datasets share 
the same underlying data model.  Additional information about the 
SSURGO data model can be obtained from the SSURGO Metadata reports in 
the MS Access SSURGO template database, or from the Soil Data Mart 
website at:

http://soildatamart.nrcs.usda.gov/ssurgometadata.aspx

For information about importing tabular data into a template database, 
or information about the capabilities of the template database in 
general, do the following:

1.  Open the MS Access SSURGO template database in the appropriate 
version of MS Access.

2.  Click the Reports tab of the Database Window.  The Database Window 
may be behind a form titled "SSURGO Import" or "Soil Reports".

3.  Either double-click the report titled "How to Understand and Use 
this Database", or select this report and then click "Preview".

4.  After the Report Viewer window is displayed, either click the 
printer icon or select "Print" from the File menu.  You can also browse 
this report using the Preview window.

There are two things you need to keep in mind when it comes to 
importing tabular data for the U.S. General Soil Map into a SSURGO 
template database:

1.  Although the entire U.S. General Soil Map tabular dataset can be 
imported into a SSURGO template database, this data is going to take up 
more than half of the maximum allowable size of an MS Access database, 
which is 2 gigabytes.  Performance is going to be poor, and in order to 
generate a soil report, you are going to have select a reasonably sized 
subset of map units.

2.  In general you are not going to be able to import data for two 
different non-national spatial extents into the same database due to 
key conflicts.

U.S GENERAL SOIL MAP SPATIAL DATA

U.S. General Soil Map spatial data is only available in Shape File 
format, in geographic coordinates.  Unlike SSURGO where a variety of 
required and optional feature classes are provided, only a single 
required feature class is provided for U.S. General Soil Map data.  
Only a map unit polygon feature class is provided, and the names of the 
files corresponding to that feature class all begin with 
"gsmsoilmu_a_spatialformatabbreviation", where spatial format 
abbreviation is always either "US" or a U.S. state or territory code.

OBTAINING ADDITIONAL HELP

Questions should be directed to the National Soil Information System 
(NASIS) Hotline.  The NASIS Hotline, which resides at the USDA NRCS 
National Soil Survey Center in Lincoln Nebraska, is staffed from 8:00 
AM to 4:30 PM Central Time.

(402) 437-5378 - Steve Speidel
(402) 437-5379 - Tammy Cheever

e-mail:  hotline@lin.usda.gov


