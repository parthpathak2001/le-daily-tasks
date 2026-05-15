# 03-11-2025

## Empower HH

- Order Approval List API changes - 10:20 - 12:25
    If user is ZBM, Display order, which users's division-wise and user's hierarchy's user is tagged in their product 
    changes discuss with Harsh

- Mavens S3 Bucket - user hierarchy sheet checked, data is proper or not, it have no data of their parent user - 12:25 - 12:55

- Order Details API changes - Display order invoice, which users's division-wise and user's hierarchy's user is tagged in their order product - 1:15 - 2:35

- Order Approval List API issue faced in live when Used is ZBM and Is authority both  - 4:10 - 5:21 
    checked issue, need many changes so currently revked new changes

- send api details to Harsh - 12:55 - 1:15, 2:35 - 03:40
- Uploaded latest changes in UAT and Live - 40 mins

- Order Details API changes - added max_invoice_percentage value in the response - 3:40 - 4:10

# ___________________________________________________________________________________________________________

# 05-11-2025

## Empower HH

- OTP send using Whatsapp API   - 10:45 - 11:10, 11:25 - 11:50
    Checked developer portal 
    tested new created template 

- Sync Doctor - User mapping changes - 11:10 - 11:25, 11:50 - 12:30, 1:55 - 2:11
    create new mapping only instead of delete doctor's existing mapping
    delete only expired user-doctor mapping, expired or not checked using startdate and enddate 
    uploaded in Live and Tested 

- Merge UAT and Local code - 12:30 - 1:00

- Help ravi bhai to test push notification changes - 1:00 - 1:30

- meeting with Harsh, Ravi, Snehalbhai, Siddh - regarding users hierarchy changes - 1:30 - 1:50 

- Send OTP using Whatsapp - 2:50 - 3:15, 3:55 - 4:18, 4:25 - 4:57, 5:19 - 5:53
    create_order Api change 
    resend_order_otp Api change
    upload_invoice Api change
    resend_order_invoice_otp Api change
    Uploaded in UAT
    message not sending after some messages - issue checked

- meeting with harsh, ravi, durgesh, siddh, snehalbhai - regarding new changes - 3:15 - 3:55

- Stockist Management changes - added Is Allowed checkbox , added Stockist - Manager mapping - 5:53 - 7:42

- User-Doctor Mapping page changes - display only allowed Stockist - 7:42 - 7:50


## Miscellaneous
- Add Worklog, Previous days worklog (31-10 ,3-11, 5-11) - 7:50 - 8:40

# ___________________________________________________________________________________________________________

# 06-11-2025

## Empower HH
- 10:17 - 10:40

- Stockist Management changes  - 10:40 - 11:25
    display is allowed and mapping status
    added action button and popup for stockist 'is allow'-> yes/no and stockist manager mapping  

- If user is authority user, Get Order List by Mapped Stockist with user - 11:32 - 1:43, 6:15 - 7:00
    Order Approval List API changes - done

    created new get_mapped_managers_by_order function (effects in verify_order api, verify_invoice api, sendOrderDetailsToStockist api - for send mail) - done
    has_pending_order_approval (effects in notification_count api, cron_notify_pending_approvals cron) - done

- Order Details changes (web) - 2:32 - 4:00, 5:00 - 5:24 
    - Display multi invoice data
    - display invoice wise tagging data
    - make design proper

- Uploaded Latest code in UAT and Tested -  5:39 - 6:15

- meeting with roshan, komal, harsh, ravi, siddh (4 PM) - 4:00 - 5:00
    regarding maven panel understanding
    maven panel - user hierarchy understanding   

    displayed our hierarchy changing functionality

- Order Details changes (web) - 7:00 - 7:30
    display invoice status, invoice type
    display only invoice date, remove time
    uploaded in UAT and Tested


# ___________________________________________________________________________________________________________

# 07-11-2025

## Empower HH

- Stockist Management changes - 10:15 - 11:00
    added validation in stockist - manager mapping popup 

- issue check raised by Durgesh - 11:05 - 11:35
    notification not sending issue checked, its working properly

- Mavens S3 Bucket sheet - custaccmap.csv sync changes - 11:00 - 11:05, 11:35 - 1:40, 1:54 - 2:15
    save all data of user_doctor mapping sheet in user_doctor_mapping_mavens with status (total records - 5,68,790)

- Order List API changes - 2:15 - 2:36, 3:00 - 4:20
    display order where logged-in user is tagged 

- 4:20 - 4:45
- Mavens S3 Bucket sheet - customermaster.csv, dealerdetail.csv, employee.csv sync changes - 4:45 - 6:00
    checked we stored all data from customermaster.csv or not, we already stored all data 
    checked we stored all data from dealerdetail.csv or not, we already stored all data 
    checked we stored all data from employee.csv or not, we already stored all data 
    checked mavens included mobile number for doctor and chemist or not

- Mavens S3 Bucket sheet - emprole.csv sync script changes - 6:00 - 7:00
    save all data of emprole.csv sheet in emp_role_mavens with status

# ___________________________________________________________________________________________________________

# 10-11-2025

## Empower HH

- 11:13 - 11:38

- Weekly Project Update and planning Meeting with Snehalbhai, Ravi, Harsh, Durgesh, Siddh - regarding project completed tasks and pending task - 11:38 - 12:15

- Run Users Hierarchy Sync script in UAT  - 12:15 - 2:31
    check hierarchy manually

- Mavens S3 Bucket sheet - empdivision.csv sync script changes - 3:21 - 4:31
    save all data of empdivision.csv sheet in emp_division_mavens with status
    Uploaded in UAT and Synced in UAT
    
- Mavens S3 Bucket sheet - accmgrrelation.csv sync script changes - 4:31 - 4:55
    save all data of accmgrrelation.csv sheet in acc_mgr_relation_mavens with status
    Uploaded in UAT and Synced in UAT

- Mavens S3 Bucket sheet - empaccmgrmap.csv sync script changes - 4:55 - 8:00
    save all data of empaccmgrmap.csv sheet in emp_acc_mgr_map_mavens with status
    Uploaded in UAT and Synced in UAT

# ___________________________________________________________________________________________________________

# 11-11-2025

## Empower HH

- user division sync issue - if user have multiple state it not store division issue resolved  - 10:29 - 11:05

- Users Hierarchy synced data checked - 11:05 - 11:35, 12:00 - 12:35, 1:05 - 1:16, 2:00 - 3:00, 3:32 - 3:37, 3:56 - 5:25, 5:40 - 6:06, 6:39 -  8:25
    - why Admin id is 0, reason: accountmanager code is missing so it break hierchy 
    - changes in hierarchy syncing code, when parent user not found then fetch their parent 
    - Uploaded in UAT
    - Synced Hierarchy 

- Product list not displaying in Order details API issue raised by Ronak - checked - 11:35 - 12:00
    - issue is from app side, they not given product in invoice upload body so products not displaying 

- Meeting with PHP team - Ram bhai, Ravi bhai, Siddh, Athikur - 12:35 - 1:05
    regarding All running project management 

- Chemist Sync, Doctor Sync changes in live - 1:16 - 2:00
    chemist Phone number sync
    run script in live to sync latest master data (FirsttimeBackup/Master/NewmasterData/IDUpdatedNew/)

- Meeting with client - 3:00 - 3:32
    regarding PMS understanding

- doctor & chemist sync script changes in Live changed to old code to sync daily incremental data - 5:25 - 5:40

# ___________________________________________________________________________________________________________

# 12-11-2025

## Empower HH

- 10:36 - 10:45

- User Hierachy Synced data checked - 10:45 - 11:20, 11:45 - 2:13
    - why role, division, hierarchy blank - checked manualy
    - empdivision.csv - if effectiveto date is past date so not stored that division
    - empdivision.csv - returns mismatched divisionid, which division code not exist in our db
    - emprole.csv - if effectiveto date is past date so not stored that role
    - emprole.csv - returns role is not exist in our db like (DSO, FSO)
    - emprole.csv, accmgrrelation.csv (hierarchy) - returns mismatched employee code it returns like (MOKSHAGNA, PHKARNATAKAPULSE)
    - user hierarchy not stored proper, because user's role is not exist in our system and their parent user's role is not exist in our system
    

- Issue Raised by Durgesh - when order create it returns - "doctor discouunt not appoved. cant create order" validation but doctor have approved discount - 11:20 - 11:45
    i checked issue, issue is from app, app not passed doctor id proper, they not change doctor id on doctor dropdown change so it returns old doctor id which have no discount so it return issue

- Mavens S3 Bucket sheet - customermaster.csv sync script changes - 3:00 - 3:35, 4:35 - 5:10 
    save all data of customermaster.csv sheet in customer_master_mavens with status
    Uploaded in UAT

- Order details API issue when is_zbm = 1  - 3:35 - 4:35
    it display all invoice, instead of this displayed tagged order invoices only when is_zbm = 1
    uploaded in UAT

- Order Details page (WEB) changes - 5:10 - 5:30
    remove old code of displaying tagging and invoice 

- Mavens S3 Bucket sheet - dealerdetail.csv sync script changes - 5:30 - 6:15 
    save all data of dealerdetail.csv sheet in dealer_detail_mavens with status
    Uploaded in UAT

- Mavens S3 Bucket sheet - employee.csv sync script changes - 6:15 - 6:50
    save all data of employee.csv sheet in employee_mavens with status
    Uploaded in UAT

- All mavens sheet sync code changes - Store mavens status from sheet, checked all mavens sync script - 6:50 - 7:20
    sync_doctors
    sync_chemists
    sync_employee

- Checked Employee, Employee Role, Employee Division sync script - 7:20 - 7:37

## Miscellaneous
- Add worklog - 7:37 - 7:59

# ___________________________________________________________________________________________________________

# 13-11-2025

## Empower HH

- 10:35 - 10:50

- Checked Employee, Employee Role, Employee Division sync script - 10:50 - 11:30
    Run scripts on Local and UAT to test

- Meeting with Client - 11:30 - 1:20
    DISCUSSION ON HIERACHY AUTOMATION -MAVENS & ENKINDLE TEAM
    regarding Two way sync data
    demo of hierachy management from our side

- Sync User Hierarchy changes - 1:20 - 2:02
    - Checked parent recursively when parent not found
    - Handled multi-level parent lookup fallback

- Order Approval List API issue solved - 3:09 - 4:19, 4:38 - 4:50, 5:45 - 8:00
    API does not support multiple roles together (e.g., user is both ZBM + Authority).
    Implement proper multi-role handling

- issue: komal said chemist data is mismatched, take all incremental data (date: 16-10-2025 to 13-11-2025) using script and send to komal, with darshil - 4:50 - 5:45

## Miscellaneous
- Add Worklog - 8:00 - 8:30


# ___________________________________________________________________________________________________________

# 14-11-2025

## Empower HH

- 10:50 - 11:00

- Run user hierarchy script to check latest script changes - 11:00 - 11:38, 11:48 - 12:45

- Order Approval list issue - when user is not authority or zbm or division head, it returns error - 12:45 - 1:00, 1:15 - 1:22
    its because of model function mismatched

- chemist data uploaded in uat mannuly (durgesh) - 1:00 - 1:15

- Mavens sync script changes - 1:40 - 2:30
    Updated Mavens ID handling — removed "ID" prefix and stored only numeric value 
    Modified logging logic — always insert into Mavens log table (no update on existing records) 

    Updated in the following scripts:
        save_doctor
        save_chemist
        save_user_doctor_mapping
        save_employee
        save_employee_account_manager_code
        save_employee_role
        save_employee_division
        save_employee_acc_mgr_relation

- 3:07 - 3:40
- Upload latest code in Live and Tested - 3:40 - 4:21, 4:35 - 4:50
    Doctor sync, Chemist sync, Doctor User mapping sync changes uploaded 

- Order Details changes (web) - Export to Excel changes - 4:50 - 7:10
    - Display multi invoice data in exported excel
    - display invoice wise tagging data in exported excel
    - displayed in proper format
    - uploaded in UAT

- New Task Discussion with Harsh, Ravi - 7:10 - 7:30
    Order List Filter, Export, other changes (web)
    Order Details page changes (web)
    Doctor List page changes (web)
    Discount Log List changes (web)

## Miscellaneous
- Add worklog - 2:30 - 2:44, 7:30 - 7:45


# ___________________________________________________________________________________________________________

# 17-11-2025

## Empower HH
- 10:32  - 11:00

- Added effective-date based cron updates for user account manager code, user role and user division - 11:00 - 11:19, 11:26 - 2:09, 2:35 - 3:05, 3:30 - 4:11, 4:24 - 4:40
    - Discussed with Ravi bhai and Siddh
    - managed is_synced_to_main flag to check data is stored in main table or not checked is_synced_to_main through
    - updated changes:
        save_employee_division
        save_employee_role
        
    - Created new crons:
        activate_today_account_manager_codes
        activate_today_roles
        activate_today_divisions

- Added effective-date based cron updates for user doctor mapping - 4:40 - 5:15
    - managed is_synced_to_main flag to check data is stored in main table or not checked is_synced_to_main through
    - created new crons:
        activate_today_user_doctor_mapping

- user hierarchy changes - 5:15 - 6:37, 7:25 - 7:30
    understanding and Analysis on manage hierarchy log (hierarchy_history_role_user table) 
    discuss regarding how to manage hierarchy log on effective date - with Siddh

- whatsapp message sending checked  - 6:37 - 7:25
    checked message sending proper or not
    i send whatsapp otp message to different users but it not send whatsapp message but from that user i send message to bussiness account and then again i sent otp meesage and then it sended to that user  

## Miscellaneous
- Add Worklog - 7:30 - 7:55



# ___________________________________________________________________________________________________________

# 18-11-2025

## Empower HH
- 10:33 - 11:00

- Added effective-date based cron updates for user hierarchy mapping changes - 11:00 - 11:14, 11:26 -  12:25
    reserch on table structure
    i stuck at how to manage inactive hierarchy data in log for history, so understamding that  

- Explain Order reports task to darshil  - 30 mins + 15 mins + 20 mins
    explain: create new Custom Export, create new Normal Export 
    checked task and given changes, bugs 
    explain new changes in that reports

- Order Custom Export report - 12:25 - 12:55
    understanding this and just started work on this then after i have new work so i given this task to Darsil

- Check data (komal) - 12:55 - 1:36
    User - doctor mapping not proper checked and replied to ramkuamar

- Check data (komal) - 1:54 - 2:41, 3:04 - 3:10
    Order status why expired
    order expired because order not approved within 2 days after verfied using otp

- discuss with ravi bhai and siddh regarding how to manage user is resigned - 20 min

- Check data (komal) - 3:10 - 4:07,  4:28 - 5:06, 6:02 - 6:30, 6:43 - 7:06
    why employee division and role not stored
    - maven sheet not have that user data, checked sheet manully to find their data
    - i checked other sheets, this user division and role data is inactive so we not updated that user's division and role
    - manully update users division where division is null from latest inactive division data
    - manully update users role where role is null from latest inactive role data
- -15 mins

- Sync changes - 5:06 - 6:02, 6:43 - 7:10
    created script to update division if current not exist then update last division and role

- meeting with client - 04:07 - 4:23
    disscussion regarding they need user import with additional information first and then user hierarchy import 
    we asked question regarding user resign confusion

- help to client (Ganesh) - 6:30 - 6:43
    invoice not displaying issue 
    order is on hold, because they not uploaded invoice within 10 days

## Miscellaneous
- Added worklog - 7:30 - 8:20


# ___________________________________________________________________________________________________________

# 19-11-2025

## Empower HH
- 10:29 - 10:55
- help darshil - 10 mins, 2:31 - 2:41, 3:02 - 3:35
    order export changes: 
        if order invoices uploaded need to display data from order_invoice_product 
        if order invoie not uploaded then display from order_product

- discussion with siddh regarding when create user need to manage log related - 10 mins

- 12:10 - 12:20 

- Add stockist data manully (requested by Komal) - 12:20 - 12:38

- User hierarchy cron changes - 12:38 - 1:30, 1:48 - 2:31
    create hierarchy from acc_mgr_relation_mavens table instead of acc_mgr_relation_incremental_csv_temp
    reverted this changes, because changed logic to do this

- Added effective-date based cron updates for user hierarchy mapping changes - 3:35 - 5:10, 5:20 - 6:45
    discuss with ravibhai and siddh
    check acc_mgr_relation.csv file from s3 bucket

- doctor mapping page changes - display all stockist, removed state condition (requested by Komal) - 5:10 - 5:20


- Change role by effective date (cron update) - 6:45 - 8:00
    If the employee is resigned, updated status to Resigned
    When role changes, removed the user’s ID from all other users’ hierarchy records  

## Miscellaneous
- Electricity issue - 11:15 - 12:10
- Added worklog - 8:00 - 8:30

# ___________________________________________________________________________________________________________

# 20-11-2025

## Empower HH

- 10:38 - 11:00

- Create a now cron script to update user hierarchy in effective date - 11:00 - 11:21, 11:28 - 12:35, 1:45 - 2:00, 2:55 - 4:05
    created script for incremental data
    created self hierarchy from parent user's hierarchy
-  -10 min, -20 mins

- Change role by effective date (cron update) - 10 mins
    Store last working date when user is resigned 

- explain to darshil - 12:35 - 1:25, +10 mins, +20 mins, +15 mins, 7:20 - 8:05
    previously developed changes checked and uploaded in GIT
    explain to create export order as old code logic (without multiinvoice)
    find old code from live and sent to darshil for create report
    solve some issue occurs in live
    uploaded darshil code in live and GIT

- incremental emprole.csv sheet checked - 1:25 - 1:45

- Role Master data sync cron change - 04:05 - 4:20, 4:30 - 4:50
    When role changes, removed the user’s ID from all other users’ hierarchy records

- incremental emprole.csv sheet sync script run in local - 4:50 - 7:20, 8:05 - 8:10
    created cron script to set previous role if user have no roles as current data

    Synced below masters:
        FirsttimeBackup/Master/NewmasterData/IDUpdatedNew/Mon Nov 10 17:04:28 IST 2025/empdivision.csv
        FirsttimeBackup/Master/NewmasterData/IDUpdatedNew/Mon Nov 10 17:04:28 IST 2025/empaccmgrmap.csv
        FirsttimeBackup/Master/NewmasterData/IDUpdatedNew/Mon Nov 10 17:04:05 IST 2025/accmgrrelation.csv
        FirsttimeBackup/Master/NewmasterData/IDUpdatedNew/Wed Nov 19 18:42:09 IST 2025/emprole.csv
- -15 mins

## Miscellaneous
- Added worklog - 8:10 - 8:35

# ___________________________________________________________________________________________________________

# 21-11-2025

## Empower HH

- 10:11 - 10:25

- employee division, role and hierarchy sync effective date crons uploaded and tested in UAT - 10:25 - 11:19, 11:25 - 12:00
    discussion related how to manage division in effective date based sync (4D/9D division setup wise) 
    minor changes in sync codes
    uploaded in UAT
    review and checked code
    Testing in UAT


- Sync mavens master data in Live - 12:00 - 2:15
    uploaded minor sync script changes in live
    checked data manully from Sheet and Database

- Testing Hiearchy updation in UAT with Siddh - 3:04 - 4:50
    Role change
    Division change
    Hierarchy change

- Meeting regarding Annual event- 4:50 - 5:05

- - Add doctor data manully (requested by Komal) - 5:05 - 5:20


# ___________________________________________________________________________________________________________

# 24-11-2025

## Empower HH
- 11:19 - 11:28 , 11:31 - 12:00

- Order List changes (Web)- 12:00 - 2:10, 3:05 - 3:35, 4:00 - 4:18, 4:23 - 5:40
    Order List page changes - count total of PTR, Discount, Total Amount - (12:55 - 1:30)
    Order List Export changes - Added count total of PTR, Discount, Total Amount - (1:30 - 1:35)
    Order Details page changes -> displayed invoice details with product tagging instead of invoice group (1:35 - 2:10, 3:05 - 3:35)
    Order details Export changes -> displayed division name with product data and displayed invoice details with product tagging instead of invoice group - (4:00 - 4:18, 4:23 - 5:40)
    uploaded in UAT and Tested

- Darshil code reviewed and uploaded in UAT and Tested - 3:35 - 4:00
    order details page changes -> displayed division name with product data in Order tagging details 

- Doctor List page changes -> displayed "Last Mapped Date". - 5:40 - 6:20
    uploaded in UAT and Tested

- Employee City and State Sync changes - 6:20 - 7:05, 7:20 - 8:00
    Sync user account manager relation based on effective date cron changes
    Master account manager relation sync changes

- Explain latest changes uploaded in UAT and added dummy doctor data and mapped with his user - 7:05 - 7:20

## Miscellaneous
- Added worklog - 8:00 - 


# ___________________________________________________________________________________________________________

# 25-11-2025

## Empower HH
- Tested hierarchy change module with siddh - 10:28 - 11:22, 1:00 - 1:30 , 4:20 - 5:10
    discussion related manager user hierarchy functionality
    find an issue where change manager then not change that manager's child user's managers
    when change any user's super parent then it not effects on that user hiearchy view
    testing after siddh changed the code to solve above issue, it have another issue it set 0 to another columns (ZBM,RBM,etc.)
    helped siddh to solve issue

- Change user hiearchy cron script changes - 11:30 - 1:00, 4:10 - 4:20
    - Fixed issue where manager changes were not reflecting in their downline hierarchy.
    - Updated script so that when a user’s manager changes, the new hierarchy chain is automatically applied to all child users under that manager. Ensures correct and consistent hierarchy updates for all levels.
    - uploaded in UAT and Tested.

- 1:30 - 2:00
- 2:18 - 2:30

- checking User hierarchy data with shared sheet data - 3:20 - 3:45, 5:30 - 6:20
    user hiearchy script run again

- mail checked -> User doctor mapping data mismatched issue mail - 3:45 - 4:10
    checked data manully and verify with our system and mavens sheet
    created mail and send reply to Mavens team and client 

- issue checked - Order approval not wroking issue raised by Komal checked - 5:10 - 5:30, 6:30 - 6:40
    issue not found

- user hierarchy change module, Testing with siddh - 6:40 - 8:00

## Miscellaneous
- Added worklog - 2:30 - 2:45, 3:15 - 3:20, 8:00 - 


# ___________________________________________________________________________________________________________

# 26-11-2025

## Empower HH

- 10:32 - 11:00

- Change Role Based on Effective Date Sync Script Changes  - 11:00 - 11:22, 11:55 - 12:10
    - Managed resignation logic: processed users with end date = today and marked them as Resigned.
    - Removed resigned users from all hierarchy role mappings.
    - Updated user_master (status & last working date) and emp_role_mavens (resigned status, sync flags).
    - Separated resignation flow from role activation to prevent conflicts and ensure correct updates.

- Checked the mail regarding the 10th November master backup, verified the Mavens data, and replied requesting the latest full master data again because syncing the old master would affect the incremental updates after the master data upload. - 11:30 - 11:55

- understanding with siddh - how to manage vacanct user flow to create new cron script - 11:55 - 12:25 

- Quiz issue checked (raised by Shaziya) - 12:25 – 1:35
    Checked the quiz issue raised by Shaziya. Found that the system was displaying 40 marks because the user attempted the quiz twice, resulting in 40 answer records even though the quiz contains only 25 questions. Identified 16 duplicate questionIds and confirmed 24 unique valid questions.

- Quiz completion issue  - 1:35 - 2:03, 2:44 - 3:05

- Testing with siddh - 3:05 - 3:45

- user data sync from mavens script run again to give UAT to client - 3:45 - 4:05

- Meeting regarding demo to client - 4:05 - 6:00

- discussion with Roshan, ravi, harsh, siddh regarding how to manage resigned user, how to manage SBM - 6:00 - 6:30


- user hierarchy checked mannuly - 6:30 - 7:30
    discussion with ravi, harsh, siddh regarding how to manage resigned user, how to manage SBM
    checking mavens sheets to verify data


# ___________________________________________________________________________________________________________

# 27-11-2025

## Empower HH

- 10:27 - 11:10

- Shaziya issue checking - 11:10 - 11:23, 11:28 - 12:15
    issue: Quiz issue checked (raised by Shaziya) - questinalry have 25 question attempte 40 and display mark 40
    issue: Quiz completion issue  - quiz not fully attempted also displayuing Completed and certificate download not available
    issue not found
    

- discuss with Siddh, Ravi regarding how to manage mavens records start_date and end_date - 12:15 - 12:35

- Dashboard taking load issue checked in live - 12:35 - 1:50
    no changes

- Create scipt to sync SBM for BE from given Hierarchy-2025.csv file - 1:50 - 1:56, 2:50 -  4:05
    uploaded in Uat and Tested 

- User list page -> created new export User hierarchy report - 4:05 - 4:13, 4:24 - 7:30

- Set Cron in UAT - 7:30 - 7:45

## Miscellaneous
- Add worklog - 7:45 - 

---
- Mavens Sync changes, store mavens_start_date_original and mavens_end_date_original -
- make mavens table empty and Run Mavens Script again because duplicate data stored   - 
---


# ___________________________________________________________________________________________________________

##### PENDING
- Admin Panel - Order status change from "On Hold & Expired", send otp also - PENDING

- Revert Order Status (Admin panel), email not working - PENDING

- Dashboard load lye che e check krvu (su load lye e check krvu)

---

- On_hold and Expired exact time e thava joi - (e research krvanu che) - PENDING

---

- mapping, role change, division change, etc. Sync ma Efective date nu rakhvu. effective avya pachi aapdi system ma effect kravu


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

- city, state sync krvanu - account_manager_relation -> hq code per thi

---

- Orde details -> invioce wise product display changes 

- Vacant user ni functinality krvi

- quiz issue - raised by Shaziya

---

- order custom export ma QTY mukvu PTR RATE, PTR Value Vache

---
- Mavens Sync changes, store mavens_start_date_original and mavens_end_date_original -
- make mavens table empty and Run Mavens Script again because duplicate data stored   - 


######
