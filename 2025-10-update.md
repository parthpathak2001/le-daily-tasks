# 01-10-2025

## Empower HH
- 09:59 - 10:15

- Download Tagging PDF changes - 10:15 - 11:30, 11:39 - 12:25

- Product Multiple division changes - 12:56 - 2:08, 2:32 - 
    get_products
    count_products
    get_order_approval_list - Doctor Division
    count_order_approval_list - Doctor Division
    fetch_division_wise_users
    get_products_by_divisions
    get_zbm_users_by_products
    get_division_heads_by_products - Doctor Division
    has_pending_tagging_approval - Doctor Division
    get_order_details - Doctor Division

- Meeting with php team, regarding task management - 12:25 - 12:56

# ____________________________________________________________________________________________________________________

# 06-10-2025

## Empower HH
- 10:02 - 10:20

- Live Server Backup - 10:20 - 10:45, 11:37 - 12:30


- meeting - 11:17 - 11:37 


- Product import, Product name not proper changed it manually - 12:30 - 2:05, 5:30 - 5:45

- Upload State , Stockiest and Chemist, Database changes - 2:46 - 5:18
 
- API changes - Multiple state supports, Uploaded latest code in UAT - 6:00 - 6:55
    Order Approval List
    Discount Approval List
    get authority user for loggedin
    notification count api (has pending order approval, has pending discount approval)

- Chemist List changes (Web) - Edit Mobile number option - 6:55 - 7:26

- Notification not sending to multiple state authority user issue, uploaded code in UAT and Live - 7:26 - 8:50

- Doctor user mapping data store in Live DB Manually  - 8:50 - 9:10

- Doctor Sync, State is not proper so import doctor properly with state - 9:10 - 12:00

## Cost Management 
- Explain task to Siddh - 10:45 - 11:10
- Sync Functinality explain and help to add in le_worklog - 5:45 - 6:00

# ____________________________________________________________________________________________________________________

# 07-10-2025

## Empower HH

- Doctor mapping - Display User's SPE, and Doctor Code, Chemist Code, Stockist Code - 10:58 - 11:17, 11:23 - 11:50, 12:50 - 1:10, 3:46 - 4:05
    Doctor Mapping section - displayed doctor code
    Doctor Chemist Stockist Mapping Section - displayed doctor code, stockist code, chemist code
    Users List section - displayed employee code
    Additional Options section - displayed chemist code
    Map Division User For Tagging section - displayed employee code

- Doctor Mobile number Edit - 5:20 - 5:35, 6:50 - 7:00
- Chemist Mobile number Edit - 5:05 - 5:20
- upload changes in Live and Tested in Live - 7:00 - 8:00

- Stockist mail changes, Send mail to stockist - 5:35 - 5:55

- Doctor import in live, it not stored state id proper so import using CSV - 11:50 - 12:50, 1:10 - 2:09


- Tagging sheet download issue, html file not found issue - 4:05 - 4:14, 4:19 - 4:40

- Doctor mapped with user (durgesh) - 2:27 - 3:00
- change data given by komal, create new chemist data manually, user doctor mapping data - 3:00 - 3:46, 4:39 - 5:05, 6:20 - 6:50

- Is Authority & Is Division head not working in Live because changes not uploaded in Model, issue solved - 5:55 - 6:20

# ____________________________________________________________________________________________________________________

# 08-10-2025

## Empower HH

- 10:10 - 10:30

- Order Details page changes (web), Order with Tagging Pdf Download changes (API)   - Displyed dash (-) if chemist, stockist, doctor not exist and changed date format in pdf - 10:30 - 11:17, 11:22 - 11:41
    Uploaded code in Live and Tested in Live
    Uploaded code in UAT and Tested in UAT

- Store log when Send OTP, Uploaded in UAT and Live and Tested - 11:41 - 12:25

- Checked doctor code, stockist code, chemist code, employee code displaying or not in Web, if not displayed it, uploaded and Tested in Live - 12:25 - 12:45, 1:35 - 1:47, 2:20 - 2:44, 3:21 - 3:35, 4:55 - 5:50
    Stockist List 
    Order List
    Order Details
    
- SMS not sending issue, we checked log and test again but issue not found and its working (then we called directly to field staff and guide to send otp and its worked) - 12:45 - 1:25

- Doctor data update manually, store uni (komal) - 1:25 - 1:35

- Added Discount Log in Live and Tested - 1:47 - 2:20

- User Edit issue, when changing division or role it not remove old data some times, issue solved and uploaded in live and tested  - 3:35 - 4:55

- stored created_at and updated_at from code India timezone, because it store other timezone date from database, uploaded in live and tested - 5:50 - 6:50

- Stockist List (Web) changes - displayed email in list, created update email popup - 6:50 - 7:45

## Miscellaneous
- added worklog - 7:45 - 8:05

# ____________________________________________________________________________________________________________________

# 09-10-2025

## Empower HH

- 10:23 - 10:35

- Status change to on_hold and expired Cron code review - 10:35 - 11:18, 11:25 - 12:10 

- Store log when cron run, uploaded in Live and UAT, Tested - 12:10 - 12:40

- Create Order API changes - change validation message when order tagging not done, order is on_hold or expired - 12:40 - 1:07
    uploaded in live and UAT and Tested

- Order changes - 1:07 - 2:19
    Cron changes - checked order_reverted_at date when order status changed to on_hold or expired
    Stored date in order_reverted_at when order status revert
    Uploaded in UAT and Live, Tested

- Whatsapp Message, Checked business portal and developer portal, phone number not verified, it displays unverified then verified using OTP and its status changed to pending, Discuss with Neha - 2:57 - 3:25, 4:17 - 4:30, 5:15 - 5:45

- Product name is not proper in Live database, issue is product name is corrupted in csv, I changed that name manually - 5:45 - 6:10

- Cron for sending Remember Notification daily 2 times - 3:25 - 4:11, 6:10 - 7:40
    Created Order Pending Approval, Discount Pending Approval, Order Tagging Pending Approval notification cron
    Cron Log stored, created new table 'cron_logs'

## Miscellaneous

- Sahilbhai Farewell Event - 4:30 - 5:15


# ____________________________________________________________________________________________________________________

# 10-10-2025

## Empower HH

- 10:16 - 10:25
- Cron changes - 10:25 - 11:22,
    Approval pending reminder notification cron set
    Used try-catch in crons and stored error logs  

-  Order Create API changes, Added validation - if doctor not have approved discount then not place order - 11:28 - 12:10

- Cron issue - 12:10 - 1:28, 2:05 - 2:30
    Cron not at set time issue, resolved its timezone issue
    Notification not sending if application not running issue - checked 

- Whatsapp documentation checked - Neha said they added payment getway so i checked message sending or not using api but still not sending message using api - 2:30 - 3:15

- Store log when order tagging pdf download, uploaded in Live and Uat - 3:15 - 3:50

- send otp in whatsapp function changes, set function where otp is sending - 3:50 - 04:02

- Doctor mapping page changes (Web) - 4:02 - 4:13, 4:23 - 4:31, 4:35 - 6:55
    cannot update only discount status issue, resolve: made stockist optional
    cannot allow discount yes if mapping not exist validation added
    added clear dropdown functionality to chemist and stockist dropdown 

- Chemist and Doctor data update, requested by komal - 20 min

# ____________________________________________________________________________________________________________________

# 13-10-2025

## Empower HH
- Created a sheet for Notifications, OTP sending, Reminder notifications, and Expire/Hold Order Cron. 
    Sent the sheet to Komal for review. - 11:15 - 12:55 (ADDED WORKLOG)

- Whatsapp API working or not checked, its not working, its display "Add Payment Method" - 12:55 - 1:10, 1:20 - 1:27, 1:40 - 2:00 (ADDED WORKLOG)
    Added Payment Method

- Discount Edit page changes - stored decimal discount (web) - 1:10 - 1:20, 1:28 - 1:40, 2:00 - 2:07, 2:27 - 2:35, 2:45 - 3:10 (ADDED WORKLOG)
    Department Edit page changes - stored decimal discount in maximum discount (web)
    Stored log when admin update discount (web)
    Uploaded in Live and UAT

- Maven sheet check and send to Komal - 3:10 - 3:30, 5:25 - 5:40 (ADDED WORKLOG)

- issue: when order invoice verified it store tagging without checking division, issue solved: checked product and doctor division and then tagged spe amount - 3:30 - 5:25, 5:40 - 6:10, 7:10 - 7:23 (ADDED WORKLOG)
    corrected order data and order tagging data manually

- Order Details page changes - Send OTP - 6:10 - 6:23, 7:23 - 8:10 (ADDED WORKLOG)
 
- whatsapp support meeting with Neha - 6:45 - 7:10 (ADDED WORKLOG)

- internal meeting regarding new changes - 6:23 - 6:45 ( ADDED WORKLOG)

## Miscellaneous
- Electricity issue - 10:15 - 11:15 (ADDED WORKLOG)

# ____________________________________________________________________________________________________________________

# 14-10-2025

## Empower HH
- Doctor Sync Code changes - 10:45 - 11:12, 11:17 - 11:45
    store state prefix wise, no update existing data, create only new data if not exist 

- import Chemist From mavens sheet - 11:45 - 12:20, 12:56 - 1:35, 2:05 - 2:17, 2:56 - 3:45
    sheet checked
    11679 existing chemist, total 11706 chemist, 27 chemist not exist in new maven data
    11679 updated

- import Doctor from mavens sheet - 3:45 - 6:45
    941 doctor new (checked using doctor code)

- import doctor-employee mapping from maven sheet - 6:45 -  11:05

- order approval issue - 12:20 - 12:56

## Miscellaneous
- Computer issue, Chassis Fan not detect issue, - 10:23 - 10:45
- Shubham Birthday event - 1:35 - 2:05


# ____________________________________________________________________________________________________________________

# 15-10-2025

## Empower HH

- 11:52 - 12:10

- imported data review, checked doctor found or not, employee found or not - 12:10 - 2:10
    checked why doctor_id and user_id is null 
    checked some data is currupted in provided sheet
    review imported data

- Doctor Mapping page - Map Division User For Tagging Section changes - 2:10 - 2:22, 3:35 - 4:00
    display all users not only active user for tagging
    Uploaded in Live & UAT, Tested

- Resend Order OTP API changes - 2:56 - 3:35
    If chemist not available not send otp to chemist
    Uploaded in Live and UAT, Tested

- Api log store functionality developed - 4:00 - 4:10, 5:10 - 5:40, 5:50 - 6:20
    store all api requests in logs
    Uploaded in Live and UAT, Tested
    
- UAT server git is currepted - 4:10 - 4:23, 4:29 - 4:45, 5:00 - 5:10, 5:40 - 5:53
    uploaded new .git folder

## Miscellaneous
- Explain Task to siddh - 4:45 - 5:00, 6:45 - 7:10
    Order Details page changes - Print and excel functionality

- Worklog added - 6:20 - 6:45


# ____________________________________________________________________________________________________________________

# 16-10-2025

## Empower HH
- 10:11 - 10:30

- Password Reset Mail template changes, make proper design, (Web & App) - 10:30 - 11:00, 12:00 - 12:35
    Uploaded in Live & UAT, Tested

- Revert Order Status Action changes - Open modal when click that action and get date, and when cron run for hold & expire order checked revert_status_date - 11:40 - 12:00, 12:35 - 2:04, 3:42 - 5:50
    Order List changes (web) - store deadline date & time when revert status
    make order_reverted_at null when order status change
    check deadline date in crons

- SMTP mail changes - 5:50 - 6:20
    checked new smtp working or not, its not working
    logging that google account but it added 2 step verification so not logged in 


- whatsapp developer and businees portal checked with harsh and neha - 2:53 - 3:22

- meeting with snehalbhai, ravi, harsh, durgesh regardiing partial invoice changes, other changes - 3:22 - 3:42

- Partial invoice functionality, Fieldstaff partial tagging invoice product quantity - 6:20 - 7:35  
### Siddh Help
- Order Details - Uploaded changes in Live and UAT, Tested - Print button functionality added by Siddh - 11:00 - 11:40, 6:20 - 6:50

## Miscellaneous
- Add Worklog - 6:50 - 

# ____________________________________________________________________________________________________________________

# 17-10-2025

## Empower HH
- 09:05 - 09:15

- Partial invoice functionality - 09:15 - 11:30
- Partial Order tagging - 11:30 - 11:54

- meeting with harsh regarding new changes - 11:54 - 12:10

- SMTP creation - 12:10 - 2:15
    Login given account using backup code
    setup 2 step verification in google account
    Create SMTP account - App Password
    send only New mails from this SMTP (Order details mail to stockist) 

- Checked mavens s3 bucket sheet, make a list and send to Komal, Explain to Ravi bhai - 3:00 - 3:15, 4:35 - 5:10

- Diwali event (games, gifts, etc.) - 3:20 - 4:35, 5:10 - 5:45

# ____________________________________________________________________________________________________________________

# 19-10-2025

## Empower HH
- 9:27 - 09:50

- Order Details API changes - 09:50 - 12:10
    add Invoice details in response
    add product details invoice-wise in response

- Order Verify API changes - 12:10 - 1:30, 2:07 - 3:10
    Order Tagging based on uploaded invoice products
    status management
    managed invoicewise product data 
    sens notification user changes - get invoice wise product's divisions users 

- Resend Order Invoice OTP API - create new api - 3:10 - 4:03

- Approve Order Tagging API changes  - 4:10 - 5:35
    understanding how to manage statuses when approve order tagging, help of harsh
    if all tagging of purticular invoice is approved by division head, change the status of invoice completed

## RMIS
- Help ravi bhai to creating whatsapp template - 5:35 - 6:05

# ____________________________________________________________________________________________________________________

# 27-10-2025

## Empower HH
- 10:02 - 10:30

- Approve Order Tagging API changes  - 10:30 - 1:42
    if all tagging of purticular invoice is approved by division head, change the status of invoice completed
    change order status to completed if all invoice tagging is approved and change order status to partially_completed if all invoice tagging not approved 
    store invoice number, invoice date, invoice value, invoice discount value in order_invoices table 
    Uploaded in UAT and Tested

- generate_order_pdf API changes - Download Order details with Tagging - 2:53 - 3:10, 4:33 - 7:20
    Generate PDF by Invoice instead of order
    Employee tagging by Invoice
    Display all other details by Invoice

- Order Approval API changes - Send order details to Stockist mail template changes, displayed product data like old template (displayed PTR VALUE, DISCOUNT, DISCOUNT VALUE, NET VALUE) - 3:10 - 4:27


- Mavens Sheet checked with ravibhai, understanding how to manage Employee hierarchy from sheet - 60 mins 

- Manualy update doctor-user mapping data (requested by Durgesh) - 30 mins

## Miscellaneous
- Add Worklog - 7:20 - 7:35
- Sync Mavens Doctor and Chemist Data with Ravi bhai - 7:35 - 9:38 


# ____________________________________________________________________________________________________________________

# 28-10-2025

## Empower HH
- 10:16 - 10:30

- Uploaded Darshil code in UAT and Tested - 10:30 - 11:00
    Order List - Setting for update Order Variation Percentage (Percentage for order invoice upload maximum price validation)

- Mavens Sheet checking with ravi bhai - 11:21 - 12:30, 1:05 - 1:40
    mavens sheet data check with our employee data manually 
    checked all date wise sheets data and check differences
    understanding employee hierarchy
    division sheets checking
    
- Order List API changes - 11:00 - 11:17, 12:30 - 1:05
    Display those orders that are tagged with the logged-in user

- Order Approval List API changes checked, Multiple invoice changes checked - 1:40 - 2:16

- Import Employee Data from Mavens Sheet - 3:11 - 7:35
    Head Quarter data (hq.csv)
    Employee data (employee.csv, empaccmgrmap.csv, accmgrrelation.csv)

## Miscellaneous
- Add worklog - 7:35 - 8:00

# ____________________________________________________________________________________________________________________

# 29-10-2025

## Empower HH

- Import Employee Data from Mavens Sheet - 10:36 - 1:15
    store division_setup (4/9) in state_master table
    store division_code in department_master table
    import emp_division_csv (empdivision.csv), update is_active, delete is_active == 0  
    store state_id in employee_csv
    store division_id in employee_csv (some data not updated because of data mismatched)

- Import Employee Data from Mavens Sheet - 1:15 - 2:35, 3:34 - 4:30
    Store account_manager_emp_code and parent_acm_emp_code acc_mgr_relation_csv table
    Store account_manager_id and parent_acm_id acc_mgr_relation_csv table , find by emp_code
    store Employee Hierarchy
    store and update user_master from employee_csv
    import emp_role_csv (emprole.csv)

- Created API Script to store Employee Hierarchy. -  4:30 - 8:36
    Stored hierarchy data from acc_mgr_relation_csv into users_hierarchy table
    Uploaded table changes in Live server


# ____________________________________________________________________________________________________________________

# 30-10-2025

## Empower HH

- Created Script in API for Sync Chemist from dealerdetail.csv file -  10:24 - 11:05, 1:30 - 1:44, 2:01 - 2:31

- questionnaire not showing issue checked (raised by Shaziya) - 11:05 - 1:30
    employee have no division so it not working, employee state is North East and it not have division setup (9D/4D) so it not stored division
    store division of all North East users

- Created Script in API for Sync Doctor from customermaster.csv file - 2:31 - 3:40

- Created Script in API for Sync User-Doctor mapping from custaccmap.csv file - 3:40 - 4:53, 5:01 - 6:25

- Upload Sync Chemist, Sync Doctor, Sync User-Doctor mapping scripts in Live and run day wise scripts - 6:25 - 7:20


# ____________________________________________________________________________________________________________________

# 31-10-2025

## Empower HH

- 10:17 - 10:30

- Notification count API changes - 10:30 - 11:05, 11:35 - 1:20
    is_tagging_approval_pending value changes - Check if ZBM/Division Head has any pending tagging approvals - query changes 
        checked approval is pending or not by users divisions and products divisions
        checked approval is pending or not by order tagging SPEs and user's hierarchy

- issue: division not stored in nepal, bhutan, Andaman and Nicobar's users, issue checked - 11:05 - 11:35
    because division name not matched in mavens sheet and our database table

- Sync Doctor from customermaster.csv, Sync Chemist from dealerdetail.csv Script changes - store status (Active/Deactive) based on start_date and end_date - 30 mins

- Employee Sync Script - 1:20 - 1:52, 2:48 - 5:00, 5:26 - 10:30
    employee.csv
    empaccmgrmap.csv

    empdivision.csv
    emprole.csv
    accmgrrelation.csv

- Notification count API changes - is_tagging_approval_pending value issue check - 5:00 - 5:26


# ____________________________________________________________________________________________________________________

##### PENDING
- Product APIs - multiple price 

- Order APIs - "Settlement" Status - said Harshbhai (need to discuss with ravibhai)

- Use DB transaction at all - PENDING 

- Multiple Invoice Upload - PENDING

- History (LOG) manage karavo (Mapping, Order, ) - PENDING


- SYNC data from Maven - PENDING

- Admin Panel - Order status change from "On Hold & Expired", send otp also - PENDING

- CRON (api url) set - PENDING

- Revert Order Status (Admin panel), email not working - PENDING

- Doctor not have division (department) - remove dependancy/conditions  - PENDING

- user, with hierarch sync (maven) - PENDING
- product, stockist sync (IBIS) - PENDING

- Dashboard load lye che e check krvu (su load lye e check krvu)

- Product - multiple division - PENDING

--

- Whatsapp OTP, Meta ma -> API Setup ma CURL thi krvanu, Credentials set kri ne - PENDING

- doctor master ma State prefix store kravu (LIVE) - PENDING 
    (UPDATE doctor_master SET stateprefix = (SELECT zzz_doc_state.stateprefix FROM zzz_doc_state WHERE zzz_doc_state.doctorcode = doctor_master.doctor_code LIMIT 1) WHERE stateprefix = ''  LIMIT 20000)

---
- On_hold and Expired exact time e thava joi - (e research krvanu che) - PENDING

######
