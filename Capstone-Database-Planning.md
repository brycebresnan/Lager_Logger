sql designer keyword: lagerlogger


batch
* HAS MANY turn
   * HAS ONE batch
   * HAS MANY employee
   * HAS ONE fermenter
* HAS ONE fermentation_tracker
   * HAS ONE batch
   * HAS ONE fermenter
   * HAS MANY employee
* HAS ONE fermenter
   * HAS ONE batch
* HAS ONE cellar_tracker
   * HAS ONE batch
   * HAS MANY task
   * HAS MANY employee
* HAS ONE packaging_tracker
   * HAS ONE batch
   * HAS MANY employee
   * HAS ONE Fermenter
* HAS MANY task
   * HAS ONE employee
   * HAS ONE batch
   * HAS ONE cellar_tracker
   * HAS ONE fermenter


employee
* HAS MANY task








BATCH TABLE
* General Info        -
Bach # 
Brand:
Style:
Volume:
Status: (Planned, InProgress, Complete, Archived)


* Yeast Info        -
Yeast_ID:
Generation:
Yeast Pitch Amount in lbs:
(Yeast from) batch_ID:


* Fermentation Info        -
FV Number
Fermentation_Tracker_ID:


* Turn Info        -


Number of Turns:
Turn_ID:




TURN TABLE
Turn #
Batch_ID
Turn Volume:
Mash Temp:


Grain Bill:
Hops:




FERMENTATION_TRACKER TABLE
Batch_ID
Day Number:
Date:
Time:
Set F
Actual F
Plato
pH
VDK
Req Actions
Comments


FERMENTER
Fermenter #:
Brand:
Volume:
Max Volume:
Type: (Transport, Uni, brite)
Carb Stone Type: 
Current Temp:
Location:
Status: (Occupied, Empty, Dumped, Rinsed, Clean, Sanitized, etc)
Batch_ID:


CELLAR TABLE


PACKAGING TABLE


EMPLOYEE TABLE


TASK TABLE


YEAST TABLE