# Prison-and-Inmate-Record-Management-System-assembly

Feature 1: Inmate Intake & Profile Creation
Registers new inmates with ID, name, age, crime category and sentence duration. Stores records in arrays with name and crime fields and validates for duplicate IDs.

Feature 2: Sentence Tracking & Release Date Calculation
Uses a dedicated procedure to calculate the expected release date based on intake date and sentence length. The procedure is reusable and is called both during initial intake and whenever a sentence is modified. Flags inmates whose release date falls within the current simulated month.1

Feature 3: Cell Block Assignment & Occupancy Management
Assigns inmates to cell blocks based on crime severity and available capacity. Tracks occupancy per block and prevents over-assignment beyond capacity.

Feature 4: Incident Reporting & Penalty Extension
Records disciplinary incidents linked to an inmate. Each incident can extend the inmate's sentence by a defined penalty period, updating their release date accordingly.

Feature 5: Parole Eligibility Checker
Checks whether an inmate meets parole criteria - served minimum time, no recent incidents. Displays eligible inmates and generates a parole recommendation list.

Feature 6: Inmate Transfer Between Cell Blocks
Processes internal transfer requests by moving an inmate from one cell block to another. Validates capacity of the destination block, updates occupancy arrays for both blocks 
