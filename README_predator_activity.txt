GENERAL INFORMATION

1.
This folder contains the data and R-code for the article: 
Laux, A., Waltert, M., Gottschalk, E. Camera trap data suggest uneven predation risk across vegetation types in a mixed farmland landscape. Ecology and Evolution.


2. Author Information

Corresponding Author:

Amelie Laux
Department of Conservation Biology, 
University of Göttingen, 
Bürgerstrasse 50, 
37073 Göttingen, Germany
amelie.laux@biologie.uni-goettingen.de

Co-Authors:

Matthias Walter
Department of Conservation Biology, University of Göttingen, Bürgerstrasse 50, 37073 Göttingen, Germany

Eckhard Gottschalk
Department of Conservation Biology, University of Göttingen, Bürgerstrasse 50, 37073 Göttingen, Germany


3. Date of data collection:

Dataset 'camera_trap_data_2019_2020'
2019/04/28 - 2019/31/07
2020/04/27 - 2020/08/04

Datasets 'camera_trap_data_flowerstrips_1m' and 'camera_trap_data_flowerstrips_all'
2020/08/03 - 2020/09/03


4. Geographic location of data collection

District of Göttingen, Germany


5. Funding sources

Amelie Laux received a PhD-Scholarship by the German Federal Environmental Foundation (DBU, AZ 20018/573). 
Field work was supported by the Deutscher Falkenorden e.V. (DFO, German falconers’ association), the Mandfred-Hermsen Foundation, 
and the Jägerschaft Duderstadt e.V. (Hunters’ Association Duderstadt).


DATA & FILE OVERVIEW

1. File list: 

camera_trap_data_2019_2020.csv
camera_trap_data_flowerstrips_all.csv
camera_trap_data_flowerstrips_1m.csv
predator_activity_script.R


2. File description:

'camera_trap_data_2019_2020.csv'
created 2022/05/30
contains camera trap locations, predator observations and environental parameters (e.g., wood area, distance to water) 
for each camera site sampled in summer 2019 and 2020 as part of the 'predator activity within the landscape'analysis. 

'camera_trap_data_flowerstrips_all.csv'
created 2022/05/30
contains camera trap sites, positions (edge or centre of the flowerstrip) and predator observations for each camera site sampled in flower strips
in August 2020 as part of the 'predator activity in flower strips'analysis. In the '_all' dataset, all observations at cameras at the edge of flowerstrips were included.

'camera_trap_data_flowerstrips_1m.csv'
created 2022/05/30
the same data as above ('camera_trap_data_flowerstrips_all.csv'), but at edge cameras, only predators that passed within 1 m of the camera were included

predator_activity_script.R
created 2022/05/30
R-script containing all code used for the analysis in the paper 'Camera trap data suggest uneven predation risk across vegetation types in a mixed farmland landscape'

2. Relationship between files: 

The camera trap data files are necessary to run the R code.


METHODOLOGICAL INFORMATION

Please see the above-mentioned paper for detailed information on data sampling and processing.
The R-script was developed using version R 4.1.1.


DATA-SPECIFIC INFORMATION:

A) 'camera_trap_data_2019_2020.csv'

1. Number of variables: 62

2. Number of cases/rows: 241 (with headings in row 1)

3. Variable List: 

stationID - unique ID for each camera trap station
site - ID for each camera site
study_area - in which part of the study area the camera was located: D (Diemarden) or E (Eichsfeld)
Vegetation - vegetation type: B (flower strip), E (field margin), H (hedge), W (winter cereal), R (rapeseed)
camera - ID number of the camera
Block - time block in which the camera was active, 1-4
SD - ID number of the SD card
Year - 2019 or 2020
xcoord - x coordinates of the camera location, in EPSG: 25832
ycoord - y coordinates of the camera location, in EPSG: 25832
Runtime - active camera time in in minutes
start - sampling start time and date
end - sampling end time and date
badger - number of independent badger captures
boar - number of independent boar captures
cats - number of independent cat captures, domestic cats and wild cats
dog - number of independent dog captures
fox - number of independent fox captures
marten - number of independent marten captures, stone and pine marten
mouseweasel - number of independent mouse weasel captures
racoon - number of independent racoon captures
stoat - number of independent stoat captures
allpredators - total number of independent predator captures
allpredators_without_dogs - total number of independent predator captures, excluding dogs
badger_100 - number of independent badger captures extrapolated to 100 active camera days
boar_100 - number of independent boar captures extrapolated to 100 active camera days
cats_100 - number of independent cat captures extrapolated to 100 active camera days, domestic cats and wild cats
dog_100 - number of independent dog captures extrapolated to 100 active camera days
fox_100 - number of independent fox captures extrapolated to 100 active camera days
marten_100 - number of independent marten captures extrapolated to 100 active camera days, stone and pine marten
mouseweasel_100 - number of independent mouse weasel captures extrapolated to 100 active camera days
racoon_100 - number of independent racoon captures extrapolated to 100 active camera days
stoat_100 - number of independent stoat captures extrapolated to 100 active camera days
allpredators_100 - total number of independent predator captures extrapolated to 100 active camera days
allpredators_without_dogs_100 - total number of independent predator captures, excluding dogs, extrapolated to 100 active camera days
Wood_Dist - distance to next woody structure (hedge, small wood, forest), in [m]
Water_Dist - distance to next permanent water body (running and standing water), in [m]
Settl_Dist - distance to next settlement, in [m]
Edge_Dist - distance to next field edge, in [m]
Road_Dist - distance to next road, in [m]
Wood_Area_500m - area of woody structures (hedge, small wood, forest) within 500 m around the camera, in [ha]
Ext_Area_500m - area of extensively used grassland (including fallows, flowerstrips) within 500 m around the camera, in [ha]
Arable_Area_500m - area of arable land within 500 m around the camera, in [ha]
Settl_Area_500m - area of settlments within 500 m around the camera, in [ha]
Water_Area_500m - surface area of permanent water bodies (running and standing water) within 500 m around the camera, in [ha]
Edge_Area_500m - area of field margins within 500 m around the camera, in [ha]
Road_Density_500m - area of roads (outside of settlments) within 500 m around the camera, in [ha]
Border_Length_500m - length of field block borders within 500 m around the camera, in [m]
Hab_Div_500m - Shannon Index of habitat diversity calulated within 500 m around the camera, please see paper for more details
Mean_Field_500m - mean area of fields within 500 m around the camera, in [m²]
Water_Area_1km - surface area of permanent water bodies (running and standing water) within 500 m around the camera, in [ha]
Water_Area_2.5km - surface area of permanent water bodies (running and standing water) within 500 m around the camera, in [ha]
Settl_Area_1km - area of settlments within 1 km around the camera, in [ha]
Settl_Area_2.5km - area of settlments within 2.5 km around the camera, in [ha]
Forest_Area_500m - forest area within 500 m around the camera, in [ha]
Forest_Area_1km - forest area within 2.5 km around the camera, in [ha]
Forest_Area_2.5km - forest area within 2.5 km around the camera, in [ha]
Arable_Area_1km - area of arable land within 1 km around the camera, in [ha]
Arable_Area_2.5km - area of arable land within 2.5 km around the camera, in [ha]
Grass_Area_500m - grassland area within 500 m around the camera, in [ha]
Grass_Area_1km - grassland area within 1 km around the camera, in [ha]
Grass_Area_2.5km - grassland area within 2.5 km around the camera, in [ha]


4. Missing data codes: 

no missing data


5. Abbreviations:
 
study_area - D (Diemarden) or E (Eichsfeld)
Vegetation - B (flower strip), E (field margin), H (hedge), W (winter cereal), R (rapeseed)



B) 'camera_trap_data_flowerstrips_all.csv'
    and
   'camera_trap_data_flowerstrips_1m.csv'

-> both files have exactly the same structure

1. Number of variables: 29

2. Number of cases/rows: 49 (with headings in row 1)

3. Variable List: 

stationID - unique ID for each camera trap station
site - ID for each camera site
study_area - in which part of the study area the camera was located: D (Diemarden) or N (Nesselroeden)
Position - position in the flower strip: e (edge) or c (centre)
camera - ID number of the camera
SD - ID number of the SD card
Runtime - active camera time in in minutes
start - sampling start time and date
end - sampling end time and date
badger - number of independent badger captures
boar - number of independent boar captures
cats - number of independent cat captures, domestic cats and wild cats
dog - number of independent dog captures
fox - number of independent fox captures
marten - number of independent marten captures, stone and pine marten
mouseweasel - number of independent mouse weasel captures
racoon - number of independent racoon captures
allpredators - total number of independent predator captures
allpredators_without_dogs - total number of independent predator captures, excluding dogs
badger_100 - number of independent badger captures extrapolated to 100 active camera days
boar_100 - number of independent boar captures extrapolated to 100 active camera days
cats_100 - number of independent cat captures extrapolated to 100 active camera days, domestic cats and wild cats
dog_100 - number of independent dog captures extrapolated to 100 active camera days
fox_100 - number of independent fox captures extrapolated to 100 active camera days
marten_100 - number of independent marten captures extrapolated to 100 active camera days, stone and pine marten
mouseweasel_100 - number of independent mouse weasel captures extrapolated to 100 active camera days
racoon_100 - number of independent racoon captures extrapolated to 100 active camera days
allpredators_100 - total number of independent predator captures extrapolated to 100 active camera days
allpredators_without_dogs_100 - total number of independent predator captures, excluding dogs, extrapolated to 100 active camera days


4. Missing data codes: 

no missing data


5. Abbreviations:

study_area - D (Diemarden) or N (Nesselroeden)
Position - e (edge) - c (centre)