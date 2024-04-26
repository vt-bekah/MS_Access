# MS Access Projects

## Repairs Database

### Background
I support an organization that does home repair for low income households that is funding by various organizations (local government and private) in which some provide money at the start of the grant period while others use a reimbursement program. Households may receive multiple repairs but applications expire after a year. There are restrictions on the total amount of support a family may receive over the lifetime of owning a property. Additionally, reporting to the funding organizations requires counting demographic information of various times within specific locations depending on the specific funding organization.

### Features
**Implemented:**
* Tables to support the following:
    * Application details (Ideally this would be normalized more than it is. For the sake of usability with this specific user group, it is not broken out further)
    * Repair Details
    * Purchase Tracking
    * Donation Tracking
    * Subcontractor Usage
    * Reimbursement Tracking
* Form to input new, modify, and copy application information including a list of repairs linked to that application
* Form to input new, modify, and copy repair information including 
    * purchase reciepts with total field and list of funding sources used
    * subcontractor estimates with total field
    * donations with total field
    * reimbursements with total field
* Form that includes In Work Repairs (Started but not completed) ONLY
* Form that includes completed repairs that have not submitted reports and surveys ONLY
* Reports
    * Total expenditure by Household (Person + Address) all time vs. limit
    * Current balance of varios funding sources

**TO DO:**
* Reporting that captures demographic information served within a time frame and location entered by the end user
* Views that easily show repairs waiting for reimbursement
* Views that show in work applications and easily navigate to the application for for updates

### DB Screenshots
DB Relationships:
![DB Relationships](Repair_DB/DB_Table_Relationships.png)

Household Application Input Form:
![Household Info Input](Repair_DB/HouseholdApp1.png)
![Household Repair](Repair_DB/HouseholdApp2.png)

Repair Input Form:
![Repair Info Input](Repair_DB/RepairInput1.png)
![Repair Costing Info](Repair_DB/RepairInput2a.png)
![Repair Costing Info](Repair_DB/RepairInput2b.png)

Budget Tracking Report:
![Balances](Repair_DB/BalanceReport.png)

Household Totals Report:
![Household Totals](Repair_DB/HouseholdTotalReport.png)