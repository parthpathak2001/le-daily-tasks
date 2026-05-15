# ___________________________________________________________________________________________________________

# 01-01-2026

## Miscellaneous
- 11:07 - 11:20
- Add Worklog - 11:20 - 11:55, 6:55 -  7:30
    Create new module
    increased estimate hour in exisiting modules 

- system setup - 11:55 - 12:15, 7:30 - 8:00
    git setup
    project updated in ravi bhai pc because i work on that system, because my system is formated
    xampp install and all project backup files move 

- system issue - 3:55 - 4:15
    - network not working
    - filezilla not conecting
    - discuss with rahul bhai

## Empower HH
- connecting live server for see stockist mail not sending issue - 2:30 - 3:00
    server not connecting, checked in ravi bhai system, checked in my system, checked in siddh system its not connecting
    checked in athikur system it connected
    checked log configured or not in empower live project, its not configured 


- send Order Details to Stockist mail - store log  - 3:15 - 3:55, 4:15 - 4:20, 4:30 - 5:10, 5:40 - 5:47
    - Added logging for Send Order Details to Stockist mail in the order_logs table to track mail status (sent / failed / not attempted).
    - Uploaded the changes on the live server.
    - Issue Identified: The requirement was to send order details to stockists using a different SMTP account. For this, SMTP email and password were statically configured in the mail-sending function, while host and port were expected to be taken from the config file. However, the SMTP host and port were changed in the configuration file, causing a mismatch with the statically configured SMTP setup and resulting in mail failure.
    - Resolution: Corrected the SMTP configuration mismatch and verified mail sending functionality.
    - Manually sent order details mails to stockists where required.

- Order Approval List API changes - 12:15 - 1:05, 1:50 - 1:56
    - Updated approval list to show orders from both _4D and _9D divisions to the same Division Head instead of a single division.

- Order Tagging Approval Action API changes - 1:56 - 2:30, 3:00 - 3:15
    - Updated approval logic so the Division Head can approve order taggings for orders belonging to both _4D and _9D divisions without any restriction.

- Order Notification Changes - 5:10 - 5:40, 5:47 - 5:53
    - Updated notification logic so Division Heads receive notifications for order invoice uploads and tagging actions from both _4D and _9D divisions.

- Notification Count API changes - 5:53 - 6:16
    - Updated logic to display the pending order tagging approval popup for the logged-in Division Head, considering orders from both _4D and _9D divisions instead of a single division.

- Order Tagging Approval Action API changes - For ZBM - 6:16 - 6:35
    - Updated ZBM approval logic to approve orders based on hierarchy mapping, aligned with the approval list behavior.

# ___________________________________________________________________________________________________________

# 02-01-2026

## Miscellaneous
- 10:19 - 10:50
- Add worklog - 10:50 - 11:23, 11:29 - 11:40

- System Setup - 11:40 - 12:10, 12:25 - 12:35, 12:45 - 1:00, 4:45 - 5:00
    database backup implement
    project backup implement
    matermost install, version not suitable, reinstall older version
    Putty install
    WPS install

## Empower HH

- Uplaod latest code - 12:10 - 12:25, 12:35 - 12:45

- 1:50 - 2:10

- Mavens Data Verification & Manual Order Mail - 2:10 - 3:15
    - Reviewed Mavens sheets with Harsh.
    - Manually verified chemist details against Mavens sheets.
    - Manually verified doctor data against Mavens sheets.
    - Manually sent order details email to stockist for Order ID 503.

- Meeting & Discussion on Mavens Sync Issue  - 3:22 - 4:05
    - Attended meeting with Snehalbhai, Ravi, and Harsh.
    - Discussed current Mavens data sync issues, root causes, and next action points.

- New Task Understanding - 4:05 - 4:20
    - Discussed requirement to store sync execution logs to track successful/failed syncs and allow re-running sync scripts for previous unsuccessful days.
    - Understood changes required in Courier and Questionnaire modules to replace existing team-wise logic with hierarchy-wise data display wherever applicable.

- employee-SBM mapping script changes - sync data based on the effective date - 5:00 - 5:30
    - Updated SBM mapping sync to run based on effective date.

- Manually sent order details email to stockist for the order due to email not being triggered automatically. - 5:30 - 6:00

- 6:00 - 6:15

- Mavens Data Sync Verification (Doctor & Chemist) - 6:15 - 7:10
    - Manually checked Mavens sheets to verify doctor and chemist data syncing issues.
    - Found incorrect Doctor UNI values.
    - Chemist sheet data is blank from 17-12-2025 onwards.

# ___________________________________________________________________________________________________________

# 05-01-2026

## Miscellaneous
- 11:10 - 11:25

- Add worklog - 11:25 - 11:45, 
- 11:45 - 12:00

- List down all tasks completed in the previous week for the weekly meeting discussion. - 12:00 - 12:10

- Weekly Meeting - 5:00 - 5:40

## Empower HH
- Checked Login API issue in UAT (not working due to server issue).  12:10 - 12:30 
    Verified Login API on live server.
    Re-tested Login API in UAT after server issue was resolved (by Ravi bhai).

- Manually Send Order Details Email to Stockist - 12:30 - 12:45
    - To send the order details email, logged in as the respective order approver and approved the order again. 
    - Verified that the order details email was sent correctly to the stockist after re-approval.
    - Order: 477, 480, 499

- 1:35 - 2:05

- send Order Details to Stockist mail - 12:45 - 1:02, 1:26 - 1:35, 2:05 - 2:15, 2:41 - 3:10, 3:30 - 3:35
    - store status to identify mail sent or not in particular order
    - Uploaded Latest changes in live

- Checked PMS API email and reviewed payload details. - 3:10 - 3:30
    Replied to mail acknowledging API details.
    Noted question regarding division name mapping between Empower and PMS for future clarification.

- CRON Log Implementation - 3:30 - 4:12, 4:17 - 4:45, 6:05 - 6:25,
    - Added daily CRON log to store whether each scheduled sync CRON ran successfully or not.

- Mail checking and reply - 4:45 - 5:00 ,5:40 - 5:50 
    - Checked emails
    - Verified UNI codes in customer master file
    - Sent reply with details

- Testing with Durgesh - 5:50 - 6:05, 6:25 - 7:45
    - exaplain changes which need to testing and explain senarios
    - database is from live so helped to manage users
    - database is old so some tables changes not in that so added that changes
    - some issue found, that solved

- Order Details Page Changes - 7:45 - 8:15
    - Updated order details page to display data for Division Heads by considering both _4D and _9D divisions


# ___________________________________________________________________________________________________________

# 06-01-2026

## Miscellaneous
- 9:50 - 10:30

- Add Worklog - 10:30 - 10:45

- Time Management - 2.5 hour

## Empower HH

- Order Approval Changes (_9D / _4D) – Testing - 10:45 - 11:23, 11:47 - 12:15, 1:35 - 1:50
    - Created test users for _9D and _4D divisions.
    - Created new test scenarios to validate:
        - Order approval list visibility for both _9D and _4D.
        - Approval action flow for Division Head.
        - Notifications and pending approval popup behavior.
    - Verified end-to-end approval flow with new scenarios.
    - Doctor, User, Chemist, Stokist managed

-  Store CRON Logs Using Common Function - 11:29 - 11:47, 12:15 - 12:40
    - Implemented logging for all CRON jobs using a common function to store their daily execution status.

- 12:40 - 12:58

- Create CRON Script to Re-run Failed Crons - 1:50 - 2:15, 3:00 - 3:15
    Created a new CRON script to identify failed CRON jobs using execution logs.
    Implemented logic to re-run only one failed CRON at a time to avoid timeout issues.
    Work partially completed due to office activities; remaining enhancements will be completed next.

- December project work summary -  1:20 - 1:35 - 3:15 - 3:40, 6:05 - 7:05
    - Checked December worked hours and completed tasks.


# ___________________________________________________________________________________________________________

# 07-01-2026

## Miscellaneous
- Add worklog - 10:55 - 11:05

- Discussed order approval flow doubts with Harsh - 11:05 - 11:12

- Order Approval Flow Check - 11:20 - 12:10
    - Checked the order approval flow to understand and solve doubts.

## Empower HH
- 12:45 - 1:00, 1:16 - 1:30 
- Update CRONs for Date-wise Sync - 1:30 - 2:24, 2:54 - 3:00 - ADDED
    - Updating existing CRON jobs to support date-wise (past data) sync instead of only current date.
    - This will help in re-running failed CRONs for past dates when required.
    - Affected CRONs:
        - sync_chemists
        - sync_doctors
        - sync_employee
        - sync_employee_account_manager_code
        - sync_employee_role
        - sync_employee_acc_mgr_relation
        - sync_users_city_state
        - sync_employee_division
        - cron_apply_effective_hierarchy
        - sync_sbm_mapping_mavens
        - apply_sbm_mapping_to_hierarchy
        - sync_user_doctor_mapping

- User Hierarchy Tree – Live Upload (New Drag & Drop) - with Siddh - 04:45 - 6:15 - ADDED
    - Manually uploaded the new User Hierarchy Tree feature and drag-and-drop hierarchy management changes to Live and verified the functionality.

- Mavens data sheet manualy checked for doctor data verification (state issue) - 12:35 - 12:45 - ADDED

- Meeting – Mavens Data Mismatch with Empower team and mavens team - 6:15 - 7:15 - ADDED
    - Meeting with Komal and Mavens team regarding data mismatch in Mavens sheets. Also discussed issue with incorrect doctor state data and received a separate CSV for doctor state details.


- Mail drafting and sending for Mavens master data syncing - 7:15 - 8:00 - ADDED

----------
- Client Meeting – Courier & Questionnaire (Shaziya) - 3:00 - 3:20 - ADDED
    - Meeting with Shaziya to discuss courier and questionnaire changes, data display based on user hierarchy instead of team, and other updates.


- Discussion with Durgesh- 3:20 - 3:30
- Study Material Notification Issue Check (Shaziya) - 3:30 - 3:40 - ADDED
    - Checked issue where study material notification was not sending. Found that the issue is due to old notification code.

- Add Courier – Primary Receiver Issue Check (Shaziya) - 3:40 -  4:25, 4:38 - 4:45 - ADDED
    - Checked issue where Jameel sir’s name was not displaying in the Primary Receiver dropdown. Issue was resolved after identifying that the user does not have an office location assigned. Time was taken to manually verify user and location data to find the cause.



# ___________________________________________________________________________________________________________

# 08-01-2026

## Miscellaneous
- 10:19 - 10:28
- Add Worklog - 10:28  - 10:44, 7:45 - 

## Empower HH
    - Verified cmpostaladdress.csv sheet - 11:25 – 11:55
        Confirmed it contains state data for Employee, Chemist, and Doctor
        Sent mail to Mavens team for confirmation
    - Checked Mavens master data sheet and verified all data successfully


- Cron Script for Syncing Doctor Address Data from Mavens to Empower - 10:44 - 11:20, 5:45 - 7:45
    - Create a new cron script
    - Read cmpostaladdress.csv from the S3 bucket
    - Sync doctor/customer state and address details into Empower
    - Log cron execution status (success/failure)


- Fix Notification Issue for Courier / Study Material - 11:55 - 1:15, 2:13 - 2:32
    - Identify issue with notification not sending
    - Replace old notification code with new notification logic
    - Test notification flow for courier and study material

- Upload Latest code in UAT - 2:32 - 3:05
    Solve Conflict

- User Hierchy issue check in live - Admin not found issue - 3:05 - 3:35
    - User is resigned as per given sheet by Roshan sir but in our system is Inactive because we syncing from Mavens 

- Upload User Module changes in  Live with Siddh - 3:35 - 4:05, 4:14 - 4:19, 4:29 - 5:30
    - User import, User export, User Hierarchy Tree, etc changes
    - after upload i checked and it have some issue, then reuploaded related changes

- Data updation - requested by durgesh - 5:30 - 5:45
    User doctor mapping data

# ___________________________________________________________________________________________________________

# 09-01-2026

## Miscellaneous
- 10:20 - 10:30
- Add Worklog - 10:30 - 10:55

## Empower HH
- Siddh have git issue - help to solve - 10:55 - 11:10

- API Changes: Update State Handling for Employee, Doctor, and Chemist - 11:10 - 12:15, 2:00 - 2:05, 2:15 - 2:30, 4:44 - 5:10
    - Disable old functionality for storing state in employee, doctor, and chemist modules
    - Store and update state only through the new address sync API
    - Test state updates thoroughly for Employee, Doctor, and Chemist to ensure correct behavior
    - checked all sync script in local

- Sync master data from Mavens using the following sheets: - 5:10 - 7:45
    - Stored chemist's pan card no. and pancard name 
    - Stored doctor's phone no. 

    - Syced data:
        - customermaster.csv
        - dealerdetail.csv
        - custaccmap.csv
        - employee.csv
        - cmpostaladdress.csv

- Upload code - 12:15 - 1:20
    - uploaded order approval changes, api changes, Add/Edit Quiz notification changes
    - Testing on Live

- 1:40 - 2:00 

- Dummy data creation manually in live for testing - 2:05 - 2:15
    product
    product division mapping 

- Testing with Durgesh - 2:30 - 2:43, 3:15 - 3:30

- Order Invoice Verification & ZBM Notification Changes - 3:30 - 4:26
    - Send notification to tagged users’ ZBM(s) instead of only the order creator’s ZBM.    


# ___________________________________________________________________________________________________________

# 12-01-2026

## Miscellaneous
- 10:11 - 10:35
- Add Worklog - 10:35 - 11:00
- 11:00 - 11:18, 11:24 - 11:40  
- 12:50 - 12:59
- Weekly meeting data prepare - 11:45 - 12:00 

- meeting with harsh - 2:40 - 2:55
    regarding how to import old offline orders in empowerhh

- 2:55 - 3:05

- Practical Task Checking (03:05 – 03:40)
    - Reviewed Nirmal Joshi’s practical task and shared detailed feedback with Ravi via email.


- Weekly Meeting - 5:00 - 5:45

- Interviewer documentation – 7:55 to 8:25
    - Created a sheet documenting interviewer names, status, and reasons, with help from Ravi Bhai.

## Empower HH
- Display Chemist name as per PAN card and PAN card no. in Chemist List - 1:19 - 1:30, 4:32 - 4:40, 6:40 - 6:50

- Komal requested product change for Order ID: 593 - 1:30 – 2:00, 5:45 - 6:10
    - Manually added the product
    - Recalculated PTR, discount, and net values
    - Removed existing produvt in order 
    - send mail to stockist manualy regarding order details  

- Add/Edit User Page – Office Location Dropdown Display Fix - 6:50 - 7:20
    - Display the Office Location dropdown on Add/Edit User page

- maven data sync verify - 11:40 - 11:45,

- Manual Invoice Correction – Order #00553 (Requested by Komal) - 12:15 - 12:50
    - Invoice issue fixed for Order #00553 – extra product was added by mistake; corrected and verified manually.

- Otp not going in chemist number issue checking - 3:40 - 4:20, 4:40 - 5:00, 6:10 - 6:40
    - issue is chemist number have 11 digit so it was issue 
    - they data came from mavens sheet 
    - manualy checked howmany chemist not have proper phone number from mavens sheet
    - Created CSV for that user and send mail to Komal ma'am

- OTP Not Received Issue – Chemist Phone Number Validation - 3:40 - 4:20, 4:40 - 5:00, 6:10 - 6:40
    - Investigated OTP not being delivered to chemist mobile numbers
    - Identified the issue: some chemist phone numbers contain 11 digits, causing OTP failure
    - Confirmed the data source as Mavens master sheet
    - Manually checked and identified chemists with invalid phone numbers
    - Created a CSV of affected chemists and shared it with Komal Ma’am via email


# ___________________________________________________________________________________________________________

# 13-01-2026

## Miscellaneous
- 9:43 - 9:58
- 10:08 - 10:20

## Empower HH
- maven data sync verify - 10:20 - 10:30

- Order Approval api changes - Display login user releted data first - 10:30 - 11:20, 12:20 - 01:20

- Doctor and Chemist data state mismatch issue - 11:20 - 12:20
    manully run sql query to updated correct state

- Order Approval api changes, issue for division head - 3:20 - 4:45

## Cost Management
- User Sync from LE - 12:40 - 2:55, 3:01 - 3:20


# ___________________________________________________________________________________________________________

# 19-01-2026

## Miscellaneous
- 11:12 - 11:30
- Electricity issue - 3:40 - 4:00

- Add Worklog - 7:25 - 8:00

## Empower HH
- Incremental data api change - 11:30 - 12:10
    store state only from new csv, removed old code for storing state (Doctor, Chemist, Employee)

- Incremental data sync - 12:10 - 12:55, 1:13 - 1:25, 3:15 - 3:35
    https://empowerhh.com/apiV3/sync_doctors?date=2026-01-19
    https://empowerhh.com/apiV3/sync_chemists?date=2026-01-19

    https://empowerhh.com/apiV3/sync_employee?date=2026-01-19
    https://empowerhh.com/apiV3/sync_employee_account_manager_code?date=2026-01-19
    https://empowerhh.com/apiV3/sync_employee_role?date=2026-01-19
    https://empowerhh.com/apiV3/sync_employee_acc_mgr_relation?date=2026-01-19

    https://empowerhh.com/apiV3/sync_users_city_state?date=2026-01-19
    https://empowerhh.com/apiV3/sync_addresses?date=2026-01-19
    https://empowerhh.com/apiV3/sync_employee_division?date=2026-01-19

    https://empowerhh.com/apiV3/cron_apply_effective_hierarchy
    https://empowerhh.com/apiV3/sync_sbm_mapping_mavens?date=2026-01-19
    https://empowerhh.com/apiV3/apply_sbm_mapping_to_hierarchy

    https://empowerhh.com/apiV3/sync_user_doctor_mapping?date=2026-01-19

- incremental synced data verify - 5:40 - 6:00, 6:13 - 7:00
    verified data
    created sheet which not approved but that have orders

- Order Approval API Changes - 1:25 - 2:36 ,3:06 - 3:15, 3:35 - 3:40, 4:00 - 5:00, 7:00 - 7:25
    - Updated the order approval API to update status to tagging approved only when doctor division matches product division
    - Verified that if the user has _4D & _9D but the doctor has only _9D, then only _9D records have their status updated
    - Ensured that records from other divisions (e.g. _4D) are not affected
    - Tested the changes with Durgesh
    - Identified an issue during testing and fixed it
    - Uploaded the updated changes
    - Re-tested all scenarios and confirmed the functionality is working as expected

- Upload latest code in UAT - 5:00 - 5:20

- Disscuss with durgesh to testing order approval changes - 5:20 - 5:40, 6:00 - 6:13

# ___________________________________________________________________________________________________________

# 20-01-2026

## Miscellaneous
- 10:30 - 10:45
- 11:19 - 11:30 

- 1:32 - 1:38
- 4:20 - 4:40
- Add Worklog - 6:50 - 7:20

## Empower HH
- Disscuss with durgesh to testing order approval changes - 10:45 - 11:00, 12:35 - 12:40, 
- Data prepare for testing - 11:00 - 11:15
    doctor data
    user - doctor mapping
- Delete chemist manualy which not included in mavens sheet - 4:40 - 4:55, 6:20 - 6:50

- Order Export changes - Order Custom export and Order Custom export (multi invoice) both - 7:20 - 08:05
    displayed order created by user's name and employee code 

## Cost Management
- User Sync from LE - 11:30 - 11:55, 12:00 - 12:35, 12:40 - 1:10, 2:10 - 4:17
    - Created API for fetching user related data (users,role_user,project_user,user_project_master)
    - User Sync Job Queue created (users,role_user,project_user,user_project_master) 
    - Testing in Local
    - job queue not working in my local system, it takes time to check issue , but issue not found
    - uploaded changes in le_worklog and cost_management

- Upload in live (le_worklog and cost_management) - 4:55 - 5:55
    git issue
    siddh old code not merged with master
    merged siddh code and reupload my code 

- User sync changes - password sync - 5:55 - 6:20


# ___________________________________________________________________________________________________________

# 21-01-2026

## Miscellaneous
- 10:42 - 11:00

## Empower HH 
- Deployment & Testing - 11:00 - 11:25, 11:30 - 12:45, 5:05 - 5:30, 5:50 - 6:05
    - Deployed and tested Order Export, User Add/Edit, and Chemist PAN details changes in UAT.
    Time: 11:00 – 11:25

    - Manually deployed User Add/Edit and Chemist PAN details changes to Live.
    Time: 11:30 – 12:45

    - Deployed Order Approval and Order Creation changes to Live and verified functionality.
    Time: 5:05 – 5:30, 5:50 – 6:05

- Offline Order Import - 12:45 - 1:25, 1:44 - 2:00, 2:40 - 3:15
    - Started development of new Order Import functionality to import offline orders.
    - The functionality is partially completed: some columns are being imported successfully, while remaining data mapping and validation are still pending.

- Send Order Details to Stockist mail changes - 3:15 - 3:50
    - Display doctor UNI instead of clinic name
    - uploaded in live and tested

- Implemented create/edit order changes to store division_id for each order product, ensuring it is matched based on doctor and product divisions. - 4:25 – 5:05, 5:30 – 5:50

- Order Division Mapping & Tagging Validation - 3:50 - 4:05, 6:05 - 7:00
    - Created and executed SQL queries in UAT to backfill division_id for existing order products.
    Time: 6:05 – 6:15

    - Created and executed SQL queries in Live to backfill division_id for existing order products.
    Time: 6:15 – 7:00

    - Identified cases where order tagging was approved by an incorrect Division Head (division mismatch) and manually verified such orders using SQL queries.

    - Discussed the issue and findings with Harsh and Ravi Bhai.

    - Root Cause Analysis:
    This issue occurred due to an earlier implementation where _9D Division Heads were allowed to approve _4D division orders based only on division code. At that time, doctor–division validation was not included, which resulted in incorrect tagging approvals.

- Doctor List API change- 7:30 - 8:00
    - Displayed only doctors mapped with chemist and stockist
    - Changes uploaded to UAT and tested

# ___________________________________________________________________________________________________________

# 22-01-2026

## Miscellaneous
- 10:23 - 10:45

- Practical check - 3:20 - 3:45

## Empower HH
- Order Custom Export – Multi Invoice Fixes & Enhancements - 10:45 - 11:15, 11:22 - 1:00
    - Fixed incorrect tagging amount calculation in multi-invoice order custom export.
    - Added Net Value display for cases where orders were not tagged or invoice was not uploaded.
    - Corrected order tagging amount to display actual values.
    - Updated export to display ZBM and Division Head employee codes along with names.
    - Resolved special character (₹, →) encoding issue in CSV export.
    - Changes uploaded to UAT and tested successfully.

- Chemist List changes - change column sequense of pan card no and pan card name - 10 min

- Verified chemist master data (Mavens sheet) and informed Komal Ma’am about PAN card data mismatch issue via email - 2:50 - 3:20

- Offline Order Import - 6:40 - 7:40
    - Reviewed and analyzed CSV mapping for multi-invoice data; changes are in progress and pending completion.

# SG Vetcare - RMIS
- Project Setup - 2:20 - 2:40

- Check IN-OUT Report Export changes - 2:40 - 2:50, 3:45 - 4:10
    - change column name to Tachometer Check Out Km, Tachometer Check In Km instead of check in km and check out km

- Discuss with durgesh about MDVR Report changes - 4:15 - 4:35

- Quarterly MDVR Report changes - 4:35 - 5:10
    - Added month-wise totals for Doctor Visit, Chemist Visit, Stockist Visit, and Farmer Visit in the quarterly MDVR report. 

- MDVR Report changes - 5:10 - 6:20
    - Added and displayed Unique Doctor count and Repeated Doctor count in the MDVR report summary.

# ___________________________________________________________________________________________________________

# 26-01-2026

## Miscellaneous
- 11:20 - 11:45
- le_worklog & cost_management: Discussed new task changes with Ram Sir - 12:45 - 12:55
- Empower HH: Reviewed existing task list and estimated time requirements - 2:36 - 3:18
- Weekly meeting prep: Listed previous week’s tasks and current week’s task points for discussion - 3:18 - 3:45
- 26-01-2026 office activity - 5:00 - 6:30

## Empower HH
- Order Import (Offline Orders) - 11:45 - 12:45, 12:55 - 1:20, 3:45 - 4:30, 4:40 - 5:00, 6:30 - 8:15
    - Implemented full CSV import flow for offline orders with multi-invoice support.
    - Mapped doctor, chemist, stockist, products, invoices, tagging, and SPE assignments from sheet to system.
    - Added division matching (doctor × product), chemist availability handling, and reference date storage.
    - Stored raw sheet data in separate table for audit and created complete order logs for import actions.
    - Handled employee code parsing from sheet (e.g., Created By, ZBM, Division Head).


# ___________________________________________________________________________________________________________

# 27-01-2026

## Miscellaneous
- 10:35 - 10:45

## Empower HH
- Order Import (Offline Orders) changes - 10:45 - 11:20, 11:30 - 11:45, 12:20 - 1:15, 1:35 - 1:45, 2:20 - 2:30, 4:05 - 4:17, 4:24 - 5:50
    - Implemented division/department mapping from CSV during import
    - Handled existing imported orders to avoid duplication
    - Added Order Import button in UI
    - Added Sample CSV file for reference
    - Performed testing of import flow

- Order Export - Multi Invoice changes - 11:45 - 12:20
    - Fixed division name logic in export to correctly map based on doctor division and product division (previously showing incorrect division).


## SG Vetcare (RMIS)
- upload all latest changes in live with siddh - 2:30 - 4:05
- Reports (MDVR & Quarterly MDVR) issue - 5:50 - 6:00, 6:10 - 7:50
    - Identified and fixed Leave & Worked Days calculation issue in reports
    - Updated logic for accurate attendance counts
    - Deployed changes to UAT and Live and verified output

# ___________________________________________________________________________________________________________

# 28-01-2026

## Miscellaneous
- 10:23 - 11:12
- KRA form filling - 6:25 - 7:05

## Empower HH
- Order Import changes upload in UAT and Testing - 11:22 - 12:20
    - Permission issue solved

- Order Import changes - 12:20 - 1:05, 1:25 - 2:04, 2:42 - 3:40 
    - Resolved invoice total & discount calculation issue for multi-product invoices

- Discussed with Durgesh regarding order import functionality - 3:40 - 3:55

- 3:55 - 4:17, 4:26 - 4:35

- Fixed issue where order details were not showing for some chemists due to permanent deletion - 4:35 - 6:00
    - Restored deleted chemists and managed them using status (set as Inactive)
    - Updated system to display only Active chemists across doctor mapping, chemist listing, and chemist list APIs
    - Uploaded changes to Live and tested with durgesh

- Order Import changes - 7:05 - 7:55
    - Added specific master validation (doctor/stockist/product) and resolved invoice value calculation issue (order tagging calculation for multiple user tagged in one product)

# ___________________________________________________________________________________________________________

# 29-01-2026

## Miscellaneous
- 10:23 - 10:45
- Add Worklog

## Empower HH
- Order Import changes - Testing With Durgesh - 10:55 - 11:10

- Fixed issue where order details were not showing for some chemists due to permanent deletion - 11:30 - 11:50
    - Updated chemist status from Inactive to Rejected for restored/deleted records and added condition to handle Rejected across mapping, listing, and APIs

Mavens Data Sync (Empower → Mavens)
- Account Manager Data Verification – 11:50 – 1:05, 1:25 – 1:45
    - Verified Account Manager code mapping and data flow from Empower to Mavens
    - Reviewed handling of Account Manager assignments during sync process
    - Checked Account Manager generation logic
    - Account Manager Name = User Role + Division + Headquarter
    - Noted that this is maintained as a separate master in Mavens, while not managed in Empower

- Mavens Data Sync – Users API – 1:45 – 2:25, 3:00 – 4:20, 4:30 – 5:45
    - Created secured API for syncing users data from Empower to Mavens
    - Implemented pagination, incremental sync, and logging

- Mavens Data Sync – Role API – 5:52 – 6:40
    - Implemented role sync API with incremental updates

- Mavens Data Sync – Division API – 6:40 – 7:30
    - Implemented division sync API with audit logging

# ___________________________________________________________________________________________________________

# 30-01-2026

## Miscellaneous
- 10:14 - 10:30
- 10:30 - 10:45
- Task List with details, Estimation - 12:15 - 12:35
- 3:15 - 3:30

## Empower HH
- PMS Cron API Major Update 
    - Modified existing cron API to call PMS system API for sending daily updated data from Empower
    - Updated payload structure, flow, and handling as per new PMS sync requirements

- User Data Change Sync Table Enhancement - 10:45 - 11:21, 11:27 - 12:00, 3:30 - 4:10, 4:26 - 6:02, 6:20 - 6:55
    - Enhanced existing request logging table to capture all user-related data changes
    - Integrated major updates across Add/Edit User modules and User Hierarchy Tree View for cron-based sync processing
    - update last working date when status changed
    - store changes from User Hierarchy Tree View in queue_employee_for_pms_sync
    - store changes from cron_apply_effective_hierarchy and apply_sbm_mapping_to_hierarchy effective date based Crons in queue_employee_for_pms_sync
    - store changes from Add/Edit User in queue_employee_for_pms_sync

    - Auto-update last working date on employee status change
    - Integrated hierarchy tree view changes with PMS sync queue (high complexity, extra effort)
    - Queued PMS sync from effective-date hierarchy and SBM mapping crons
    - Added PMS sync queue trigger on user add/edit actions

- Custom Order Export – Excel Format & Mapping Changes - 7:20 -  
    - Modified existing multi-invoice order export Excel sheet structure
    - Updated columns, data format, and field mapping as per new provided template


- OTP not sending to doctor (id: 65435), checked log - otp sends from our side (sms provide response: {"txId":47173,"status":"Sent"}) - 12:00 - 12:15

- Doctor not displaying chmist or stockist issue - 12:35 - 12:50
    If chemist not available then it need to dislpay only stockist but after added condition to remove Chemist which not approved from mavens this issue occurs, issue solved removed that condition

## RMIS (SG Vetcare)
- Discussion with Durgesh on MDVR Report Logic Updates - 12:50 - 1:15
    - Discussed MDVR report requirements and DA allowance calculation changes with Durgesh.

- MDVR Report – DA Allowance Calculation Enhancements - 1:35 - 2:37
    - Implemented MDVR report logic updates to correctly calculate DA allowance based on visit type, check-in/check-out presence, and stockist, chemist, doctor, and farmer visit counts.
    - Deployed changes to UAT and Live environments and validated results with Durgesh.


######
- Mail to Ramkumar - regarding account manager 

- Courier & Questionnaire Modules – Web Changes - 120
    - Updated web data display to show hierarchy-wise data instead of team-wise data.
    - Replaced all team-wise conditions with hierarchy-wise conditions wherever applicable.

- Courier & Questionnaire Modules – API Changes - 180
    - Modified APIs to fetch and return hierarchy-wise data instead of team-wise data.
    - Updated existing team-wise logic to hierarchy-wise logic in all relevant APIs.

- Offline Order Import (import file lik custom order export)

# ___________________________________________________________________________________________________________

##### PENDING
- Admin Panel - Order status change from "On Hold & Expired", send otp also - PENDING

- Revert Order Status (Admin panel), email not working - PENDING

- Dashboard load lye che e check krvu (su load lye e check krvu)

---

- On_hold and Expired exact time e thava joi - (e research krvanu che) - PENDING

---

- (WEB) Need to check datatable - after search it display data by search but page and count of records not changing - ISSUE 

--

---

- Store logs (Web & APIs)

---

- Replace user to resigned user (waiting for siddh updation) - Pending

######
