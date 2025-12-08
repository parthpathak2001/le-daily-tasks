# ___________________________________________________________________________________________________________

# 01-12-2025

## Empower HH

- 11:24 - 11:35

- Export discount log upload in live - 11:35 - 12:10

- Order export changes checked which is done by siddh and changes in darshil's uploaded order export  - 12:10 - 12:35

- user sync checked - users_hierarchy table have multiple row of same user - 12:35 - 1:12
    uploaded latest user division sync changes in live (DELETE OLD DIVISION ENTRIES changes) 

- Order Details page changes - 1:20 - 1:51, 6:20 - 7:25
    display invoice details in seperate table
    remove columns of invoice details from tagging section

- Order Approval List issue checking in Live - 2:45 - 4:15, 4:25 - 4:50
    Checked the Order Approval List issue. Found that the order was visible because the user's parent hierarchy included that ZBM, so the ZBM user was able to see the order as per the hierarchy chain.

- Order Approval List API chages – ZBM Logic Update - 4:50 - 6:20
    - Updated ZBM approval logic to fetch orders based on user hierarchy (ZBM → downline users) instead of division-based mapping.
    - Orders are now displayed only when the tagged user belongs to the logged-in ZBM’s downline.

    - Order Tagging Approval API changes – Pending Clarification
        Reviewed required changes based on new ZBM logic.

        Need clarity on:
            1. How to handle approvals when a single tagging has SPEs under different ZBMs.
            2. How to update final tagging status when multiple ZBMs approve the same tagging.

- Sync changes - 7:25 - 8:10
    Updated the sync process to store the original Mavens start and end dates in the respective tables (acc_mgr_relation_mavens, emp_acc_mgr_map_mavens, emp_division_mavens, emp_role_mavens) so the raw Mavens data remains available even after admin-side updates.


## Miscellaneous
- Add worklog - 8:10 - 8:35


# ___________________________________________________________________________________________________________

# 02-12-2025

## Empower HH

- 10:35 - 11:16

- User hierarchy export - 11:30 - 11:50

- questionary issue checking - raised by shaziya - 11:50 - 12:15, 12:30 - 1:43, 2:00 - 2:29, 2:54 - 3:00, 3:30 - 4:14, 4:23 - 4:45 

- Meeting with Empower and Mavens team, regarding BE-SBM mapping and mavens master data issue - 3:00 - 3:30

- User Group (Web) – Developed full User Group CRUD module. - 4:45 - 5:07, 5:35 - 5:38, 5:57 - 7:35

## Miscellaneous
- help to siddh for whatsapp otp sent for RMIS project  - 12:15 - 12:30, 5:07 - 5:35, 5:38 - 5:57
    checked meta panel of RMIS to find template and other details
    message not sending from meta API so i helped to check it, it returns issue - template not found issue (template exist in meta but also sending this issue)
    created new template

- Add worklog and create new module - 7:35 - 8:00
    

# ___________________________________________________________________________________________________________

# 03-12-2025

## Empower HH

- 10:34 - 11:10

- Quiz List API Changes – Fetch Data From User Group - 11:10 - 11:20, 11:27 - 12:36, 12:39 - 1:03, 1:18 - 2:03, 3:15 - 3:35 (148 mins)
    Updated Quiz List API to fetch quizzes based on User Group.
    Integrated quiz list and quiz submit apis changes shared by Siddh into local code.
    Uploaded updated code to UAT.
    Tested API responses and verified User Group filtering.

- Quiz List issue checked - 20 mins
    Checked issue reported by Durgesh; functionality was correct, the issue occurred due to incorrect data - Durgesh used an old quiz instead of the newly assigned one.

- Quiz List -> Completed Quiz -> View Answer: “Data not found” Issue Check - 30 mins
    Verified the API and found no issue. The message appeared because the user had not submitted any questions, resulting in no data to display.

- Order Approval List API changes - changed Sorting by status - 2:25 - 2:41

- Order Details Api changes - 2:56 - 3:15, 4:05 - 6:30
    Implemented logic to ensure that when a logged-in user views an order that was not created by them, the API will now display only those products where the user is tagged.
    If the user is not tagged for a product, that product will not be shown in the order details response.
    Unit Testing
    Uploaded in UAT

- Discussion with Harsh, Siddh regarding how to manage user vacancy, how to manage account manager code of new user    - 6:30 - 7:20

## Miscellaneous
- Add worklog - 7:20 - 7:50

# ___________________________________________________________________________________________________________

# 04-12-2025

## Empower HH

- 10:33 - 11:00

- Send mail to Empower team and Mavens team, regarding how to manage Account Manager code for a new user - 11:25 - 11:40

- User hierarchy export - 11:00 - 11:21, 

- Hierarchy sync changes: - 11:40 - 1:00
    - Updated hierarchy sync logic: when a parent user's hierarchy is updated, the corresponding child users now inherit the latest hierarchy structure.
    - As discussed with the client, the SBM hierarchy value should not be updated through the sync script. Removed SBM-related hierarchy updates from all relevant scripts.
    - Changes uploaded to UAT.

- Developed two new cron scripts for the user vacancy: - - 1:00 - 1:55, 3:17 - 3:25, 4:13 - 5:25
    1. Vacancy Activation Cron: Activates user vacancies based on the effective date.
    2. Vacancy Replacement Cron: Automatically replaces users into activated vacancies on their effective date.
    - Changes uploaded in UAT

- Doctor Discount Approval List issue - only is_authority user can approve doctor discount, division head or other users can not approve order - issue checked, issue is from Application not in web or api - 2:13 - 2:34, 2:53 - 2:59

- Doctor discount allowed updated issue checked - issue not found - 3:25 - 3:55

- Discussion with Harsh regarding display invoice-product user's division wise when is_tagged = 1 - 3:55 - 4:06

- Store log when doctor -> is_discount 0/1 update in live - 5:25 - 6:00

- Checking attempted quiz displaying or not to thier manager, attempted quiz which assigned in user group - 6:00 - 6:55

- 6:55 - 7:20

## Miscellaneous
- Add worklog - 7:20 - 7:55

# ___________________________________________________________________________________________________________

# 05-12-2025

## Empower HH

- 10:38 - 10:50

- User → User Q/A Module Issue (Raised by Durgesh) – Checked & Fixed    - 10:50 - 11:45
    - Issue existed only in UAT/Local, not in Live.
    - Result was not displaying correctly even though marks were correct.
    - Fix was already applied in Live but missing in UAT/Local.
    - Synced Live code to UAT & Local → issue resolved.

- Order details changes - 11:45 - 12:45
    Order Details API updated to display only tagged invoice products when the user is not the creator and is_tagged = 1.
    - Changes uploaded in UAT

- PHP team meeting - 12:45 - 1:10
    project priority discussion

- 1:10 - 1:20

- HR ma'am meeting- 1:20 - 1:50
    probation evalution meeting with HR Ma'am, Ram sir and Snehalbhai

- 1:50 - 02:00

- user hiearchy export changes- 3:00 - 3:30, 5:30 - 6:00, 6:35 - 7:10

- upload user group related changes in Live - 3:30 - 3:35, 6:00 - 6:35, 7:10 - 7:50
    some issue solved in live - date format issue

## RMIS (SG Vetcare)

- Task Understanding with Siddh - 3:35 - 4:25, 4:37 - 5:30
    - Since Siddh will be on leave next week, I reviewed and understood the RMIS project tasks directly with him.
    - Discussed the pending tasks so I can continue work in his absence.

## Miscellaneous
- Add worklog - 7:50 - 8:25


# ___________________________________________________________________________________________________________

# 05-12-2025

## Empower HH

- Testing in UAT - User Hierarchy role change, division change, vacant user functionality change - 10:36 - 11:26, 11:30 - 12:10, 2:29 - 5:30
    some issue found - parent code not storing properly so other changes not working - given to siddh to solve this issue 
    after siddh solved an issue tested again
    change user role based on effective date cron script changes - user status change to Active from Resigned effective date based cron script changes
    it takes too much time to unit test because we tested multiple scenarios - user role change on current date and on future effective date, user division change on current date and on future effective date, user hiearchy (manager) change on current date and on future effective date, create user vacancy on current date and on future effective date, replace user vacancy on current date and on future effective date, etc.

- Testing in UAT – User Hierarchy, User Role, User Division, User Vacancy Create and Replace User Vacancy cron script changes 
    Performed detailed UAT testing for:
        User role change (current & effective date based)
        User division change (current & effective date based)
        User hierarchy / manager change (current & effective date based)
        Vacant user creation & vacancy replacement (current & effective date based)
    Found an issue: parent code was not storing properly, causing dependent logic to fail.
        → Reported to Siddh, issue fixed.
    Re-tested all flows after fix.
    Updated “role change based on effective date” cron script:
        Ensures user status correctly changes to Active from Resigned when effective date is reached.
    Testing took longer due to the large number of scenarios, including:
        Role changes (current & effective date based)
        Division changes (current & effective date based)
        Manager (hierarchy) changes (current & effective date based)
        Vacancy creation (current & effective date based)
        Vacancy replacement (current & effective date based)

- check_header_authentication api changes - Display proper message when user resigned and already logged in - 45 Mins
    changes uploaded in UAT and Tested
    Issue raised by Durgesh: Apis not working issue, it was not an issue, user is resigned so data not displaying

- User hierarchy export functionality testing - 12:10 - 1:33,

## RMIS (SG Vetcare)

- Discuss with siddh, regarding he done point at last saturday which i will work on it - 10:26 - 10:36

# ___________________________________________________________________________________________________________

##### PENDING
- Admin Panel - Order status change from "On Hold & Expired", send otp also - PENDING

- Revert Order Status (Admin panel), email not working - PENDING

- Dashboard load lye che e check krvu (su load lye e check krvu)

---

- On_hold and Expired exact time e thava joi - (e research krvanu che) - PENDING

---

- mapping, role change, division change, etc. Sync ma Efective date nu rakhvu. effective avya pachi aapdi system ma effect kravu

- (WEB) Need to check datatable - after search it display data by search but page and count of records not changing - ISSUE 

---


- Order Details changes (web) -> Order Invoices section - Invoice details product tagging list ma j batavi - DONE

- Implement export functionality in the Order List screen with two formats: - (DONE by Darshil)
    Normal Export
    Custom Export (format to be provided by Komal)

- Include a Total Amount row at the bottom of the Order List table.(ALL price 3 column) - DONE

- In the Order Detail tagging section, display the division name after the product name. [Order Invoices ma Product ni baju column ma Division name btavu] - (IN WEB DONE DARSHIL & EXPORT DONE BY PARTH) - DONE

- In the Doctor List, add a “Last Mapped Date” column. - DONE

- In the Discount Logs screen, add a state filter and enable export functionality. - DONE BY DARSHIL

- Order Details changes (web) -> Order Invoices section - Invoice details tagging product list ma j batavi - DONE

---

- quiz issue - raised by Shaziya

---

- Vacant user ni functinality krvi - DONE test is pending

- user hierarchy export changes

- Store logs (Web & APIs)

---

- Replace user to resigned user (waiting for siddh updation) - Pending

######
