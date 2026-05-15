# ___________________________________________________________________________________________________________

# 02-02-2026

## Miscellaneous
- 11:05 - 11:09, 11:12 - 11:20

## Empower HH
- EMPOWER HH – Clarification mail sent on Emp Master fields, Account Manager master requirement, and date field confusion (Maven-provided sheet for Empower API response format) - 12:20 - 1:20
    - Prepared clarification points on Emp Master fields (Location, City, Country)
    - Clarified requirement for Account Manager master setup
    - Raised confusion on Account Manager date field mappings
    - Reviewed client replies and gained clear understanding of data mappings and expectations.

- Courier Hierarchy (team to hiearchy) API and Web Changes - 1:25 - 2:43, 3:10 - 5:25, 5:45 - 6:15
    - New API created for Questionnaire Result – Division-wise data retrieval (get_my_division_results)
    - New API created for Questionnaire Result – State-wise data retrieval (get_my_state_results)

- mail checking - 7:15 - 7:30

- Discussion on Maven data with Prashantbhai and Shubhambhai - 6:50 – 7:15

## RMIS (SG Vetcare)
- MDVR Report – Fixed DA allowance not showing issue by removing activation/expiry date condition from DA config fetch - 11:20 - 12:10
    - Changes uploaded to both UAT and Live environments and successfully tested

- monthly_allowance_report issue - 5:25 - 5:45
    - its not an issue, need to run cron

- Enabled President & Vice President web login access (earlier only Admin) — 6:15 – 6:50

# ___________________________________________________________________________________________________________

# 03-02-2026

## Miscellaneous
- 10:29 - 10:45

## Empower HH
- 10:45 - 11:08, 11:13 - 1:08, 1:30 - 2:10, 2:42 - 3:15
    - City Master Import - 11:13 - 11:45
        - create new table, imported csv from Mavens 
    - Location master Import - 11:45 - 12:25
        - create new table, imported csv from Mavens 
    - State master linked with country - 12:25 - 1:05
        - verified all state of mavens with empower's state
        - verified all head quarter of mavens with empower's head quarter
    - Account Manager Master - 1:30 - 2:10, 2:42 - 3:15
        - understanding flow of managing account manager

- Mavens script date condition updates - 3:15 - 4:15
    - Updated start date logic to process today & past records (startdate ≤ today)
    - Updated resigned handling to include past end dates (enddate ≤ today)
    - Implemented in below given scripts:
        - activate_today_roles
        - activate_today_divisions
        - activate_today_account_manager_codes
        - apply_effective_hierarchy_changes
        - activate_today_user_doctor_mapping
    - Uploaded in Live


## RMIS
- MDVR reports changes - 4:15 - 4:25, 4:43 -  7:40
    - DA Allowance calculation changes
    - Total changes calculation changes
    - Grand Total calculation changes
    - Set Wise data display changes - Display only Approved Sets data


# ___________________________________________________________________________________________________________

# 04-02-2026

## Miscellaneous
- 11:24 - 11:31
- Add Worklog - 8:05 -  
## RMIS
- Admin Panel Login Page Enhancement — 10:35 - 10:50
    - Updated login logic to allow all user roles to access the Admin Panel
    - Deployed changes to Live environment

- MDVR Export & Cron Update – Approved Set Filtering - 12:05 - 12:50
    - Updated MDVR export logic to fetch and display only Approved Set data (changes in cron)
    - Applied approval condition across set selection queries to exclude pending/rejected records
    - Tested changes in UAT and deployed updates to Live environment


## Empower HH
- Mavens Data Sync – Account Manager & Parent User Mapping API – 12:50 - 1:12, 1:28 - 1:39, 1:55 - 3:55
    - Developed secured APIs to sync Account Manager mappings and parent (L1) relationships from Empower to Mavens
    - Implemented pagination, incremental (date-based) sync, and detailed API logging

- Account Manager Master Import - 3:55 - 4:25, 4:40 - 5:05, 5:15 - 5:30
    - create new table, imported csv from Mavens 

- All database related changes which used for sync data to Mavens uploaded in Live and UAT - 5:05 - 5:15

- Stored city mapping in user_master, chemist_details, and doctor_master from cmpostaladdress_mavens using MySQL batch update queries  - 5:30 - 7:00, 7:40 - 8:05
    - Implemented city code to city ID updates across all related tables
    - Executed updates in limited batches to avoid MySQL timeout and locking issues
    - Additional time taken due to large data volume requiring multiple batch runs

- sync_addresses Mavens script changes - 7:00 - 7:40 
    - store city and location from cmpostaladdress.csv
    - uploaded in Live

# ___________________________________________________________________________________________________________

# 05-02-2026

## Miscellaneous

## Empower HH

- City and Location mapping updates in user_master, chemist_details, and doctor_master from cmpostaladdress_mavens using MySQL batch queries - 10:27 - 11:34, 11:43 - 1:13, 1:31 - 1:35, 1:59 - 2:07, 2:11 - 2:50 
    - Mapped city codes to city IDs and location codes to location IDs in all master tables
    - Processed only latest active address records for accurate data sync
    - Ran updates in limited batches to avoid MySQL timeout and locking issues on large datasets
    - Extra time spent due to high record volume requiring multiple batch executions and verification

- Meeting with Devansh Sir, Ravibhai and Harshbhai, regarding Add/Edit Doctor functionality (new) and new changes - 2:50 -  3:10

- Meeting with Empower Team, regarding new changes - 6:15 - 7:20


## RMIS (SG Vetcare)
- MDVR issue - 3:30 - 4:15, 4:20 - 6:15, 7:20 - 8:00
    - discussed with durgesh
    - Da Allowance calculation issue in some users - issue is in check-in check-out condition issue soved

    - Monthly Allowance Report issue - DA Allowance calculation issue, calculate based on visit type
    - uploaded in Live and Uat


# ___________________________________________________________________________________________________________

# 06-02-2026

## Miscellaneous
- 10:06 - 10:30
- 10 min discusion with durgesh about rmis mdvr issue solved

## Empower HH
- Manuly update in live, requested by komal - 10:30 - 11:22, 11:26 - 11:50, 2:05 - 2:15, 2:35 - 3:10
    - Import product as temp table, update ptr of product and if product not exist create it manually - 10:30 - 11:22, 11:26 - 11:40
    - Add Dummy Doctor given by komal ma'am - 2:35 - 3:10
    - Change Chemist state and mapped with doctor - 2:05 - 2:15

- Meeting with Empower Team - 1:30 - 2:05
    - Regarding development updates
    - Discussed HR hierarchy master data sync and automation across systems
    - Finalized twice-weekly review meetings for faster issue resolution
    - Reviewed upcoming access role functionality updates for security and control

- Explain task to siddh, account manager management from user hierarchy update - 3:25 - 4:05

## RMIS 
- Issue Discussion with Durgeshbhai and Ravibhai - 11:50 - 1:30
    - Monthly Allowance Report issue - DA Allowance calculation issue 
    - Check IN/OUT report issue
    - checking issue with ravibhai

- Check In/Out Report - Display Absent value proper - 3:10 - 3:25, 4:05 - 4:20


# ___________________________________________________________________________________________________________

# 10-02-2026

## Miscellaneous
- KRA Meeting with Ramsir and Ravibhai - 11:50 - 12:20

## Empower HH
- Discucssion with Athikur - Empower Tasks - 11:10 - 11:20
    - Check given task
    - explain PMS Sync

- Discuss with Ravi bhai about new changes - 11:20 - 11:40, 1:45 - 2:00
    - Doctor list changes
    - doctor's aadhar card related new apis
    - Doctor Manager mapping

- doctor_aadhar_mapping_list API – list doctors mapped to authority for Aadhaar verification - 3:30 - 6:30
- store_doctor_aadhar API – upload doctor Aadhaar details with in-progress status - 6:30 - 8:30

- Meeting With Mavens Team - 1:00 - 1:45 
    - Work update


# ___________________________________________________________________________________________________________

# 11-02-2026

## Miscellaneous
- Exaplain task to athikur - - 10:50

## Empower HH
- Doctor Aadhar APIs - 11:00 - 12:35, 5:30 - 6:30
    - doctor_aadhar_mapping_list API – list doctors mapped to authority for Aadhaar verification
    - store_doctor_aadhar API – upload doctor Aadhaar details with in-progress status
    - doctor_aadhar_mapping_list API changes - Added Search Filter, added reject reason filed

- Account manager code logic changes - 12:35 - 1:04, 1:30 - 2:12, 2:40 - 4:10
    - checked old data of account manager 
    - asked some confusion to Mavens team

- Sync Data to mavens API changes - 4:10 - 4:30, 4:38 - 5:30
    - send code of city, state, country, location
    - uplaoded in UAT and tested

- Doctor List API Changes — 6:50 – 7:05
    - Display only doctors having UNI or Aadhaar number.

- Doctor List Web Changes — 7:05 – 7:35
    - Display only doctors having UNI or Aadhaar number.
    - Show Doctor Code in brackets with name when UNI is not available.

- store_doctor_aadhar API Changes — 7:35 – 7:50
    - Implemented unique Aadhaar validation to prevent duplicate entries.

- Change Doctor state manully. Requesed by Komal ma'am - 7:50 - 8:00

# ___________________________________________________________________________________________________________

# 12-02-2026

## Miscellaneous
- Find Coolify Key from Ravibhai system - 15/20 minute

## Empower HH

- Notification count api changes - 10:14 - 10:29, 10:36 - 11:30
    - added is_aadhar_approval_pending for display Addar Approval Pending to Manager (is_authority = 1) 
    - Uploaded in UAT 

- store_doctor_aadhar api chnages - 12:25 - 12:55
    - update based on id 

- 11:30 - 11:40

- Meeting with Empower Team (Nilesh sir) - for testing Syncing to PMS script - 11:40 - 12:25

- Meeting with Empower Team - 1:00 - 2:10
    - Progress Meeting

- Doctor Aadhar display changes and search filter change - 1:50 - 2:10, 3:10 - 3:30

- Testing with durgesh - 3:30 - 4:15, 5:30 - 5:40
    - doctor aadhar mapping changes
    - add manualy data requested by durgesh

- Institutional change discussion with Harsh - 4:20 - 4:45

- New changes discussion with ravibhai - 4:45 - 5:00

- Mavens sync issue check - 5:15 - 5:30
    - S3 have no folder for 12-02-2026 so issue occurs
    - mail to mavens

- Order Approval API Issue - 5:40 - 6:43, 6:50 - 6:55
    - Investigated and fixed an issue where the “tagging_approved” status was displayed incorrectly for orders with multiple invoices. The problem occurred when the first invoice was approved and a new invoice was uploaded later, causing incorrect approval status visibility. Adjusted the logic to handle multi-invoice approval flow correctly.

# ___________________________________________________________________________________________________________

# 13-02-2026

## Miscellaneous

- Add Worklog - 11:40 - 12:00, 6:45 - 
- Office Activity - 3:00 - 4:15 

## Empower HH
- Mavens Testing - 10:30 - 11:00

- Meeting With Mavens team and Empower Team - 11:00 - 11:40 

- Documentation Create for sync data to mavens APIs - 11:40 - 1:00 
- Discuss with Harsh Regarding Documentation changes - 4:35 - 4:45
- Changes in documentation - 5:50 - 6:05

- Account manager management in User management - 1:35 - 2:40, 4:15 - 4:35
    - Upload in Uat

- Create Dummy User Data in UAT - 4:53 - 5:05, 5:20 - 5:25, 5:40 - 5:50

- API issue only on UAT - 5:05 - 5:20, 5:25 - 5:40
    - headers not fetched 
    - Headquarter code not stored issue solved

- Synced data from Mavens or not checked - 6:05 - 6:45

# ___________________________________________________________________________________________________________

# 16-02-2026

## Miscellaneous

## Empower HH
- Display Account Manager code in User Listing page - 8:50 - 9:10, 9:20 - 9:25 

- Synced data from Mavens or not checked - 9:10 - 9:20

- Display Account Manager code in User Details page - 9:25 - 9:40

- User Doctor mapping changes - 9:40 - 10:20
    - Selected Division and Users cannot select in another dropdown

- doctor last mapped date - store in doctor master - 10:20 - 10:55, 1:15 - 1:30

- Display Aadharcard number in Doctor Details page - 10:55 - 11:05

- (WEB) Invoice Dropdown for resend invoice OTP (invoice_uploaded and partial_invoice_upload) - 11:20 - 11:33, 11:40 - 12:25
    - Added invoice_partially_uploaded filter in Order List filter

- Upload changes in UAT - 12:25 - 12:51, 1:10 - 1:15


- Upload in Live - 1:15 - 2:22, 2:36 - 4:45
    - Make ApiV3 to ApiV4
    - DB changes
    - Aadhar changes

- Order Apprval Action api issue - 4:45 - 5:45
    - order approval not working properly
    - issue not solved

# ___________________________________________________________________________________________________________

# 17-02-2026

## Miscellaneous
- Discuss with athikur, regarding pms changes
- updates - 6:50 - 

## Empower HH

- Order Approval List and Order Tagging Approve api issue - 10:15 - 11:00
    - i checked issue, its an test case issue - given 2 same division to doctor and choosen product is also both division same, its issue

- Notification not working issue - 12:35 - 2:36, 2:53 - 4:00
    - issue is in fcm token generation

- Meeting with Empower Team - 1:00 - 2:10
    - Progress Meeting

- Upload code in live_uat - 12:15 - 12:35, 5:05 - 6:50
    - User changes
    - order changes
    - quiz changes
    - doctor changes
    - api changes

- Requestd by Komal ma'am- 4:00 - 4:08, 4:15 - 4:41
    - manuly send Order details Mail to stockist 
    - invoice otp issue check - it not issue (we send otp) 

- login api check - 4:40 - 5:05
    - it store fcm token 0 when approve for login from admin to login 

# ___________________________________________________________________________________________________________

# 18-02-2026

## Miscellaneous
- Discuss with athikur, regarding pms changes (empowerhh) - 10:03 - 10:13
- User syncing related discussion (cost management) - 10:25 - 10:45

- Add Worklog - 7:10 -  

## Empower HH
- merge code in live_uat - 10:45 - 11:20
    - cron url change apiv3 to apiv4 in live

- Discuss with durgesh, regarding test new uploaded changes - 11:25 - 11:45

- Mail to komal ma'am - 11:55 - 12:10
    - Order invoice OTPs send to mail to verify order invoice

- Invoice uploading issue after new live code setup on UAT (Live UAT changes) - 12:10 - 12:35, 1:28 - 2:00
    - it not have folders in project
    - folder/file permission issue 

- Doctor discount not displaying in discount approval listt - manual check - 2:00 - 2:30
    - Doctor discount added but not displaying to approver
    - its not an issue - it not displaying because fieldstaff state and approver state is different


- created cron_hold_pending_aadhar cron -  11:45 - 11:55, 12:35 - 1:05, 3:10 - 3:40
    – auto move pending Aadhaar records to ON_HOLD after 48 hours and store action logs in order_logs

- Order details change - 3:40 - 4:10, 4:14 - 4:50
    - Invoice OTP Resend changes
    - checmist otp not sending issue in live_uat - its not an issue chemist status is not "Approved"
    - upload code and testing

- order have multi tagging issue checking - 4:50 - 5:30
    - in single order multiple time same invoice verification proced and same product multiple time tagged issue checked 
    - it because of invoice verify using otp api called multiple times  

- Shaziya ma'am issue - 5:30 - 6:35
    - MySQL Error 1205 (Lock wait timeout exceeded) issue faced by Shaziya ma'am during quiz creation checked and handled.
    - Added try–catch and displayed “Something went wrong. Please try again.” message to avoid crash.

- Check Why Product mrp price is 1 and discussed with harsh - 6:35 - 7:10 
    - when we updated product prices i update only ptr field value not updated mrp because we used ptr not mrp from sheet so it display old value 1  

# ___________________________________________________________________________________________________________

# 19-02-2026

## Miscellaneous
- discussion with durgesh - - 10:55

## Empower HH
- Product price update - 11:00 - 11:50
    - update produxt price
    - check issue - issue is imported sheet have comma(,) in price so it store 1
    - updated that products price where is issue 
    - mail to komal ma'am

- Order details changes - 11:50 - 12:25
    - Invoice OTP resend button displaying after invoice verified - issue solved
    - uplaoded in UAT

- Order Invoice Verify Changes – 12:25 - 1:00, 3:27 - 4:56, 4:11 - 4:20
    - Added check to prevent multiple invoice verification and duplicate tagging.
    - Implemented validation to detect already verified/tagged invoices.
    - Updated error message for better user clarity.

- Meeting with Empower Team - Progress Meeting - 1:00 - 2:10

- 2:35 - 2:45

- Manuly deleted duplicate Order Tagging in Live - 2:45 - 3:00

- User Doctor maping mavens sync script changes - 4:20 - 4:35
    - Only Active User Map with doctor - condition added

- mavens data sync issue - 4:35 - 4:55
    - Check manually data - why user doctor mapping not work

- Latest Code upload on live and Tested

# ___________________________________________________________________________________________________________

# 20-02-2026

## Miscellaneous
- 6:45 -  

## Empower HH
- cron_hold_pending_aadhar changes and testing - 10:25 - 11:20, 11:30 - 11:55
    - uploaded in live

- Discusssion with Siddh - regarding new replacement user changes  


- User sync issue from mavens sync manualy check - 11:55 - 1:05, 1:25 - 1:50, 2:10 - 2:20, 2:50 - 3:45

- Mavens script changes - 3:45 - 6:15
    role, division, hierarchy related scripts changes - only Active user data update 

- Meeting with Empower Team - 1:05 - 1:25
    - Regarding new changes, previously faced issue 

- Discussion with harsh, regarding sync to mavens api changes - 6:15 - 6:45 


# ___________________________________________________________________________________________________________

# 23-02-2026

## Miscellaneous
- 11:12 - 11:21, 11:26 - 11:30

## Empower HH
- Sync users to Mavens API checking - 11:30 - 12:20, 1:05 - 3:20
    - status calculation
    - checked why other fields is null
    - test all apis again

- sync data from mavens and effective date based cron changes - 3:20 - 4:30

- User Add/Edit - Account manager code generation changes - 4:30 - 4:50, 6:30 - 7:25

- list down all api mavens script urls list with dates and manully run - 4:50 - 6:30, 7:25 - 7:45
    - employee realted all apis (employee, employee division, employee role, employee account manager code, employee hiearchy)
    - created python script to run crons manually


- upload latest code in live - 12:20 - 1:05 

# ___________________________________________________________________________________________________________

# 24-02-2026

## Miscellaneous

## Empower HH
- User division sync cron have issue - 10:30 - 11:15
    - check and find issue
    - re run script for 20-02-2026 date and verify data

- generate query to check existing data is proepr or not for employee division and employee role - 11:15 - 11:45, 11:50 - 1:00
    - manually verify data 
    - re-run activate_today_divisions and activate_today_roles to fix some mismatched data

- Client Meeting - Progress review meeting with Empower team - 1:00 - 1:50 

- 2:20 - 2:45

- order changes - 2:45 - 3:05, 3:30 - 4:50, 5:20 - 6:15
    - Order Reassign functionality

- manualy stockist add - requested by komal ma'am - 4:50 - 5:20

- User hiearchy mismatch issue  - 6:15 - 7:45 
    - issue finding
    - issues because of sync data using crons
    - issue not resolved

# ___________________________________________________________________________________________________________

# 25-02-2026

## Miscellaneous
- Add Previous Worklog - 10:15 - 10:50
- KRA form - 12:35 - 1:10

## Empower HH

- Employee division, role, hierarchy Issue solving - 10:50 - 12:35  
    sync all employee related master data

- Meeting with Shaziya ma'am & Jammel- 1:25 - 4:05

- User sync issue check - 4:20 - 4:55

- New scripts - for data store and sheet store - 5:15 - 5:50, 6:10 - 6:55
    - save_employee_log
    - save_employee_account_manager_code_log
    - save_employee_acc_mgr_relation_log
    - save_employee_division_log
    - save_employee_role_log



- order issue check - Order status changes to On_hold issue - 5:50 - 6:10

- User hiearchy checking manually - 6:55 - 7:20

# ___________________________________________________________________________________________________________

# 26-02-2026

## Miscellaneous

## Empower HH
- New log storing script upload in live and run script - 9:55 - 10:05, 10:20 - 11:25

- checking quiz data manually in database with ronak - 10:05  -  10:20
    - checking time consuming, take time, total time calculation

- maually add tesing doctor data - requested by durgesh - 11:25 - 11:45

- Order reassign changes- 11:54 - 12:30
    - order rassign changes - display reassign button to admin if order status is on_hold or expired
    - cron_hold_pending_aadhar cron set in live

- Order status changed to on_hold, expired cron issue  - 12:30 - 1:00, 3:30 - 4:50
    - issue is because of revert_deadline
    - issue solved

- Testing with durgesh - Order status changed to on_hold, expired cron issue - 4:50 - 5:30
    - helped to manaully data updation in db 

- upload changes in live manually  - 5:30 - 5:45
    - Order status changed to on_hold, expired cron issue changes

- Client meeting - Progress meeting with Empower team - 1:00 - 2:00

- Discussion with durgesh, regarding order crons for change status to on_hold, expire issue  - 20 min

- Discussion with Ravi bhai & Athik, ragarding Team Master (State team) creation and Quiz Result changes - 25 min

- Manully order revert which hold by cron code issue  - 5:45 - 6:00

# ___________________________________________________________________________________________________________

# 27-02-2026

## Miscellaneous
- Townhall - 4:30 - 7:15

## Empower HH
- User Role, Division, Hierarchy related Testing with siddh - 10:15 - 11:35, 11:40 - 12:40
    - sync data to mavens api test
    - effective date based cron test

- user hierarchy change on effective cron changes - 12:40 - 12:50, 1:25 - 3:55

- ronak - 12:50 - 1:05

- changes upload in Live server - 3:55 - 4:30

- issue check, requested by komal ma'am - 7:15 - 8:20
    - synced data from mavens mismatched issue 
    - checked mail and reverted back

######

- Active user data based on effective date cron
- User hiearcy on effectivr date change 

- submit quiz changes (discuss with harsh) - column mismatch issue (taken time) - FULL PRIORITY


- otp not sending to all device, if user login in multi device

- account manager code on dailuy base cron 


- Manually Deleted Duplicate Order Tagging (Live)


- sync from Mavens data Testing


- Order List changes

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

--

- Store logs (Web & APIs)

---

- Replace user to resigned user (waiting for siddh updation) - Pending

######
