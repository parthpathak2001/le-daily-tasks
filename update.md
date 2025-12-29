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

# 08-12-2025

## Empower HH

- Testing in UAT – User Hierarchy, User Role, User Division, User Vacancy Create and Replace User Vacancy cron script changes - 10:36 - 11:26, 11:30 - 12:10, 2:29 - 5:25 , (-45 mins ), (- 40 min)
    Performed detailed UAT testing for:
        User role change (current & effective date based)
        User division change (current & effective date based)
        User hierarchy / manager change (current & effective date based)
        Vacant user creation & vacancy replacement (current & effective date based)
    Found an issue: parent code was not storing properly, causing dependent logic to fail.
        → Reported to Siddh, issue fixed.
    Re-tested all flows after fix.
    Testing took longer due to the large number of scenarios, including:
        Role changes (current & effective date based)
        Division changes (current & effective date based)
        Manager (hierarchy) changes (current & effective date based)
        Vacancy creation (current & effective date based)
        Vacancy replacement (current & effective date based)

- Cron Script Update (Role Change Effective Date) -  - 40 mins
    Updated “role change based on effective date” cron script:
        Ensures user status correctly changes to Active from Resigned when effective date is reached.


- check_header_authentication API – Resigned User Message - 45 mins
    Issue raised by Durgesh (“APIs not working”) was not an issue — the user was Resigned, so data was not supposed to display.
    Discussed the scenario with Durgesh and Ronak for correct flow.
    Updated API to display a proper message when a resigned user tries to access the system while already logged in.
    Uploaded changes to UAT and tested.

- User Hierarchy Export Enhancements & Testing - 12:10 - 1:33, 5:25 - 5:47, 5:52 - 6:50
    Added logic to identify any resigned or deactive user in the hierarchy (NSM, DNSM, ANSM, ZBM, RBM, SBM, ABM, SBE, BE).
    Updated export to display such users’ names in red color and append status labels “- RESIGNED” or “- DEACTIVE” next to their names.
    Ensured BE-level resignation highlights the entire row in red, while parent-level resignation highlights only the respective hierarchy columns.

- Order Invoice – Unit Testing (With Durgesh)
    Durgesh reported an issue in multi-invoice upload — only the last invoice was showing on the web.
    Re-tested the flow together with Durgesh.
    Verified that all invoices were displaying correctly — no issue found.

## Miscellaneous
- Add worklog - 6:50 - 7:10, 7:25 


# ___________________________________________________________________________________________________________

# 09-12-2025

## Empower HH
- 10:37 - 10:55

- User Hiearchy check - 10:55 - 11:21, 11:30 - 12:55,
    Roshan sent mail and said they checked hiearchy wise tree there are some employees missing 
    User hiearchy checking manually
    send reply mail

- Order Data delete manuly requested by Durgesh - 20 mins

- Meeting with client, regarding data sync with PMS - 12:55 - 1:50

- mail to roshan regarding export user hierarchy confusion - 1:50 - 2:14

- Order details email to stockist on order approval - 3:00 - 3:30
    - update to display doctor name when chemist name is missing
    - changes uploaded in UAT

- Sync doctor from Mavens script changes — fixed dummy doctor UNI change issue by adding flag to prevent UNI update for dummy doctors - 3:45 - 4:18, 4:38 - 5:05

- Notification count API changes – modified pending tagging approval check for ZBM & Division Head to include tagging_processing + tagging_processing_partially statuses. - 30 min
    changes uplaoded in UAT

- Order Approval list api changes - sorting changes - 5:05 - 5:37
    - Implement sorting updates (status priority + latest order first)

## RMIS (SG Vetcare)
- Reports -> Monthly Allowance  report - export Quarterly MDVR Report changes -  3:30 - 3:45, 5:37 - 5:40, 5:48 - 6:30
    change heading to Worked day in place of Leave and Leave in place of Worked Days
    uploaded in UAT and Tested

- Reports → Monthly Allowance Report → MDVR Export Changes - 6:30 - 7:45
    Working on implementation for Set-wise data display in MDVR export
    Analyzing and understanding existing MDVR report code structure

## Miscellaneous
- Add worklog - 7:45 - 8:20


# ___________________________________________________________________________________________________________

# 10-12-2025

## Empower HH
- scheduld meeting mail send to Roshan - 11:40 - 11:55

- Meeting with roshan - 12:30 - 1:30
    User hierarchy issue and discussion
    employee name not proper issue
    
- Employee sync script run to make name of employee proper - 1:30 - 1:45

- Cron script set in UAT server - 7:25 - 8:10
    minor cron changes done and uploaded in UAT

## RMIS (SG Vetcare)
- 10:23 - 10:50
- Monthly Allowance Report Enhancements -> MDVR Export changes - Set-wise Data Implementation – 10:50 - 11:15, 11:21 - 11:40, 11:55 - 12:30, 2:44 - 4:26, 4:37 - 5:40
    - Analyzed and understood the existing report generation logic
    - Updated MDVR cron (user_mdvr) to store set-wise records
    - Modified Monthly Allowance export to display set-wise data
    - Implemented correct sorting sequence (set-wise → date-wise)
    - changes uploaded in UAT

- Added “Potential Revenue Category” (A/B/C) dropdown in Doctor Add/Edit page - 5:40 - 5:58, 6:04 - 6:50 
    - uploaded changes to UAT and tested


## Miscellaneous
- Add worklog - 6:50 - 7:25

# ___________________________________________________________________________________________________________

# 11-12-2025
- 10:21 - 10:45

## Empower HH
- watch recording of tommorow meeting and checked hiearchy issue and explained to durgesh to test some users hierarchy  - 12:05 - 12:30

## RMIS (SG Vetcare)
- Meeting with client - regarding current works updates - 12:00 - 12:07

- Routes-> Tour Plan Approval - Excel export feature added and implemented - 11:00 - 11:28, 11:41 - 12:00, 12:30 - 1:30, 2:20 - 3:05, 3:45 - 7:05
    - Faced many issues during testing.
    - Fixed one issue, then another appeared repeatedly.
    - Resolved missing data problems, including Joint Visit requests not showing


## Pucho AI
- Help dharmesh to setup template in Laravel - 3:05 - 3:45
    image not displaying
    discuss how he can manage image dynamicaly

## Miscellaneous
- Add worklog - 7:05 - 7:30



# ___________________________________________________________________________________________________________

# 12-12-2025
- 9:55 - 10:15

## RMIS (SG Vetcare)
- Meeting with client - 12:30 - 1:20
    regarding new report changes (Check in/out report, Monthly allownace report)


- apiv2/daily_allowance_summary API changes – 10:15 - 11:10
    Added total_hours calculation based on Check-In and Check-Out time
    Uploaded changes to UAT and tested

- apiv2/chemist_visits API changes checked – 11:10 - 11:20
    display chemist mobile number
    Mobile number was already present in API response
    No code changes required

- change in all message template "Rakesh Pharmaceuticals" to "Rakesh Healthcare (India) Limited" - 11:20 - 11:35, 12:05 - 12:30

- Discussion with durgesh regarding report changes - 11:35 - 12:05

## Empower HH
- User login history not displaying issue, issue checked but issue not solved - 1:50 - 2:54

## Miscellaneous
- Meeting with Ravi and Ram regarding Projects current works - 15 min


# ___________________________________________________________________________________________________________

# 15-12-2025

## Empower HH

- Reset User Device / Login History Issue Check – 11:02 – 11:25, 11:45 – 12:00, 12:20 – 1:25, 2:09 – 2:45
    - Checked issue where user login history is not displaying properly when the app is uninstalled without logout and the same device is used again.
    - Also checked Dany login issue and found that data is not displaying because the same device ID already exists in old records for another user.

- Courier Notification Issue Check – 2:45 – 3:55
    - Checked issue where courier add/edit notification is not sending.
    - Found that notification is not working because old notification code is being used.


## RMIS (SG Vetcare)
- Chemist Order List API – Mobile Number Addition - 12:00 - 12:20
    - Updated Chemist Order List API to include chemist mobile number.
    - Uploaded changes to UAT.


- SMS Message Not Sending – Issue Check (With Durgesh) - 03:55 - 4:19, 4:26 - 5:00
    - Found root cause: message text was changed in the application, but the same change was not updated on the SMS provider server, so messages failed.
    - Tested and discussed the issue with Durgesh.

- Check In–Out Report Enhancements – 5:00–6:30, 6:50–8:00
    - Added Doctor Completed / Pending visit counts.
    - Added Chemist Completed / Pending visit counts.
    - Added Stockist Completed visit count.
    - Added Farmer Completed / Pending visit counts.


## Miscellaneous
- finding pdf generation code, code creation by jatan, requested by Ram sir - 6:30 - 6:50

- add worklog - 11:25 - 11:45, 8:00 - 8:10

# ___________________________________________________________________________________________________________

# 16-12-2025

## RMIS (SG Vetcare)
– 10:10 - 10:20

- Check In–Out Report Enhancements – 10:10 - 12:10, 3:30 - 3:40
    - Added new fields: Date, Role, Attendance, Total Hours, and Total Call
    - Uploaded changes to UAT and verified functionality
- Reports -> Monthly Allowance report - 12:10 - 12:25
- Routes → Tour Plan Approval — fixed issue where “#Dr. Planned” was not displaying correctly - 12:25 - 12:45
- Create New API – get_approved_set_dates -  12:45 - 2:48
    - Created new API to fetch approved SET visit dates with correct submission join and date filtering.


## Empower HH
- Script for manage multi invoice for old orders - 3:40 - 4:10, 4:16 - 4:55, 5:30 - 7:20

- durgesh raised issue cheking - 4:55 - 5:30
    order approval list displaying order for approval but tagging approval pending popup not displaying issue - checked issue it is not an issuse logged-in user is authority user so it display order in approval list because user is mapped with stickist and popup not displaying because order tagged user is not in hiearchy of logged-in user  

## Miscellaneous
- Add worklog - 7:20 - 7:45

# ___________________________________________________________________________________________________________

# 17-12-2025
- 10:28 - 10:45

## Empower HH
- Script for manage multi invoice for old orders - 10:45 - 11:55, 12:40 - 1:00

- PHP team internal meeting - 11:55 - 12:40
    reagrding project task management

- Taking database backup from live to test in UAT live data - 1:00 - 1:20  

- upload all API changes, database changes in UAT, created API V3 - 1:20 - 2:05, 2:25 - 2:48
    - upload live data in UAT
    - run script for manage old order to new to test that script in UAT

- Upload code in Live- 3:06 - 3:50, 4:23 - 8:00
    api changes in API v3 
    order module changes (web)
    doctor module changes (web)
    stockist module changes (web)
    Unit Testing


- dummy data creation in Live server - requested by durgesh - 3:50 - 4:15
    Doctor, Chemist, Stockist, Product, Doctor mapping, Product mapping 

# ___________________________________________________________________________________________________________

# 18-12-2025
- 10:28 - 10:45

## Empower HH
- Created two cron scripts:  - 11:10 - 11:55, 12:15 - 2:06, 2:31 - 2:47, 3:09 - 4:00
    Sync SBM (BE/SBE) mapping data from Mavens
    Update SBM (BE/SBE) mapping in users_hierarchy
    uploaded in Live 
    Cron url changed

- Order List - new status added in filter  - 11:55 - 12:15

## Neeti Reports
- Neeti report server setup - 4:50 - 6:15
    snowflake file check
    try to connect server but not connecting  

## LE Worklog
- Task understanding with Ram sir - 6:15 - 6:25
- 6:25 - 6:40

- User Worklog & Monthly Worklog CSV Export Issue Fixed – 6:40 – 8:00
    - Tried multiple approaches but the issue was not resolved initially.
    - Identified extra output buffer as the root cause.
    - Fixed the issue by clearing the output buffer using ob_end_clean().
    - CSV now downloads correctly without a blank first row.

- Employee Worklog - Update status action form changes - 8:00 - 8:20
    - If status set to "not done" it read only minute box and when submit it returns validation in minutes its issue - issue solved

## Miscellaneous
- Finding PDF code with Ramsir done by Jatan - 20 min
    + 20 min to find in LSPC 

- 4:15 - 4:50


# ___________________________________________________________________________________________________________

# 19-12-2025

- 10:12 - 10:40

## Le Worklog
- Employee Worklog - Create Employee Worklog – Module-wise & User-type-wise Hours Validation - 11:33 - 12:30 - 12:30 - 1:05, 1:25 - 1:55, 2:59 - 4:05
    - Implemented module-wise and user-type-wise hours validation while creating Employee Worklog.
    - Added backend validation to calculate allowed minutes based on module estimation and user department, and to restrict worklog entry when limits are exceeded.
    - Added jQuery validation to display remaining minutes on module selection and validate minutes on input change and form submit.
    - Performed unit testing to verify different scenarios and edge cases.

    - Backend validation: 60 mins
    - jQuery validation: 120 mins

    - Reason for extended time:
        This task involved handling multiple scenarios, syncing backend and frontend validations, and ensuring existing limits (like single task max minutes) were not affected. Extra time was spent testing edge cases to avoid incorrect hour calculation.


## Empower HH 
- Old Order Migration – Completed Status Fix - 1:05 - 1:25
    - Updated migration script to process only completed orders.
    - Uploaded changes to live server.
    - Executed the script on live.
    - Manually verified the migrated data.

- Reset User Device / Login History Issue Check – Checked issue related to user device reset and login history; verified user data manually – 1:25–2:20

- Login API – Multi-Device Approval Issue Fixed - 4:20 - 5:45
    - Fixed issue where the same user logging in multiple times from the same device was showing multiple approval entries in admin panel.
    - Now, the same device is shown only once per user in admin approval.
    - Earlier, approval was triggered only for the 3rd user. Additional users (4th, 5th, etc.) were not going for approval.
    - Updated Login API logic so when 2 users are already logged in, every additional user (3rd, 4th, etc.) correctly goes for admin approval.

- User Attempt List & Approval Action Update - 5:45 - 6:40
    - Updated admin approval listing to show only pending device login requests.
    - Removed approved and rejected records from the user attempt list.
    - Ensured the same device ID is displayed only once per user.
    - Updated approve action to correctly add the approved device to the active login device list.

- Testing with Durgesh – Tested login flow, device approval, and re-login scenarios to verify recent fixes – 6:40–6:50, 7:10–7:45

- Login API changes - Approved Device Handling Fix - 6:50 - 7:10
    - Fixed issue where an already approved device was still going for admin approval during login.
    - Updated login logic to check approved device status and allow login directly.
    - Ensured approved users are not sent for approval again on the same device.

## Miscellaneous
- Add worklog - 10:40 - 11:15, 7:45 - 

- System issue discuss with Rahul bhai - 11:15 - 11:25


# ___________________________________________________________________________________________________________

# 22-12-2025

- 10:22 - 10:40

## Empower HH 
- Sync mavens master data - 11:20 - 11:50, 11:55 - 2:10, 2:30 - 2:45, 3:08 - 4:19, 4:32 - 5:10, 6:10 - 6:40
    - Files:
        FirsttimeBackup/Master/Updated Master Data/New Backup/Fri Dec 19 19:18:41 IST 2025/employee.csv
        FirsttimeBackup/Master/Updated Master Data/New Backup/Fri Dec 19 19:18:40 IST 2025/empaccmgrmap.csv
        FirsttimeBackup/Master/Updated Master Data/New Backup/Fri Dec 19 19:18:42 IST 2025/emprole.csv
        FirsttimeBackup/Master/Updated Master Data/New Backup/Fri Dec 19 19:18:10 IST 2025/accmgrrelation.csv
        FirsttimeBackup/Master/Updated Master Data/New Backup/Fri Dec 19 19:18:41 IST 2025/empdivision.csv
        FirsttimeBackup/Master/Updated Master Data/New Backup/Fri Dec 19 19:18:39 IST 2025/dealerdetail.csv
        FirsttimeBackup/Master/Updated Master Data/New Backup/Fri Dec 19 19:18:32 IST 2025/custaccmap.csv
        FirsttimeBackup/Master/Updated Master Data/New Backup/Fri Dec 19 19:18:36 IST 2025/customermaster.csv
        FirsttimeBackup/Master/Updated Master Data/New Backup/Fri Dec 19 19:18:55 IST 2025/sbmmapping.csv
    - Manually Checking data from sheets
    - this task take time because apis taking time to sync data so it takes time 
    - Minor code changes for logging and verification
    - uploaded latest sync changes 

- Courier Module – Notification Issue 
- upload login api changes in live 

## Miscellaneous
- Add workog - 10:40 - 10:55, 7:20 - 8:15

- System Issue Discussion & Backup Preparation – 10:59 – 11:20
    - Discussed system issues with Rahul bhai. - 10:55 - 11:05
    - Took complete system backup before formatting. - 11:05 - 11:20 

- Meta Tag Implementation Support – 6:55 – 7:20
    - Helped Tirth add dynamic meta tags on a single-page application based on URL conditions.

- Townhall Meeting - 5:10 - 6:10


# ___________________________________________________________________________________________________________

# 23-12-2025

## Empower HH
- checked data which synced in full night - 10:45 - 11:20 

- Courier Notification Issue - 11:20 - 11:55, 12:10 - 1:08
    - Checked and fixed the issue where courier notifications were not working.
    - Updated the notification logic using the latest APIs.
    - Uploaded the changes to UAT and tested successfully.

- PMS Employee Data Sync - 2:10 - 2:19, 3:00 - 4:18, 4:24 - 4:31, 4:37 - 6:25, 6:35 - 6:45 (212 minutes)
    - Reviewed PMS API document.
    - Created database table to store employee sync request and response data.
    - Developed CRON API scripts for employee create/update and deactivate sync. - 100 mins

## Neeti Report
- New Server Setup  - 1:25 - 1:55
    Mail Check
    Try to conect, not connecting 
    review mail
    try to install putty on ht server given by ravi bhai

## RMIS (SG Vetcare) 
- Chemist Order WhatsApp Template - 6:45 - 7:35
    - Created WhatsApp order confirmation template in Meta using client-provided content
    - Added dynamic variables for chemist, order ID, employee, stockist, and product details

## Miscellaneous - PENDING
- Task management with ravi bhai - 11:55 - 12:10
- Add Worklog - 10:20 - 10:45, 7:35 - 8:00
- Taken backup of all project's postman collection - 1:55 - 2:10 
- Sent email to confirm whether the shared Empower updates are working properly – 10 minutes


# ___________________________________________________________________________________________________________

# 24-12-2025

## Empower HH
- Log Employee Data Changes into PMS Sync Queue - 6:45 - 7:40
    - Logged all employee-related data changes into the PMS sync queue table. 
    - Captured employee create and update actions. 
    - Logged updates related to employee details, division, role/designation, and reporting hierarchy. 
    - Stored the full request payload in the employee_pms_sync_queue table for each change.

- Hierarchy Data Discrepancy Check (Derma & Vitality) – Raised by Roshan - 11:05 - 11:22, 11:32 - 11:43, 11:50 - 1:10, 1:38 - 2:10, 2:40 - 3:20
    - Investigated hierarchy data discrepancy issue raised by Roshan.
    - Manually checked Derma and Vitality hierarchy data.
    - Verified Empower database data with source sheet and client observations.

    - Updated employee sync script to handle resigned users (status update when remarks = Resigned).
    - Uploaded latest employee data from Live to UAT.
    - Verified Kerala State hierarchy data.
    - Checked all reported discrepancies and shared confirmation with Roshan.

- User Login functinality checking  - 4:50 - 5:15, 5:30 - 6:10
    - Tested with Durgesh by logging in from 3–4 devices.
    - Verified multi-device approval flow.
    - Observed issue: after admin approval, the first device ID is not deleted from the Reset User Device page.
    - Implemented changes to fix the issue and re-tested the flow to confirm the device record is now removed correctly after approval
    - Also tested whether approval is required again on the next login after approval and verified the behavior.

- Reset User Device page changes - 5:15 - 5:30
    - Reset User Device page updated to display only active records.
    - Excluded soft-deleted device data (deleted_at IS NULL) from the listing.

## RMIS (SG Vetcare)
- Update Chemist Order WhatsApp Template (chemist_order_confirmation) - 3:20 - 4:23, 4:31 - 4:50, 6:20 - 6:45
    - Updated the chemist order WhatsApp template to send complete order details, including multiple product details.
    - Shared the updated template with the client for approval.
    - Client requested to display products one by one on separate lines.
    - Attempted to display products in separate lines, but WhatsApp template sending failed due to formatting limitations.
    - Adjusted the product display to a supported format.
    - Updated the WhatsApp phone number as shared by the client after approval.

## Miscellaneous
- 10:10 - 10:23
- Add Worklog - 10:25 - 11:05, 6:10 - 6:20

# ___________________________________________________________________________________________________________

# 26-12-2025

## Miscellaneous
- 10:15 - 10:30
- Add Worklog - 10:30 - 10:45, 11:00 - 11:14, 7:10 - 7:20

## Empower HH
- Upload & Test Latest Changes on Live Server - 11:27 - 1:20
    - Uploaded latest Login API changes on Live server.
    - Updated Reset User Device page changes.
    - Fixed Courier notification not sending issue.
    - Since the Live server does not have Git access, code changes were uploaded manually, and all modified files were carefully updated.
    - Performed post-upload testing on Live to ensure all features are working as expected.

-  Mavens Incremental Master Data Sync (Date-wise - 20-26) - 10:45 - 11:00, 1:34 - 2:47, 3:19 - 7:10
    - Performed date-wise incremental sync of Mavens master data for the period 20 to 26.
    - Executed 13 sync scripts for each date to update master records.
    - Synced the following data for each date:
        Employee
        Employee Role
        Employee Division
        Dealer
        Customer
        Employee Hierarchy
        Employee–Doctor Mapping
        SBM Mapping
    - Manually checked all synced data to ensure it is correct.

- Setup Crons on Live Server - 7:20 - 
- Added cron entries to execute the following APIs:
    -  sync_chemists
    -  sync_doctors
    -  sync_employee
    -  sync_employee_account_manager_code
    -  sync_employee_role
    -  sync_employee_acc_mgr_relation
    -  sync_users_city_state
    -  sync_employee_division
    -  cron_apply_effective_hierarchy
    -  sync_sbm_mapping_mavens
    -  apply_sbm_mapping_to_hierarchy
    -  sync_user_doctor_mapping
---

# ___________________________________________________________________________________________________________

# 29-12-2025

## Miscellaneous
- 10:23 - 10:40
- Add Worklog - 10:40 - 11:10, 3:30 - 3:55
    increase Estimation hours of modules
    added additional tasks
    
- previous week tasks - Townhall meeting - 11:10 - 11:17, 11:25 - 11:35
- System Issue - 12:10 - 12:40
    - Blue Screen Error - 3 times
    - discuss with Rahul bhai and deleted some data from C drive 

- Townhall meeting - 5:00 - 6:00

## Empower HH
- Datatable issue checking - 11:35 - 12:10, 12:40 - 12:50,: 3:55 - 4:05, 4:14 - 5:00, 6:00 - 7:00
    - Checked all datatable - 11:35 - 12:00
    - solve issue - 12:00 - 12:10, 12:40 - 12:50,: 3:55 - 4:05, 4:14 - 5:00, 6:00 - 7:00
    - Chemist list - count issue
    - Product list - count issue
    - User List - returns to dashboard
    - User Groups - Sorting not working

- Division Head Pending Approval Popup Issue - Raised by Komal ma’am - 12:50 - 1:15, 1:35 - 2:33, 3:25 - 3:30
    - Issue: Pending approval popup was showing incorrectly for Division Head because some products are mapped to multiple divisions.
    - Fix: Updated the logic to validate doctor–division mapping so the popup shows only when there are correct pending approvals.
    - uploaded in Live

- Order Create – OTP Not Received by Chemist - Raised by Komal ma’am - 3:04 - 3:25
    - Issue: Issue raised by Komal ma’am. OTP was not received by the chemist during order creation.
    - Check Done: Verified manually and checked logs. OTP is being sent successfully from our side.

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
