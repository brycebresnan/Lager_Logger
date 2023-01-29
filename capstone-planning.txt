Tools
* Ruby On Rails
* Tailwind CSS 
* PostgreSQL
* Deployment on Linux Server 


Nav Bar Structure


* Logo
* “Logged In As…”
* Log Out Button
* Dashboard (Home view)
* Brew Data
   * Brew Planning/Tank Schedule
   * Recipe Builder
   * Brewsheet Editor
      * Start New Brewsheet
   * Brewing Corrections Calculator (Maybe built into brew sheet)
* Cellar Data
   * Fermenters
      * Location (overview)
         * FV Dropdown (Details)
   * QA Data
   * Yeast Management Tool
      * Yeast Count/Pitch Calculator
      * Yeast Count Log
   * Tank Cleaning Log
* Packaging Data
   * Package Log (records QA checks/progress for packaging runs)
   * Package Type Calculator (how many cans v kegs)
   * Can Weight Calculator
   * Keg sticker generator
* Task Manager
   * Daily Tasks
   * Task Editor
* Inventory
* Data Archive (search through master sheets)


















Views


* Log In
* Sign Up
* Dashboard (Home View)
   * Cellar Overview (can change locations) 
      * View of all set up fermenters (click to show Fermenter # Details)
         * Beer Brand
         * Initial Batch Volume
         * Volume - recorded loss
         * Age (Day #)
         * Temperature of tank 
         * Last Recorded Gravity (Green < 24 hours, yellow > 24 hours)
         * Last Recorded pH (Green < 24 hours, yellow > 24 hours)
   * Daily Tasks
   * Warnings? (If tasks not completed previous day, tank temps out of range, tank age > average, inventory low)
   * Brew Schedule Viewer


Brew Data


* Brew Planning/Tank Schedule
   * Colored calendar to show tank times visually
      * Yeast Harvest Planning 
      * Packaging Planning
* Brewsheet Editor
   * Start New Brewsheet (if no current sheet)
   * Continue Current Sheet (save state automatically)
   * Open Sheet by Batch Number (opens old sheet if batch number is known)
      * Search for sheet function? Show last time this brand was brewed etc.
* Brewing Corrections Calculator (Maybe built into brew sheet)


Cellar Data


* Cellar Overview (see above)
* Fermenter # Details
   * Status
      * Empty/Rinsed/Clean/Fermenting/Finished/Crashed/Carbed
   * Brand Name
   * Batch Volume
   * Volume - Dump volumes
   * Brew Date
   * Batch Number
   * Brew Data (Link to brew sheet)
   * Yeast: (auto populated from yeast count log?)
      * Yeast ID
      * Generation
      * Pitch Rate
      * From Batch #
      * Harvest?
   * Set Temp
   * Actual Temp
   * Plato
   * pH
   * VDK
   * Crashed?
   * Last Action
   * Next Action
   * Action Needed?
      * Task assigned?
         * Task assigned to…
   * Warnings?
   * Notes
   * QA Check Log:
      * Date
      * Time
      * Set Temp
      * Actual Temp
      * Plato
      * pH
      * VDK result
      * Initials
   * Fermentation Graph
   * Dry Hop Log
      * Hop Name
      * Lot Number
      * Amount (in lbs)
      * Date
      * Initials
   * Fining Log:
      * Biofine amount (in liters)
      * Date
      * Initials
   * Carb Log:
      * Date
      * Time Started
      * Time Ended
      * Vol CO2
      * Tank PSI
      * Initials 
   * Confirmation Carb
      * Date
      * Vol CO2
      * Tank PSI
      * Initials
* Add fermenter
   * Location (in case  multiple locations)
   * Tank Number
   * Volume
   * Max Volume
   * Manufacturer
   * Row number? Cellar Number?
* Edit Fermenter
   * Delete Fermenter
* Cleaning Logs
   * Select Fermenter #
      * Display historic logs (date desc)
   * Add Entry
      * Date
      * Type:
         * Caustic
         * Acid
      * Notes: (spray ball clogged, replaced gasket, etc)
      * Initials


Packaging Data


* Package Log (records QA checks/progress for packaging runs)
* Package Type Calculator (how many cans v kegs)
* Can Weight Calculator
* Keg sticker generator




Task Manager


* Daily Tasks Overview
   * View (Auto populated by fermentation profile)
   * Edit
   * Add 
   * Assign tasks 


Inventory
* Inventory Overview
   * Low Stock Warnings?
   * Add Inventory Items
   * Edit Items
      * Delete Items


Archive
* Master Sheet Archive
   * Search
      * Batch Number
      * Date
      * Brand
      * Fermenter Number
      * Yeast Type
   * Display Filter
      * Date (asc/desc)
      * Date Range
      * Batch Number  (asc/desc)
      * Brand
      * Fermenter Number  (asc/desc)
      * Yeast Type