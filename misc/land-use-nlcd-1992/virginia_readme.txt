National Land Cover Data 
Virginia

Version 05-27-99
(Updated: January, 1996; February, 1997; July, 1998; January, 1999; 
          May, 1999; March, 2000; April 2000)


Introduction

This land cover data set was produced as part of a cooperative project
between the U.S. Geological Survey (USGS) and the U.S. Environmental
Protection Agency (USEPA) to produce a consistent, land cover data layer
for the conterminous U.S. based on 30-meter Landsat thematic mapper (TM)
data.  National Land Cover Data (NLCD) was developed from TM data
acquired by the Multi-resoultion Land Characterization (MRLC) Consortium. 
The MRLC Consortium is a partnership of federal agencies that produce or
use land cover data.  Partners include the USGS (National Mapping,
Biological Resources, and Water Resources Divisions), USEPA, the U.S.
Forest Service, and the National Oceanic and Atmospheric Administration. 


Virginia

The Virginia NLCD set was produced as part of a project area encompassing
portions of Federal Region III, including the states of Delaware, Maryland,
Pennsylvania, Virginia, West Virginia, and the District of Columbia.  This
data set was produced under the direction of the MRLC Regional Land
Cover Characterization Project of the USGS EROS Data Center (EDC),
Sioux Falls, SD. Questions about the data set can be directed to the MRLC
Regional Team at (605) 594-6114 or mrlc@edcmail.cr.usgs.gov.   


Version/Revisions:

1st Draft - Completed 96-01

Version 97-02 Edits
 -- The hay/pasture/grass class (initial version) was split into hay/pasture and   
    "other grasses" (parks/golf courses, etc). 
 -- The high intensity developed class (initial version) was split into high     
    intensity commercial/industrial and high intensity residential.
 -- The data set was edge-matched with a Region 4 land cover data set.

Version 98-07 Edits
 -- Initial masking and distribution of the state of Virginia.  The mask      
    boundaries are the minimum bounding rectangle for the state of Virginia.
 -- Adjustments were made to the agricultural classes, specifically to fine-tune 
    the hay/pasture and row crop classes.

Version 99-01 Edits
 -- More refinements made to agricultural classes (in southwest corner of      
    state), specifically to fine-tune the hay/pasture and row crop classes.

Version 99-05 Edits
 -- Additional 300 meters of data (10 pixels) added beyond the Virginia 
    border to facilitate creation of multi-state mosaics.

Version 2000-03  Edits

The following processing steps were taken to eliminate about 20 pixels
of zero data values found sprinkled through the state. The origin
of the zero data is not known but one theory is that they are a result 
of the modelling process to split confused classes.  If a possible
model combination was not taken into account, the model returned a
value of zero.  The zero data values were eliminated using a 3x3 
majority filter.  It was constrained to only work on zero values and
to ignore zeros when determining the majority value.
          
Version 2000-04  Edits
 -- Adjustments were made to the relative amounts of hay/pasture and row 
    crops in the Coastal Plain region based upon crop statistics reported in
    the 1992 US Department of Commerce Census of Agriculture.  The Coastal
    Plain region of Virgina now has less hay pasture and more row crops.


Projection Information:

The initial Landsat TM mosaics, all ancillary data sets, and the land cover
product are all map-registered to an Albers Conical Equal Area projection. 
The following represents projection information for the final land cover
product for the state of Virginia. 

      Projection: Albers Conical Equal Area
           Datum: NAD83
           Spheroid: GRS80
           Standard Parallels: 29.5 degrees North Latitude       
                               45.5 degrees North Latitude       
      Central Meridian:  96 degrees  West Longitude
      Origin of the Projection: 23 degrees North Latitude   
      False Easting:   0 meters
      False Northing:  0 meters

Number of Lines (rows):  13032                          
Number of Samples (columns):  23630  
Number of Bands: 1   Pixel size: 30 X 30 meters
Projection Coordinates (center of pixel, projection meters)
     Upper Left Corner:  1088700 meters(X),
                         1967100 meters(Y)
     Lower Right Corner:  1797570 meters(X),         
                          1576170 meters(Y) 

NOTE: Each state data set was extracted from the larger regional data set. 
State boundaries from the USGS 1:100,000 Digital Line Graph (DLG) series
were used as the basis for extracting the state data.  In many instances, the
precision of the boundaries in the 1:100,000 DLG data does not match the
spatial precision of the Landsat TM data.  This is most apparent where state
boundaries follow small rivers.  To overcome the possibility of data being
lost in the extraction process, a 300 meter (10 pixel) buffer was added to the
state boundary used to extract the state data. 
     

Data Sources:

The base data set for this project was leaves-on Landsat TM data,
nominal-1992 acquisitions.  Other ancillary data layers included leaves-off
TM, USGS 3-arc second Digital Terrain Elevation Data (DTED) and derived
slope, aspect and shaded relief, Bureau of the Census population and housing
density data, USGS land use and land cover (LUDA), and National Wetlands
Inventory (NWI) data if available. 

     Landsat thematic mapper (TM) scenes:

     Path   Row     Date
     014    034     15-Mar-91
     014    035     13-Oct-92 
     015    033     16-Mar-89 
     015    034     11-Apr-92 
     015    035     20-Oct-92  
     016    033     01-Mar-92  
     016    034     16-Apr-91 
     016    035     01-Mar-92  
     017    033     24-Mar-86 
     017    034     24-Mar-86  
     018    034     29-Nov-93 
     018    035     06-Jun-93
     019    035     23-Apr-92  

     LEAF ON:
     014    034     04-May-91 
     014    035     23-Jun-92         
     015    033     08-May-90  
     015    034     17-Jun-93 
     015    035     16-May-93
     016    033     28-Sep-93  
     016    034     28-Sep-93 
     017    033     02-Oct-92 
     017    034     02-Oct-92   
     017    035     03-Nov-92 
     018    034     29-Sep-94  
     018    035     25-Oct-92  
     019    035     12-Nov-90 
     019    035     30-Sep-92 


Caveats and Concerns:
  
     While we believe that the approach taken has yielded a very good general
land cover classification product for a very large region, it is important to
indicate to the user where there might be some potential problems.  The
biggest concerns are listed below:

1)  Quantitative accuracy checks have yet to be conducted.  We plan to make
comparisons with existing data sets in order to develop a general overview
regarding the quality of the land cover data set developed.  Feedback from
users of the data will be greatly appreciated.
     
2)  Accurate definition of the transitional barren class was extremely difficult.
The majority of pixels in this class correspond to clear-cut forests in various
stages of regrowth.  Spectrally, fresh clear-cuts are very similar to row-crops
in the leaves-off data.  Manual correction of coding errors was performed to
improve differentiation between row-crops and clear-cuts, but some errors
may still be found.  As regrowth occurs in a clear-cut region, the definition of
transitional barren verses a forested class becomes problematic.  An attempt
was made to classify only fresh clear-cuts or those in the earliest stages of
regrowth, but there are likely forested regions classed as transitional barren
and vice versa.

3)  Due to the confusion between clear-cuts, regrowth in clear-cuts, forested
areas, and shrublands, no attempts were made to populate the shrubland
classes.  Any shrubland areas that exist in this area are classed in their like
forest class, i.e., deciduous shrubland is classed as deciduous forest, etc


Accuracy Assessment:  
   
   Accuracy assessment is pending.
    

21-Class National Land Cover Data Key:

NOTE - All Classes May NOT Be Represented in a specific state data set. 
The class number represents the digital value of the class in the data set.
          

NLCD Land Cover Classification System Key - Rev. July 20, 1999
                         
Water                                        
     11 Open Water
     12 Perennial Ice/Snow

Developed
     21 Low Intensity Residential
     22 High Intensity Residential
     23 Commercial/Industrial/Transportation

Barren
     31 Bare Rock/Sand/Clay
     32 Quarries/Strip Mines/Gravel Pits
     33 Transitional     

Forested Upland 
     41 Deciduous Forest
     42 Evergreen Forest
     43 Mixed Forest

Shrubland
     51 Shrubland

Non-natural Woody
     61 Orchards/Vineyards/Other 

Herbaceous Upland 
     71 Grasslands/Herbaceous

Herbaceous Planted/Cultivated
     81 Pasture/Hay
     82 Row Crops
     83 Small Grains
     84 Fallow
     85 Urban/Recreational Grasses

Wetlands
     91 Woody Wetlands
     92 Emergent Herbaceous Wetlands

                         
NLCD Land Cover Classification System Land Cover Class Definitions

Water - All areas of open water or permanent ice/snow cover.

11.  Open Water - All areas of open water; typically 25 percent or greater
cover of water (per pixel). 
  
12.  Perennial Ice/Snow - All areas characterized by year-long cover of ice
and/or snow.

Developed - Areas characterized by a high percentage (30 percent or greater)
of constructed materials  (e.g. asphalt, concrete, buildings, etc).
  
21.  Low Intensity Residential - Includes areas with a mixture of constructed
materials and vegetation.  Constructed materials account for 30-80 percent of
the cover. Vegetation may account for 20 to 70 percent of the cover.  These
areas most commonly include single-family housing units.  Population
densities will be lower than in high intensity residential areas.

22.  High Intensity Residential - Includes highly developed areas where
people reside in high numbers.  Examples include apartment complexes and
row houses.  Vegetation accounts for less than 20 percent of the cover. 
Constructed materials account for 80 to100 percent of the cover. 
 
23. Commercial/Industrial/Transportation  - Includes infrastructure (e.g.
roads, railroads, etc.) and all highly developed areas not classified as High 
Intensity Residential.
 
Barren - Areas characterized by bare rock, gravel, sand, silt, clay, or other
earthen material, with little or no "green" vegetation present regardless  of its
inherent ability to support life. Vegetation, if present,  is more widely spaced
and scrubby than that in the "green" vegetated categories; lichen cover may be
extensive. 
 
31.  Bare Rock/Sand/Clay - Prennially  barren areas of bedrock, desert 
pavement, scarps, talus, slides, volcanic material, glacial debris, beaches, and
other accumulations of earthen material.

32.  Quarries/Strip Mines/Gravel Pits - Areas of  extractive mining activities
with significant surface expression.

33.  Transitional - Areas of sparse vegetative cover (less than 25 percent of
cover) that are dynamically changing from one land cover to another, often
because of land use activities.  Examples include forest clearcuts, a transition
phase between forest and agricultural land, the temporary clearing of
vegetation, and changes due to natural causes (e.g. fire, flood, etc.).

Forested Upland  - Areas characterized by tree cover (natural or semi-natural
woody vegetation, generally greater than 6 meters tall); tree canopy accounts
for 25-100 percent of the cover.

41.  Deciduous Forest - Areas dominated by trees where 75 percent or more
of the tree species shed foliage simultaneously in response to seasonal
change.
 
42.  Evergreen Forest - Areas dominated by trees where 75 percent or more of
the tree species maintain their leaves all year.  Canopy is never without green
foliage.
       
43.  Mixed Forest - Areas dominated by trees where neither deciduous nor
evergreen species represent more than 75 percent of the cover present. 

Shrubland - Areas characterized by natural or semi-natural woody vegetation
with aerial stems, generally less than 6 meters  tall,  with individuals or
clumps not touching to interlocking.   Both evergreen and deciduous species
of  true shrubs, young trees, and trees or shrubs  that are small or stunted
because of environmental conditions are included. 
 
51.  Shrubland - Areas dominated by shrubs; shrub canopy accounts for
25-100 percent of the cover.  Shrub cover is generally  greater than 25 percent
when tree cover is less than 25 percent.  Shrub cover may be less than 25
percent in cases when the cover of other life forms (e.g. herbaceous or tree) is
less than 25 percent and shrubs cover exceeds the cover of the other life
forms.

Non-natural Woody - Areas dominated by non-natural woody vegetation;
non-natural woody vegetative canopy accounts for 25-100 percent of the
cover.   The non-natural woody classification is subject to the availability of
sufficient ancillary data to differentiate non-natural woody vegetation from 
natural woody vegetation. 

61.  Orchards/Vineyards/Other - Orchards, vineyards, and other areas planted
or maintained for the production of fruits, nuts, berries, or ornamentals. 

Herbaceous Upland - Upland areas characterized by natural or semi-natural
herbaceous vegetation; herbaceous vegetation accounts for 75-100 percent of
the cover.
  
71.  Grasslands/Herbaceous - Areas dominated  by upland grasses and forbs. 
In rare cases, herbaceous cover is less than 25 percent, but exceeds the
combined cover of the woody species present.  These areas are not subject to
intensive management, but they are often utilized for  grazing.

Planted/Cultivated - Areas characterized by herbaceous vegetation that
has been planted or is intensively managed for the production of food, feed,
or fiber; or is maintained in developed settings for specific purposes. 
Herbaceous vegetation accounts for 75-100 percent of the cover.  
         
81.  Pasture/Hay - Areas of grasses, legumes, or grass-legume  mixtures
planted for livestock grazing or the production of seed or hay crops. 
       
82. Row Crops - Areas used for the production of crops, such as corn,
soybeans, vegetables, tobacco, and cotton. 
      
83.  Small Grains - Areas used for the production of graminoid crops such as
wheat, barley, oats, and rice.
        
84.  Fallow - Areas used for the production of crops that are temporarily
barren or with sparse  vegetative cover as a result of  being tilled in a
management practice that incorporates prescribed alternation between
cropping and tillage.

85.  Urban/Recreational Grasses - Vegetation (primarily grasses) planted in
developed settings for recreation, erosion control, or aesthetic purposes. 
Examples include parks, lawns, golf courses, airport grasses, and industrial
site grasses. 
    
Wetlands - Areas where the soil or substrate is periodically saturated with or
covered with water as defined by Cowardin et al.      

91.  Woody Wetlands - Areas where forest or shrubland vegetation accounts
for 25-100 percent of the cover and  the soil or substrate is periodically
saturated with or covered with water.        

92.  Emergent Herbaceous Wetlands - Areas where  perennial herbaceous 
vegetation accounts for 75-100 percent of the cover and the soil or substrate
is periodically saturated with or covered with water.     


General Procedures

Land Cover Characterization:

The project is being carried out on the basis of 10 Federal Regions that make
up the conterminous United States; each region is comprized of multiple
states; each region is processed in subregional units that are limited to the
area covered by no more than 18 Landsat TM scenes. The general NLCD
procedure is to: (1) mosaic subregional TM scenes and classify them using an
unsupervised clustering algorithm, (2) interpret and label the clusters/classes
using aerial photographs as reference data, (3) resolve the labeling of
confused clusters/classes using the appropriate  ancillary data source(s), and
(4) incorporate land cover information from other data sets and perform
manual edits to augment and refine the "basic" classification developed
above. 

Two seasonally distinct TM mosaics are produced, a leaves-on version
(summer) and a leaves-off (spring/fall) version.  TM bands 3 4 5 and 7 are
mosaicked for both the leaves-on and leaves-off versions.  For mosaicking
purposes, a base scene is selected for each mosaic and the other scenes are
adjusted to mimic spectral properties of the base scene using histogram
matching in regions of spatial overlap.

Following mosaicking, either the leaves-off version or leaves-on version is
selected to be the "base" for the land cover mapping process.  The 4 TM
bands of the "base" mosaic are clustered to produce a single 100-class image
using an unspervised clustering algorithm. Each of the spectrally distinct
clusters/classes is then assigned to one or more Anderson level 1 and 2 land
cover classes using National High Altitude Photography program (NHAP)
and National Aeria l Photography program (NAPP) aerial photographs as a
reference.  Almost invariably, individual spectral clusters/classes are
confused between two or more land cover classes.

Separation of the confused spectral clusters/classes into appropriate NLCD
class is accomplished using ancillary data layers.  Standard ancillary data
layers include: the "non-base" mosaic TM bands and 100-class cluster image;
derived TM normalized vegetation index (NDVI), various TM band ratios,
TM date bands; 3-arc second Digital Terrain Elevation Data (DTED) and
derived slope, aspect and shaded relief; population and housing density data;
USGS land use and land cover (LUDA); and National Wetlands Inventory
(NWI) data if available.  Other ancillary data sources may include soils data,
unique state or regional land cover data sets, or data from other federal
programs such as the National Gap Analysis Program (GAP) of the USGS
Biological Resources Division (BRD).  For a given confused spectral
cluster/class, digital values of the various ancillary data layers are compared
to determine: (1) which data layers are the most effective for splitting the
confused cluster/class into the appropriate NLCD class, and (2) the
appropriate layer thresholds for making the split(s).  Models are then
developed using one to several ancillary data layers to split the confused
cluster/class into the NLCD class.  For example, a population density
threshold is used to separate high-intensity residential areas from
commercial/industrial/transportation.  Or a cluster/class might be confused
between row crop and grasslands.  To split this particular cluster/class, a TM
NDVI threshold might be identified and used with an elevation threshold in a
class-spliting model to make the appropriate NLCD class assignments.  A
purely spectral example is using the temporally opposite TM layers to
discriminate confused cluster/classes such as hay pasture vs. row crops and
deciduous forests vs. evergreen forests; simple thresholds that contrast the
seasonal differences in vegetation between leaves-on vs. leaves-off.  

Not all cluster/class confusion can be successfully modeled out.  Certain
classes such as urban/recreational grasses or quarries/strip mines/gravel pits
that are not spectrally unique require manual editing.  These class features are
typically visually identified and then reclassified using on-screen digitizing
and recoding.  Other classes such as wetlands require the use of specific data
sets such as NWI to provide the most accurate classification.  Areas lacking
NWI data are typically subset out and modeling is used to estimate wetlands
in these localized areas.  The final NLCD product results from the
classification (interpretation and labeling) of the 100-class "base"cluster
mosaic using both automated and manual processes, incorporating both
spectral and conditional data layers.  For a more detailed explanation please
see Vogelmann et al. 1998 and Vogelmann et al. 1998.


Accuracy Assessment:

An accuracy assessment is done on all NLCD on a Federal Region basis
following a revision cycle that incorporates feedback from MRLC
Consortium partners and affiliated users.  The accuracy assessments are
conducted by private sector vendors under contract to the USEPA.  A
protocol has been established by the USGS and USEPA that incorporates a
two-stage, geographically stratified cluster sampling plan (Zhu et al., 1999)
utilizing National Aerial Photography Program (NAPP) photographs as the
sampling frame and the basic sampling unit.  In this design a NAPP
photograph is defined as a 1st stage or primary sampling unit (PSU), and a
sampled pixel within each PSU is treated as a 2nd stage or secondary
sampling unit (SSU).    

PSU's are selected from a sampling grid based on NAPP flight-lines and
photo centers, each grid cell measures 15' X 15' (minutes of
latitude/longitude) and consists of 32 NHAP photographs.  A geographically
stratified random sampling is performed with 1 NAPP photo being randomly
selected from each cell (geographic strata), if a sampled photo falls outside of
the regional boundary it is not used.  Second stage sampling is accomplished
by selecting SSU's (pixels) within each PSU (NAPP photo) to provide the
actual locations for the reference land cover classification. 

The SSU's are manually interpreted and misclassification errors are estimated
and described using a traditional error matrix as well as a number of other
important measures including the overall proportion of pixels correctly
classified, user's and producer's accuracies, and omission and commission
error probabilities.  


Discussion:

While we believe that the approach taken has yielded a very good general
land cover classification product for a large region, it is important to indicate
to the user where there might be some potential problems.  The biggest
concerns are listed below:

1)  Some of the TM data sets are not temporally ideal. Leaves-off data sets
are heavily relied upon for discriminating between hay/pasture and row crop,
and also for discriminating between forest classes.  The success of
discriminating between these classes using leaves-off data sets hinges on the
time of data acquisition.  When hay/pasture areas are non-green, they are not
easily distinguishable from other agricultural areas using remotely sensed
data.  However, there is a temporal window during which hay and pasture
areas green upbefore most other vegetation (excluding evergreens, which
have different spectral properties); during this window these areas are easily
distinguishable from other crop areas. The discrimination between
hay/pasture and deciduous forest is likewise optimized by selecting data in a
temporal window  where deciduous vegetation has yet to leaf out. It is
difficult to acquire a single-date of imagery (leaves-on or leaves-off) that
adequately differentiates between both deciduous/hay and pasture and
hay-pasture/row crop.                           
      
2)  The data sets used cover a range of years (see data sources), and changes
that have taken place across the landscape over the time period may not have
been captured.  While this is not viewed as a major problem for most classes,
it is possible that some land cover features change more rapidly than might be
expected (e.g. hay one year, row crop the next).

3)  Wetlands classes are extremely difficult to extract from Landsat TM
spectral information alone.  The  use of ancillary information such as
National Wetlands Inventory (NWI) data is highly desirable.  We relied on
GAP, LUDA, or proximity to streams and rivers as well as spectral data to
delineate wetlands in areas without NWI data.

4) Separation of natural grass and shrub is problematic. Areas observed on
the ground to be shrub or grass are not always distinguishable spectrally.
Likewise, there was often disagreement between LUDA and GAP on these
classes. 


Acknowledgments

This work was performed by the Raytheon STX Corporation under U.S.
Geological Survey Contract 1434-CR-97-CN-40274. 


References

More detailed information on the methodologies and techniques employed in
this work can be found in the following:

Kelly, P.M., and White, J.M., 1993. Preprocessing remotely sensed data for
efficient analysis and classification, Applications of Artificial Intelligence
1993: Knowledge-Based Systems in Aerospace and Industry, Proceeding of
SPIE, 1993, 24-30.
 
Cowardin, L.M., V. Carter, F.C. Golet, and E.T. LaRoe, 1979. Classification
of Wetlands and Deepwater Habitats of the United States, Fish and Wildlife
Service, U.S. Department of the Interior, Washington, D.C.

Vogelmann, J.E., Sohl, T., and Howard, S.M., 1998. "Regional
Characterization of Land Cover Using Multiple Sources of Data."
Photogrammetric Engineering & Remote Sensing, Vol. 64, No. 1,  pp. 45-47.

Vogelmann, J.E., Sohl, T., Campbell, P.V., and Shaw, D.M., 1998. "Regional
Land Cover Characterization Using Landsat Thematic Mapper Data and
Ancillary Data Sources." Environmental Monitoring and Assessment, Vol.
51, pp. 415-428.  

Zhu, Z., Yang, L., Stehman, S., and Czaplewski, R., 1999. "Designing an
Accuracy Assessment for USGS Regional Land Cover Mapping Program."
(In review) Photogrametric Engineering & Remote Sensing.    


                                             