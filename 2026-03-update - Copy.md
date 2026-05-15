# ___________________________________________________________________________________________________________

# 02-03-2026

## Miscellaneous

## Empower HH
- new script to store doctor log with file path and date - 10:30 - 12:10

- doctor data issue from mavens manully checking - 2:45 - 4:02 
    - doctor data missing issue
    - uni turn to blank (null)

- meeting with snehalbhai, ravibhai, harsh, prashant bhai, etc. - 12:10 - 12:40
    - for current work details

- State issue checking - 12:40 - 1:25, 1:45 - 2:00
    - state not exist 
    - added manually states and updates coded which not exist

- Created new script to Activate Deactive users on effective date - 2:00 - 2:45

- Discussion with Athikur and Ravibhai - 04:25 - 4:45

- find user sync incorrect data in mavens - for JAMEEL AHMED A and send mail to komal and jameel  - 4:45 - 5:20

- send order details mail to stockist change - 5:20 - 6:40
    - remove mail
    - quiz issue solve
    - sync log with file path and date code upload in live

- sync data to mavens script changes - 6:40 - 7:15
    - added condition to display only testing user data
    - send mail to mavens 

# ___________________________________________________________________________________________________________

# 03-03-2026

## Miscellaneous
- System issue - 1:45 - 2:20

## Empower HH
- Push Notification issue - 10:25 - 11:10
    - if same user is logged in multiple place it send push notification only on latest device

- Upload code in UAT, add crons - 11:10 - 12:30
    - it have conflicts so solving this
    
- doctor state issue - 12:30 - 1:10, 1:30 - 1:45, 2:35 - 3:35
    - doctor 
    - chemist
    - user state changed

- Discuss with Athik 
    - Regarding Quiz result change
    - help to git conflict solve 

- discuss with siddh and roshan - 10 
    - regarding user deactivation 

- Issue in Push notification sending code - 4:00 - 5:00
    - finding issue taking long time because of system issue (blue scren) and git corrupt issue

- git corrupt issue - 5:00 - 5:20


- discuss with athikur regarding push notification issue - 15 min

- role permission wise module access - 5:30 - 

# ___________________________________________________________________________________________________________

# 05-03-2026

## Miscellaneous

## Empower HH

- Progress meeting PPT updation

- discussion with athik reagrding pms queue functionality

- role permission wise module access - 10:20 - 1:00
    - Added module-wise permission checks for Admin, State Team, User, Announcement, City, Courier, Department, Device, Doctor, Education Content, Notification, Office Location, Order, Product, Question, Quiz, Region, Result, Role, State, Team and related modules with model and view-level validation.

- Meeting With Empower Team - Progress meeting - 1:00 - 1:35
 
- User Creation and Assign Role Permission - 2:20 - 5:10, 5:55 - 7:10

- Meeting with Komal ma'am, regarding Order Reassign Demo and Role Permission module demo - 5:10 - 5:55


# ___________________________________________________________________________________________________________

# 06-03-2026

## Miscellaneous
- Add worklog - 10:10 - 10:45

## Empower HH
- Role & Permission module - Bug solve - 10:45 - 1:20, 1:43 - 3:50, 4:40 - 5:00, 5:30 - 5:50
    - Admin User, Admin Role, Admin Permission module changes 
    - Admin Role - Permission Dropdown not working properly, fixed
    - Added proper validations 
    - Admin Role Module - Added Select All, Deselect All buttons for Select Permissions
    - Admin Role Issue - Some time display database issue in role permission, Unique constraint issue solved
    - Other reported bugs by Jaya solved
    - Uploaded in Uat
    - solved bugs which comes after new changes uploaded
        - Validation changes

- In full project check condition like login user id is == 1 then its admin and can perform task. instead of this added condition like is_super_admin == 1/0 condition - 3:50 - 4:30


- Login Module changes - 5:00 - 5:30
    -  Inactive Admin User can not login and display msg like "User is Inactive. Please contact Administrator"
    -  Inactive Admin Role User can not login and display msg like "User Role is Inactive. Please contact Administrator"

- Created new cron script to Deactivate User on effective date - 5:50 - 6:50

# ___________________________________________________________________________________________________________

# 09-03-2026

## Miscellaneous
- system setup (my system formated so setup system) - 11:00 - 3:15
    - installed software 
    - at that time i faced also system issue (blue screen error), discused with rahul bhai, they checked my system 

- Pucho CRM Static page design and verification - 7:15 - 8:00 

## Empower HH
- Dummy Doctor not dispaying issue, because of dummy doctor's uni value turns to blank by mistake so issue occurs (when updating all doctor's latest uni upadate using mysql at that time that is turns to blank)  - 3:15 - 3:45

- Order issue checked - log checked - 3:45 - 4:15
    - order edit not working checked log 

- Role Permission changes - 4:25 - 7:15
    - Added missing role permision manualy find all permissions from code and added in permissions
    - Permission setup for Chemist Phone number change action
    - Zone List action permissions 

# ___________________________________________________________________________________________________________

# 10-03-2026

## Miscellaneous
- System Setup - 10:20 - 12:10

## Empower HH
- Role permission changes - 12:10 - 12:15, 12:40 - 1:00
    - Admin User, Admin Role listing issue solve (db fiealds issue)

- Internal meeting with harsh and ravi bhai - 12:15 - 12:40

- Meeting with Client - Progress meeting - 1:30 - 2:30

- Store Country id from sync address cron (cmpostal.csv) - 1:30 - 2:30
    - uploaded in live
    - old existing data update manualy


- User Vacancy and Resinged generation - 03:45 - 7:47
    - discussion with siddh and ravi bhai
    - manully vacant user generate from given hierarchy 2026 sheet
    - manuaaly resigned user

# ___________________________________________________________________________________________________________


# 11-03-2026

## Miscellaneous
- 

## Empower HH
- Create user for demo of role permission
    - assign permissions

- Verify user Hierarchy

- Vacancy generation - 11:35 - 11:55, 12:45 - 1:10, 1:30 - 2:05, 2:15 - 2:25, 5:10 - 5:35, 6:30 - 8:30
    - manually vacancy generate

- Internal meeting - 11:55 - 12:30
    - Hierarchy Flow demo
    - discussion with siddh, regarfing issue  - 12:30 - 12:45

- Discuss with harsh  - 2:05 - 2:15
- User doctor mapping issue finding (harsh) - 2:25 - 2:40
    - it have no doctor mapped from mavens

- Order issue (tagging issue) (harsh) - 2:40 - 2:57, 3:20 - 5:10
    - issue: Order tagging approved by division head so should it status changes to completed but it not changed the status 
    - checked scenarios but issue not reproduce 

- Order: 856 - manualy changes invoice file and details - 5:35 - 6:10

- Mavens sync issue checking with ravi bhai - 6:10 - 6:30 

# ___________________________________________________________________________________________________________

# 12-03-2026

## Miscellaneous
- Discuss with Om, ragarding role-permission task doubts of Om
- help siddh to merge code 

## Empower HH

- Manully verify hierarchy data and vacancy generate - 11:00 - 12:55, 2:45 - 2:55, 3:25 - 4:45

- store log with path for synced data log in UAT - 11:55 - 1:00

- Progress Meeting - 1:00 - 2:25

- Sync Data to Mavens APIs changes - remove the "page" and "limit" fields from scripts (empower to mavens) - 4:45 - 7:00
    - Document updation 
    - Mail revert to Mavens Team

- Discussion with ravi bhai reagarding user hiearchy mismatch issue solve

# ___________________________________________________________________________________________________________

# 13-03-2026

## Miscellaneous

## Empower HH
- Discuss with Om and Dhruvik - 10:10 - 10:45 
    - assign task to dhruvik
    - check task of om

- Mavens Script changes - 12:30 - 1:10, 1:30 - 2:00, 2:25 - 3:40
    - If User is not BE/SBE remove SBM from hierarchy
    - If Role changed, remove old parent hierarchy
    - Uploaded in Live

- Costing of Empower - 4:00 - 4:15
    - Verify added data by ravibhai (tasks - any missing or not)

- Git issue solve - 4:15 - 6:10
    - for upload in live create new branch and upload latest change
    - create new brach and manage code which no need to upload
    - for upload siddh hiearchy related latest data

- User Master changes - 6:10 - 7:15
    - Display division state - division setup wise
    - Zone field make optional


# ___________________________________________________________________________________________________________

# 16-03-2026

## Miscellaneous
- RMIS costing point verification - 12:25 - 12:40

## Empower HH
- user can not order of doctor which order is on_hold - 10:45 - 11:15, 11:20 - 12:25
    - Uploaded in UAT Tested
    - it takes extra time because of git conflicts

- User Add/Edit changes - 12:40 - 1:15, 1:35 - 1:45, 2:30 - 9:05
    - Moved Permanent Address to first tab
    - Moved Replacement Information to first tab
    - Replacement Information to first tab - added Resigned/Vacant Users dropdown and get users details dynamicaly
    - make this field read only spe code, spe name, division head, division setup, budget
    - After Added Statewise division feature, In edit form its hiearchy not displaying on load, issue solved
    - Git Issue on uploading in UAT (conflict issue), to solve this created new branch and merged siddh's branch, parth's branch and live_uat branch and checkout that on uat branch
    - Durgesh faced multiple time issue, old working code not working now, because of git issue, it have developer wise diff branch and merging it have lots of conflicts and confusion so it take much time 
    - multiple time branch change, created new branches and merging codes
    - Replacement of Resigned Users functionality

# ___________________________________________________________________________________________________________

# 17-03-2026

## Miscellaneous


## Empower HH
- User Add/Edit changes - 10:30 - 1:40, 2:40 - 2:46, 3:05 - 3:55 , 4:00 - 8:30
    - Replacement of resigned/vacant users functionality

- Progress Review meeting - 1:40 - 2:10

- Merge changes with ravi bhai, to solving git issue - 3:10 - 4:00


# ___________________________________________________________________________________________________________

# 18-03-2026

## Miscellaneous


## Empower HH
- User Add/Edit changes - 10:20 - 12:30, 12:55 - 4:50, 5:20 - 5:50, 6:40 - 8:00
    - Replacement of resigned/vacant users functionality - Store data in mavens tables
    - Testing
    - stored History in hierarchy_history_role_user and hierarchy_change_audit 

- KRA KPI - 12:30 - 12:55

- Hierarchy Demo Meeting - 4:50 - 5:20

- meeting with harsh and ravi -  5:50 - 6:40

# ___________________________________________________________________________________________________________

# 19-03-2026

## Miscellaneous

## Empower HH
- Display users division code wise (_9d and _4d both) - 10:45 - 11:15

- User Add/Edit Form — UI Layout Fixes - 11:15 - 12:50
    - Reorganized form fields across all 7 tabs to fill empty right-side column gaps by pairing solo fields into two-column rows
    - Fixed long label wrapping issue with CSS adjustments
    - Restructured Status, Is Authority, Is Division Head, Office Location and Upload Photo rows into correct order and alignment
    - No functionality, JS, PHP, or validation logic was changed

- Add/Edit User form - 12:50 - 1:20, 1:50 - 2:20, 2:50 - 6:35
    - Create Vacancy 
    - On replacement, User's State,City,Country,Location also replace
    - on user add/edit page - displyed all replaced details when replacement user select

- Displayed manager dropdown users from _4d/_9d both using division code - 6:35 - 8:10
    - when i done this it have issue parent of selcted manager is from both division (_4d/_9d) is not working 

# ___________________________________________________________________________________________________________

# 20-03-2026

## Miscellaneous

## Empower HH
- Add/Edit User – Changes & Bug Fixes - 10:35 - 1:00
    - Cross-Division Manager Fix – Used division_code to include sibling divisions (_4D/_9D) in manager lookups.
    - Admin Fallback in Hierarchy – Ensured admin field never saved as 0 when building hierarchy records.
    - NSM → Admin Manager Fix – Skipped division filter when selected manager is Admin role.
    - Vacancy Pre-Check Fix – Moved active vacancy check before any DB writes to prevent partial saves.
    - Role & Manager Validation (Server-Side) – Added required validation for role and role_manager fields in addUser().
    - Role & Manager Validation (Client-Side Edit Mode) – Added validateAssignRole() call inside validateForm() so edit mode also validates Role and Role Manager on save.

- Discussion with jaya, regarding sync data to mavens API testing - 1:40 - 2:00


- Add/Edit User – Changes & Bug Fixes - 2:20 - 3:00
    - Effective Date Validation Fix – Client-side validation was not blocking form submit when Division, Role, Headquarter, or Manager changed in edit mode.

- Discussion with jaya - 3:00 - 3:20
    Regarding User Master Testing and Changes


- User vacancy generation and vacancy replacement change - 3:20 - 4:00, 4:30 - 4:40


- User Master Testing - 4:40 - 5:00, 6:30 - 6:40

- User Hierarchy Demo meeting with internal team - 4:00 - 4:25, 5:00 - 6:30


- Git Branch manage - 6:40 - 7:10
    - manage role & permission branch


# ___________________________________________________________________________________________________________

# 23-03-2026

## Miscellaneous

## Empower HH
- Add/Edit user
    - Testing
    - log not store proper, stored that
    - vacancy not generated proper, issue solve
    - vacant user details not fetched proper from vacamcy table, it fetch from main table (user master and user hierarchy) so its wrong, made it proper 
    - Headquarter based on State

# ___________________________________________________________________________________________________________

# 24-03-2026

## Miscellaneous

## Empower HH
- Add/Edit User - 10:15 - 12:25
    - UI Improvement - Country → State → Headquarter → City → Location → Pincode - changed placement 
    - Emp code unique validation
    - pincode can add only digit validation
    - Exception: explode(): Argument #2 ($string) must be of type string, array given - issue solved

- git issue in UAT - 12:25 -  12:45
    - Re-initialize git

- Add/Edit User - 12:45 - 1:40
    - lastworkingdate issue, it store current date if user added for Future date 
    - join date and effective date same validation on Add user 
    - lastworkingdate not displaying in user edit - issue solved

- Progress Review Meeting with Empower Team - 1:00 - 1:25

- User Add/Edit  - 3:00 - 8:00
    - User Master testing and Mavens data checking 
    - sync_account_managers_to_mavens API changes - It fetched old data of purticular account_manager_code - issue fixed
    - when updated only manager - also create records in emp_division_mavens and emp_role_mavens - it issue, solved this 
    - In mavens history tables (_mavens table) - when user update we change old record's end date, its an issue - issue solved now we create new record same as old record with end date

# ___________________________________________________________________________________________________________

# 25-03-2026

## Miscellaneous
- Kotak bank account opening - 4:20 - 4:45
- worklog add - 8:25 - 

## Empower HH
- User Add/Edit - 10:15 - 12:10, 12:20 - 1:05, 1:25 - 01:50, 3:40 - 4:08, 4:45 - 08:25
    - Add/edit User Testing, mavens data proepr added or not testing
    - SBM included when replaced vacant user
    - account manager changed when only user manager changed
    - added unique account manager code validation
    - on replacement mavens data not proper stored - issue solved
    - In emp_acc_mgr_map_mavens it update old active record date to end date, intead this created new record with end date 

- manually data change - 12:10 - 12:20
    - Changed division for employee (emp code: 325)

- meeting with nilesh sir (empower) - 1:50 - 1:55

- Courier Testing - 1:55 - 3:10
    - Attachment Details - Courier Action

# ___________________________________________________________________________________________________________

# 26-03-2026

## Miscellaneous

## Empower HH
- User Add/Edit - 10:10 - 11:35
    - User Add/ Edit Testing and Checked Data stored for mavens is proper or not
    - On changes State, resets all dropdown related to State

- Effective date based cron changes - 11:35 - 12:25
    - CRON Testing

- Upload latest code in Live and testing - 12:25 - 1:00

- Progress Meeting with Empower team - 1:00 - 2:10

- Discount Approval changes - 1:35 - 2:10, 3:20 - 3:30, 4:30 - 5:50
    - Doctor mapped stockist and stockiest mapped to manager, that mapped manager only can approve doctor discount - this functionality added 
    - Discount List, Notification send on discount addition 

- upload role permission code to live - 3:30 - 4:30
    - create all roles, permissions 

- Data manully verify for user can not attempt quiz - 5:50 - 8:05
- Order Approval List API and Notification count API changes 
    - if zbm not approved not approved order invoice but division head already approved that also that order display that order is pending approval in ZBM login - issue solved  , if ZBM tagging not approved but division head approved, so that order invoice is not pending tagging - 

# ___________________________________________________________________________________________________________

# 27-03-2026

## Miscellaneous
- Weekly meeting - 2:30 - 3:40
- Add worklog - 7:55 -

## Empower HH
- In live Sync data to mavens apis testing - 11:00 - 12:00, 12:30 - 1:05, - 7:35
    - Client given data to test 
    - faces issue in Live: 
        - for effective date its not working
        - Script for mavens have issue - issue for replaced user
        - from tree view also its not woring for replacement - it not store parent mapping in mavens table

- Discuss with Om 
    - Role Permission changes

- Manually stockist data add, Requested by Komal ma'am - 7:35 - 7:55
- Manually Doctor state change, because chemist not displaying in that doctor for mapping, Requested by Komal ma'am - 7:55 - 8:05

- tree view issue in live - 12:00 - 12:30
    - php version issue - solved

# ___________________________________________________________________________________________________________

# 30-03-2026

## Miscellaneous
- In my system, System testing running - 10:30 - 10:50

## Empower HH
- user master test - 10:50 - 11:05, 11:25 - 5:40
    - Resign test
    - Effective date changes - It update user mater and users_hierarchy - issue solved - do not update if its effective date is future - 11:25 - 12:00 
    - Effective date changes - Generate vacancy but no active vacancy - Checked - 12:00 - 12:10
    - Effective date changes - Replace vacancy on future effective date based - checked - 12:10 - 12:50
    - when status change to furture effectove date - it update at time - issue solved - resign on effective date - 12:50 - 
    - When user replaced on effective date it status changed Active -> Deactive - issue solved -  
    - Testing

- User Master testing in Live as per given sheet by roshan sir - 5:40 - 8:30
    - Sync data to mavens api also test


- Git manage for role permission changes with Om - 11:05 - 11:25

# ___________________________________________________________________________________________________________

# 31-03-2026

## Miscellaneous
- In My system Testing is running (testing by it support team) - 10:25 - 10:50
- System issue - it display blue screen error (2 times)
- System Issue, Tilakbhai and Rahulbhai solving issue - 4:25 - 4:45

## Empower HH
- Progress review meeting - Client Meeting - 1:00 - 1:25

- Latest code merge and upload in UAT - Role Permission changes and User master changes - DB change - 10:50 - 11:20

- User Master changes - 11:40 - 1:00, 1:25 - 1:45, 2:15 - 4:25, 4:45 - 7:45
    - User Master Testing (Replacement and Vacancy Testing, etc.), Issue found and solved that issues
    - store vacant_id when generate vacancy
    - make null vacant_id when vacancy full fill 
    - when user replacement on same level it have issue 

- Help to Team
    - Upload Latest change of OM for Role permission changes in UAT
    - Exaplain Bugs, take updates

#
- Add new entry in _mavens table, no update exisiting (new add with end date as old) 
#


# --- 
- on replacement -> all data save of vacant/resign user
- on resign/deactive change end date in all mavens
- Generate vacancy for all roles (for BE and SBE also)
- generate vacancy testing

- 11-03 (9.21)

# --------------------

- User Hierarchy Export Date Month wise, year wise
- BE Hiearchy Export ma - Promoted and Replaced ma Blue Color karvo

- function generate to generate vacancy - 

- Doctor order is on hold then no field staff can order of that doctor 


- User Hierarchy manully verify -  - 



######

- Create Users for Role Permission demo 

- All day validation cron ma only working days count krava (no count sunday)

- Order Reassign functionality demo to komal ma'am (Monday)

- User Deactive on effective date Cron

- Active user data based on effective date cron
- User hiearcy on effectivr date change 


- Manually Deleted Duplicate Order Tagging (Live)


- sync from Mavens data Testing


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
