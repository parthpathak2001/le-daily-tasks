# 01-09-2025

## Empower HH
- Order Create API changes - used stockiest from doctor_chemist_map instead stockist_chemist_map - 9:59 - 10:40
    - Get Stockist by Chemist API change - used stockiest from doctor_chemist_map instead stockist_chemist_map

- Resend Order OTP - 10:40 - 11:15 , 11:36 - 11:45,  (+ 10 minute)

- New API created - Order Edit API - 11:45 - 12:14, 12:54 - 1:44  (+ 10 minute)

- Get Doctor API changes - display only is_discount true doctor - 2:15 - 2:39 (+ 5 minute)
- Get Chemists by Doctor API change - Include Stockiest Details in the response - 2:39 - 3:06 (+ 5 minute)
- Login API changes - If api_key is null, generate and update it for api authentication - 3:06 - 3:26 (+ 5 minute)

- Uploaded in UAT and Testing

- GIT setup, uploaded all jatan code to git from bitbucket - 4:21 - 5:38
 
- Meeting with client - 5:38 - 6:44
- meeting with team - 6:50 - 7:10

## EHS Worklog
- Discussion with Athikur regarding new changes (tasks) - 12:39 - 12:54

- run project, change branch - 4:00 - 4:05
- Leave List - Employee can delete leave, leave permission issue - 4:05 - 4:15


## Miscellenious
- Ganeshji Aarti - 11:20 - 11:36
- weekly meeting - 12:14 - 12:39
- add worklog - 6:44 - 6:50, 7:10 - 7:30

# ____________________________________________________________________________________________________________________

# 02-09-2025

## EHS Worklog
- 10:00 - 10:20
- Excel Download Keep permission - 10:20 - 11:09, 11:26 - 11:33, 11:36 - 11:39
    - changed the format of export file to csv 

- Employee Worklog List & Export changes - displayed only active employees in 'Employee Name' filter - 11:39 - 12:25 (added)
- Employee Worklog List & Export changes - added new filter 'Inactive Employee' to display only Inactive employees (added)

- remove Inactive Employee filter, add status filter, change employee filter data active/inactive on change (added)
    list - 12:25 - 1:10
    export - 1:16 - 1:25

- understanding new task, Attendance -> worklog details task , person utilization export changes - 1:25 - 1:40 (added)

- person utilization export changes - displayed '0' instead of blank value   - 1:40 - 2:02 (added)
- Monthly User Attendance -> worklog details changes - In Missing Worklog Dates - display holiday name - 2:23 - 3:10,  (added)
- User Attendance -> worklog details changes - In Missing Worklog Dates - display holiday name - 3:34 - 3:50, 3:54 - 4:00 (added)


## Empower HH
- doctor assign condition remove(temparory) - 1:10 - 1:16 (uat - need to uncomment)
- sample data upload in UAT (Durgesh), assign doctor, give authority to users - 4:30 - 4:50
- sample data add in UAT db - create doctors and chemists, mapping - 4:50 - 5:15 
- understanding hierarchy flow -  5:15 - 6:07
- Get Order API changes - get logged-in user order - 6:07 - 6:27

## Miscellenious
- Ganeshji Aarti - 20 min
- add worklog - 4:11 - 4:30
- Ganeshji Aarti, Visarjan - 6:27-7:13


# ____________________________________________________________________________________________________________________

# 03-09-2025
## Empower HH

- 10:00 - 10:15
- Verify Order API changes - previous changes removed its override by old code when uploading in git (verify only one otp doctor/chemist) - 10:15 - 10:28

- Order Approval List API changes - added hierarchy condition - 10:28 - 11:37, 11:44 - 12:50
    - get data by hierarchy (in previous code getting from user_doctor mapping)

- Discount Approval List API changes - added hierarchy condition - 12:50 - 1:45
    - get data by hierarchy (in previous code getting from user_doctor mapping)

- change given doctors email (durgesh) in UAT DB - 11:37 - 11:44  

- Doctor list API changes - added last_discount_percent, last_discount_status in response - 1:45 - 2:07

- is_authenticate user logged-in - 2:24 - 2:45, 2:59 - 3:31, 4:10 - 4:16, 4:28 - 5:19
    order approval list
    discount approval list

- Discussion with Harsh bhai - 3:31 - 4:10

- Upload in UAT, Setup Git Branch for UAT - 5:40 - 6:36
    make ravi_main branch up to date, merge parth branch, resolve conflicts
    get backup of upload folder
    setup ravi_main brach for UAT 

## EHS Worklog
- testing on UAT - 5:19 - 5:30
    Excel Download Keep permission
    Employee Worklog List & Export changes
    person utilization export changes
    Monthly User Attendance -> worklog details changes
    User Attendance -> worklog details changes

- Added Holiday in Server - 5:30 - 5:35
- remove permission for User to leave_delete - 5:35 - 5:40

## Miscellenious
- Create Cycle for future apis - 6:36 - 6:55
- add worklog - 6:55 - 7:45



# ____________________________________________________________________________________________________________________

# 04-09-2025

## Empower HH

- 9:57 - 10:20

- Upload Invoice of Order API - 11:00 - 11:30, 2:45 - 3:10 , 4:10 - 4:30, 5:00 - 5:55
- Verify Invoice of Order, decide status of order flow-wise and added in database table field comment - 5:55 - 6:25
- uploaded in UAT and tested - 6:25 - 7:05

- notification count api changes - add is_zbm field in response (check role is zbm or not) - 7:05 - 7:35

- old working code removed after git setup, so checking that - 11:30 - 12:10, 12:55 - 1:46, 2:05 - 2:45, 4:30 - 5:00
    created new branch from main and merge latest code on that, it override old code, so issue occurs
    created new branch from main and merge latest code on that manualy, so it not overidde old code
    changed in .gitignore

- Quiz List API not working, it returns error in response, it because of old code is override - 10:20 - 11:00
    errors:
    'Cannot modify header information - headers already sent'
    'Trying to access array offset on value of type null'

## Cost Management
- meeting with snehal bhai - 12:10 - 12:38
- Note changes and understanding it - 12:38 - 12:55

## Miscellenious
- Add worklog - 7:35 - 8:00

# ____________________________________________________________________________________________________________________

# 05-09-2025

## Empower HH

- 10:06 - 10:15

- order_timeline_settings - 10:15 - 10:58, 11:25 - 11:28
- created cron jobs url - 1:17 - 1:55, 2:18 - 2:52, 2:59 - 3:36
    - added new db columns in orders (verified_at, invoice_uploaded_at, invoice_verified_at, tagging_approved_at)
    - verify order API changes - stored verified_at field 
    - upload invoice API changes - stored invoice_uploaded_at field 
    - verify invoice API changes - stored invoice_verified_at field 

- Create Order API changes - Added validation - Field staff can not create order if previous orders are invoice uploaded but within 10 days not create tagging - 3:36 - 4:03 

- upload changes in uat - 4:03 - 4:11


- Quiz API not returns blank array in quiz issue checked, it because of it attempted that quiz maximum time so there adde condition to check attempt and it false so not returning in response - (Ronak) - 12:27 - 1:17

- Meeting with client - 10:58 - 11:25

- order status listing (tagging_pending, tagging_approved, claim_settled), read document  - 11:55 - 12:27 

- tagging flow understanding - 4:11 - 4:21, 4:29 - 4:39


- Upload Invoice API changes - 4:39 - 5:04, 5:19 - 5:34
    added new fields: invoice_no, invoice_date, invoice_value, invoice_discount_value 

- Create Order API changes - 5:34 - 6:20
    generate Refernce number and store
    removed invoice number generation
    Field staff can not create new order if previous orders are on_hold or expired status

## Eligibility
- Eligibility Query take too much load, analisis using Telescope - 11:28 - 11:55
- Meeting regarding availity Amber's response discussion with Ram bhai, EHS team member - 5:04 - 5:19

## EHS worklog
- finding why daily in-out data not storing - 6:20 - 7:13
    finding script in Task Scheduler

# ____________________________________________________________________________________________________________________

# 08-09-2025

## Empower HH

- 10:01 - 10:17

- Verify Invoice API changes - checked otp is expired or not - 10:35 - 11:11
- Upload Invoice API changes - stored otp sent date in db

- Order Details API changes - Added Department(division) id and name in the response- 11:54 - 12:08
- Field Staff (user) by division(department) API - 12:08 - 12:43, 6:37 - 6:53
    change response structure

- Create Order Tagging API, understanding tagging flow - 10:17 - 10:35, 11:17 - 11:54, 12:43 - 1:27, 3:50 - 4:08, 5:00 - 5:22


- Invoice upload size change 5mb - 1:27 - 2:11
    tried from .htaccess but not affect
    changed in php.ini

- Order Approval List API changes - issue on calling multiple time query, we can not use $this->db multiple time in one api it overrite main query issue solved - 2:52 - 3:50

- Upload in git and UAT - 04:08 - 4:21

- Create Order API changes - Field staff can not create new order if previous orders are not filled tagging form within 10 days after invoice verified  - 4:26 - 4:55

- upload in git and uat - 4:55 - 5:00 

- Doctor List API changes -> added is_paginate request params - 5:22 - 5:39 

- User Add/Edit form - add Is Authenticate in User Add/Edit form- 7:27 - 7:51

# Miscellenious
- upload darshil code to UAT and check code - 5:39 - 6:37, 6:53 - 6:57
- add worklog - 6:58 - 7:20

# ____________________________________________________________________________________________________________________

# 09-09-2025

## Empower HH

- 9:47 - 9:55
- Order Management -> chnage status name tagging_pending to tagging_processing - 9:55 - 10:07  (done)

- add courier api issue check with ronak - 11:21 - 11:38

- Doctor Mapping change - 11:46 - 12:15, 12:30 - 1:18

- Product List API - is_paginate - 12:15 - 12:30

- Order Details API changes - Include Tagging Details (Spa name and Spa amount) - 2:54 - 3:27, 04:03 - 04:08, 4:14 - 4:30 
    Add is_zbm in request and send only thier division products - 4:30 - 5:19 (done)

- Tagging Approval API - 5:19 - 6:39, 6:55 - 7:17
- upload task on UAT and testing - 6:39 - 6:55


- assigned doctor not displaying issue checked, it was no issue, he not set is_discount true so doctor not fetched - 3:27 - 3:50

- 3:50 - 3:55

- make darshil branch and help to clone - 3:55 - 04:03 

- discussion with snehalbhai to complete work - 7:17 - 7:45

- Order List - 8:00 - 8:55 (done)



# Miscellenious
- Check Darshil code, review code, testing - Doctor Management, Stockiest Management, Chemist Management, Order Management, Discount Log Management and Upload in Git and UAT and testing on UAT - 10:07 - 11:18, 11:38 - 11:46, 1:18 - 1:59
- help darshil, explain list changes - 7:45 - 8:00

# ____________________________________________________________________________________________________________________

# 10-09-2025

## EHS Worklog
- checked Monthly productivity report data - athikur says your data is not proper i checked it is already proper,  4:52 - 5:30

## Empower HH

- 9:50 - 10:00

- Discount Log List - 10:00 - 11:16, 11:18 - 11:45 (+10 min)
    sidebar menu active not working - solved
    breadcrumb make dynamic 

- Order List - displayed missing data, responsive not working issue, data is displaying outside column issue - 11:45 - 12:40 (+10 min)
    breadcrumb make dynamic
    
- User Add/Edit - added is_division_head - 12:40 - 1:20
    added Note for Disvision head and authority check mark

- Dashboard -  Top Performing User section - php issue displaying regarding array offset solved, uploaded in UAT - 3:10 - 3:27


- upload in UAT and git - 1:20 - 1:40, 2:00 - 2:24, 2:55 - 3:10
    review darshil code
    test darshil code

- notification count api - include is_division_head in response - 3:27 - 3:40, 4:07 - 4:15

- discount not working on uat check, solved and Uploaded - 3:40 -  4:07

- is_discount not storing in UAT, because darshil changed that code - 4:15 - 4:52

- Discount Approval List API changes - issue on calling multiple time query, we can not use $this->db multiple time in one api it overrite main query issue solved - 5:30 - 6:00

- Order detail API changes - include in response of is_zbm approval and is_division_head approval - 6:00 - 6:30

- meeting with snehal bhai, ravi, harsh, durgesh, darshil - 6:38 - 7:16

- task understanding with ravi bhai and time-line - 7:16 - 8:20
## Miscellenious 
- add worklog - 6:30 - 6:38, 8:13 - 8:30



# ____________________________________________________________________________________________________________________

# 11-09-2025

## Empower HH

- 9:45 - 9:58

- upload all latest code in UAT and tested, resolve conflicts - 9:58 - 10:21  

- Doctor management - UNI code changes - 10:21 - 11:20
    added uni in doctor_master table
    store dummy data
    doctor list api - displayed uni of doctor, search also and fetch only doctors having uni code
    get orders api - displayed uni of doctor, search also
    get order details api - displayed uni of doctor
    get_discounts_by_doctors api - displayed uni of doctor
    get_discounts_approval api - displayed uni of doctor
    get_order_approval_list api - displayed uni of doctor

- Order Details API changes - send zbm_approved and division_head_approved as integer instead string - 11:28 - 11:39

- uploaded in UAT and Tested - 11:39 - 11:46

- product price changes - 11:46 - 12:17, 12:46 - 1:00
    stored 3 price 
    used price field as ptr (price to retailer)

- Order Approval list API changes - it returns 500 error when hierarchy users not found issue - solved - 12:17 - 12:36

- Send SPE code (employee code) with employee (field staff) data - 1:15 - 1:50
    order details api
    discounts_by_doctor api
    discounts_approval_list api
    order_approval_list API
    fetch_division_wise_users api

- get order division users API changes - BE & SBE role users only - 1:50 - 2:16

- 2:58 - 3:05

- Order OTP Verification API changes - doctor and chemist otp both verify - 3:50 - 4:04, 4:08 - 4:12
- Order Invoice OTP Verification - doctor and chemist otp both verify - 4:12 - 4:23

- Add/Edit Order API changes - 4:23 - 5:44
    added is_approve in requests and make some changes in edit functionality 
    store discount, stockiest 
    reference number change (store order id as ref no.)

- Order Details API changes - 5:44 - 6:09, 6:15 - 6:40, 6:45 - 6:55
    include doctor_id, chemist_id, stockies_id, reference no., created_by_name, division_head_approved_by_name, zbm_approved_by_name, created_by_spe_code, division_head_approved_by_spe_code, zbm_approved_by_spe_code in response of api

- approve_order_tagging API changes - mark order tagging as completed if it’s fully approved OR if the current user is a Division Head. - 6:55 - 7:10

- Order List api changes - include discount_percent in response - 7:35 - 7:50

- Order List (web) - Default sorting is descending - 7:50 - 8:00

- Save Order Tagging API changes - discussion with harsh - 8:00 - 8:15  

- upload code in UAT, testing - 3:21 - 3:50, 6:40 - 6:45

- Darshil code review, testing, uploaded in git and UAT - 3:05 - 3:21
- help darshil - doctor mapping changes, explained, review, testing - 12:36 - 12:46, 1:00 - 1:15

- help durgesh to add new product and assign to division, set mail in chemist  - 6:09 - 6:15, 7:25 - 7:30

- discussion with harsh regarding changes, order, tagging approval - 7:10 - 7:25

- Save Order Tagging API changes - discussion with harsh - 8:00 - 8:15  

- understanding notification - 8:15 - 8:45
    send_push_notification

# ____________________________________________________________________________________________________________________

# 12-09-2025

## Empower HH

- 9:52 - 10:05

- Notification - 10:05 - 11:40, 11:48 - 2:04, 2:54 - 3:23, 3:30 - 3:57, 4:23 - 6:19, 6:49 - 9:00
    old notification sending code not working so make new notification sending code old is deprecated
    send notifications in new flow 

- Order Details API changes - 3:23 - 3:30

- Order Approval list - created_by_spe_code - 11:40 - 11:43

- upload in UAT - 11:43 - 11:48

- disscussion with durgesh - tagging approval data issue for zbm - 4:10 - 4:20

## Telemed LSPC 
- Export diagnosis Jaya ma'am- 3:57 - 4:10

## Eligibility
- meeting with kapil sir -  6:19 - 6:49

# ____________________________________________________________________________________________________________________

# 13-09-2025

## Empower HH

- 9:40 - 9:50

- Notification -> user fetching testing - 9:50 - 10:10

-  get order division users api - returns user_id, user_name null, issue solved- 10:10 - 10:26
    issue is user_hierarcgy table have data and user_master have no data so display null (solved)

- Discount Approval API changes - 10:26 - 11:04
    added search functionality
    display division-wise data if logged-in user is is_division_head 

- Mail send to stockiest when approve order - 11:04 - 11:30

- upload in UAT and Test, add data for testing - 11:30 - 12:07

-  - 12:07 - 12:40

- testing with Durgesh - 12:40 - 12:53

- tagging sheet generate and download - 12:53 -  1:25, 2:05 - 3:20 - 5:20 - 5:30

- Doctor List API change - display only last approved discount - 1:25 - 1:30

- discussion related to client meeting, get new changes - 3:20 - 3:35, 3:45 - 4:00



- doctor list api issue - discount not proper, get approved data - 5:30 - 6:00

- upload invoice api issue - it not storing data because invoice number is unique - issue solved - 6:20 - 6:40

- Taging api not working - 6:40 -  7:10

- Order Aproval List API changes - display division-wise data if logged-in user is is_division_head - 7:10 - 7: 

- notification testing - 3:35 - 3:45, 4:00 - 5:00, 6:00 - 6:20, 7:10 - 7:15


- data store in database - set division in doctor (durgesh) - 5:00 - 5:20

# ____________________________________________________________________________________________________________________

# 15-09-2025

## Empower HH

- notification changes,  testing - 10:12 -  11:05, 11:20 - 12:20
    tagging notifications checked

    verify_order API changes - notification changes
    add_discount API changes - notification changes
    discount_approval_action API changes - notification changes
    verify_invoice API changes - notification changes

- generate order pdf api issue - 11:05 - 11:20
    not found order pdf html file

- Notification Testing - with Durgesh - 12:20 - 12:40

- get_order_approval_list api changes - displyed all orders that have at least one product belonging to the logged-in user’s division(s). - 12:40 - 1:00

- Order edit api changes  - 1:00 - 1:21
    notification to fieldstaff
    if approved -> send order details to Stockiest (mail)

- Order Tagging Save API changes - notification to ZBM (hierarchy zbm) instead all zbm of division - 1:21 - 1:30, 1:40 - 2:26
    order complete if product approved by their product division head

- Login API change - When user login 3rd time it not return is_manager proper - 1:30 - 1:40
    discuss with harsh

- 3:03 - 3:23
- send Order Details to Stockist in Mail changes - 3:23 - 4:18

- Meeting With Client In Google Meet to explain Application and Web - 4:15 - 5:48

- Set notification at all old places - 4:30 - 5:00
    add_update_courier api

- Order Add/Edit API changes - Chemist not mandatory, if not chemist store only stockiest  - 6:00 - 7:00
    order otp verify api changes
    order list api changes
    added 'chemist_available' field in db table 

- Edit & Approve Tagging API (new) - 7:00 - 8:20


# ____________________________________________________________________________________________________________________

# 16-09-2025

## Empower HH

- 10:07 - 10:35
- Darshil code review, test and upload in server - 10:35 - 11:12

- Order/Discount Approval API changes - added search functionality, check division of product instead user division for count result of order list pagination,  - 11:16 - 12:23
    uploaded in UAT and Tested

- Order Log, Added database transaction - 12:23 -  1:59, 3:30 - 4:12, 4:22 - 5:42
- Discount Log, Added database transaction - 5:42 - 7:05
    - CRON 

- 2:52 - 3:10
- Order list & Order Details API changes - included chemist_available in response - 3:10 - 3:30
    Order Verify API changes - verify only doctor otp when chemist not available 

## LSPC (lspcdata.com) 
- when submit form from home page it returns 405 error, issue checked not resolved - 7:15 - 7:40


# ____________________________________________________________________________________________________________________

# 17-09-2025

## Empower HH

- System Issue - when system starts it display fan not detected, called Rahulbhai to resolve - 10:07 - 10:35 


- verify invoice api changes - if chemist not available then not check otp of chemist, uploaded and testing with durgesh - 11:30 - 12:18

- Order - Claim Settled fucntionality, uploaded in UAT and testing, checked documentation - 12:18 - 12:40, 1:50 - 2:12, 3:03 - 4:51
    it takes time because when merging it given conflicts becasue darshil also works in this 

- Send Otps in whatsapp researching - 4:51 - 5:25, 6:12 - 6:22, 6:30 - 7:12

- Edit & Approve Discount - 5:25 - 6:12 

- Invoice upload api chages - Invoice maximum file upload validation, uploaded and tested - 12:40 - 1:25

- Review code of Darshil and upload in UAT - 10:35 - 11:04
- Explain task to darshil - 11:09 - 11:30
    Order list changes
    invoice display
    discount log changes
- check darshil code, tested and uploaded in UAT - 1:25 - 1:50

- If otp is 123456 then verify order and invoice, send mail to field staff, approver and our mails instead stockiest mail for beta testing- 6:22 - 6:30, 7:12 - 7:50

- Discount Approval List - 7:50 - 8:15


# ____________________________________________________________________________________________________________________

# 18-09-2025

## Empower HH

- 10:03 - 10:10
- Order Edit & Order Approval API changes - added komal mail to send order details mail when approve, and solved is_authority users id fetching issue  - 10:10 - 10:35


- Orders API changes, count orders not displaying right count as per list issue solved - 10:50 - 11:06

- 11:06 - 11:16
 

- Notification changes, store json , listing api changes, uploaded in uat and testing - 11:27 - 1:04  

- Notification changes, user not logged in it not store notification issue, reolve:User not have fcm then also store notification  - 1:04 - 1:41


- Login API changes - remove max device condition from login api for purticular 3 devices for beta testing - 3:20 - 3:35

- chemist import - 3:58 - 4:03
- stockiest import - 4:10 - 4:30
- Product Create under new division - 4:30 - 4:40

- order approval list api changes - it display same order 2 time when it have multiple product and products from same division issue solved - 4:53 - 5:29


- Meta developer portal checked, check for mobile number, check template  - whatsapp otp sent check - 5:29 - 6:45

- Darshil code review, test, uploaded - 10:35 - 10:50, 11:16 - 11:27, 1:41 - 2:00

- Testing for beta testing - 
- 2:29 - 3:00

- 3:00 - 3:20

- 3:20 - 3:48

ordr

## Eligibility
- help darshil 
- 3:48 - 3:58
4:40 - 4:53

## Miscellenious
- Add Worklog, created module - 6:55 - 7:30


# ____________________________________________________________________________________________________________________

# 19-09-2025

## Empower HH
- 9:41 - 10:01 

- 10:12 - 10:17

- change status from on_hold, expired - 10:50 - 11:14, 11:17 - 11:30, 11:55 - 12:15, 12:38 - 2:04, 2:53 - 3:17
    it takes time because email not sending, not resolved

- Order Details API changes - include invoice details in response - 12:15 - 12:38

- Tagging PDF download changes - Display Prepared by data- 3:17 - 3:40

- Sync Doctor - 3:40 - 6:28

- Sync Chemist - 6:28 - 7:00




## Eligibility
- Explain task to darshil, availity response data check, check which data we not displaying in our side - 10:17 - 10:50

## Miscellenious
- Review my worklog with ram sir (previous 2 days) - 11:30 - 11:55

# ____________________________________________________________________________________________________________________

# 22-09-2025

## Empower HH
- 10:00 - 10:20

- Doctor and division no connection, so where i added division condtions i changed it to logged-in user division - 10:20 - 11:18 - 11:22 - 11:40
    doctor list api changes, get maximum_discount and division data of logged-in user
    discounts approval list api changes, get division data by created_by 

- 11:40 - 12:00
- State Sync from Maven CSV, create country if no exist  - 12:00 - 1:07
- Find Speciality Sync from Maven Sheets, not found master sheet - 1:07 - 1:40

- Order List (Web) changes - Field staff search not working, added searching for fieldstaff - 1:40 - 1:55 

- Discount Log List (Web) changes - displayed Rejected By and Rejected At - 2:53 - 3:43
    Discount Approval Action API changes - Stored rejected by and rejected at when Discount Reject
    Discount Approval List API changes - Display Rejected by user name and SPE code and Rejected at

- AWS S3 configuration for Sync data (aws-sdk-php), its not working, it returns "Invalid handle provided" error - 3:43 - 4:14, 4:21 - 7:15


# ____________________________________________________________________________________________________________________

# 23-09-2025

## Empower HH

- 10:16 - 10:40
- AWS S3 configuration for Sync data (amazon-s3-php-class) - 10:40 - 1:30
    first, i created php demo for AWS S3 Bucket
    thenafter i implemented it in our project
    Sync data from AWS S3 Bucket (doctor, chemist, state)
 
- Order details changes, displayed product details same as order details sent in mail - 1:30 - 1:53, 2:41 - 3:20

- 3:20 - 3:45
- Sync Product from Maven, checked sheet it have some confusion, finding division of product - 3:45 - 3:56, 5:05 - 5:55

- Sync User, cheking maven sheets, check how to store hiearchy, checking how to manage role and division - 5:55 - 7:02

- Announcement api check - its working in IOS and not working in Android (shaziya empowerhh), returns data based on hierarchy, check database query - not changed - 3:56 - 4:11, 4:24 - 5:05

# ____________________________________________________________________________________________________________________

# 24-09-2025

## Empower HH

- 10:21 - 10:40

- User Sync from Maven Sheet, its almost done just minor changes is pending, finding connections in given sheet by Maven - 10:40 - 10:53, 1:30 - 2:13

- Meeting with client, Regarding tagging changes, doctor list changes - 3:00 - 3:45
- internal meeting, regarding proper explaination fo changes given by client in previous meeting, future task planing - 3:45 - 4:25

- Doctor Mapping page changes (web) - create new form section to store user tagging division and doctor wise  - 4:25 - 4:45, 4:55 - 7:26

- Notification count API changes, added below details in response - 10:53 - 11:21, 11:25 - 11:35, 11:40 - 1:30
    is_discount_approval_pending
    is_order_approval_pending
    is_tagging_approval_pending


# ____________________________________________________________________________________________________________________

# 25-09-2025

## Empower HH

- 10:25 - 10:35
- Doctor Mapping page changes (web) - manage existing tagging - 10:35 - 1:45, 2:38 - 3:35

- Whatsapp messaging checking with Harsh and Neha, API calling, send message api not working, get phone number api working - 3:35 - 5:20
    generated token, given whatsapp permission

- after uploaded changes in UAT it returns error "Return value of Doctor_model::get_available_chemists() must be an instance of mixed, array returned" - 5:20 - 5:50
- Order Approval API changes - it not displaying Pending data (ronak) - 5:50 - 6:15
- Product List API changes, display product doctor's division wise  - 6:15 - 6:40
- tagging - 6:40 - 8:20

# ____________________________________________________________________________________________________________________

# 26-09-2025

## Empower HH

- 10:14 - 10:35

- Doctor Mapping page changes (web) - Tagging form Validation - 10:35 - 11:25, 2:54 - 4:00
    Alert when Delete selected User or Division
    If total tagging percentage is not 100% then not can not submit   

- Order Approval API changes - 11:35 - 12:10, 12:31 - 2:15
    status wise sorting not working because of distinct (mysql), issue solved
    if logged-in user is is_authority, then sorting otp_verified first, then approved, then rejected, others after
    if zbm or division head logged-in (other user), then tagging_processing first, then tagging_approved, then approved, then rejected, others after 

- order detail changes, product price calculation issue checked, issue not found (raised by ronak, issue is he passed wrong data) - 12:10 - 12:31

- Navaratri event - 4:00 - 5:30

- 5:30 - 5:50
- Doctor List changes (web) - Displayed Mapping status - 5:50 - 6:45 

- 6:45 - 7:19

# ____________________________________________________________________________________________________________________

# 29-09-2025

## Empower HH

- 10:21 - 10:30

- Uploaded latest code in UAT and Tested - 10:30 - 10:55

- Chemist List Changes (web), Removed extra details from listing, displayed only chemist_name, chemist_code, drug_license, state_name - 10:55 - 11:16, 11:20 - 11:47, 12:00 - 12:06

- uploaded privacy policy file in UAT - 11:47 - 12:00

- Whatsapp  - 12:06 - 1:45
    discussion with Snehalbai and Harsh
    create new meta business account
    trying to get test number for otp send but not success


- Test Application Order Flow - 2:00 - 3:00

- creating whatsapp account for OTP Sent, from video tutorials for create account and test number - 6:00 - 7:04
    created business account and developer account from other facebook account because in previous account its not working properly 
    created new app and testing number 

## Cost Management
- Employee Cost Report (Used 'Actual Cost' report - changes in Export and List for Count cost) - 3:00 - 4:21, 4:29 - 4:45
- Hide Reports -> Estimation Cost, Reports -> Estimation Hours, Reports -> Actual Cost - 4:45 - 4:50
- Display Employees and Clients Module, Added new permission - 4:50 - 5:06
- Department List - Remove Action (Average Cost Button) - 5:06 - 5:10
- Employee Cost - Change Date format - 5:10 - 5:25
- Uploaded code in UAT and Tested - 5:25 - 6:00


# ____________________________________________________________________________________________________________________

# 30-09-2025

## Empower HH
- 10:13 - 10:35

- Check stockiest, chemist, users sheets - mobile number exists or not - 10:35 - 11:05 
- announcement api image not exist, downloaded images from live server and uploaded in UAT using command line - 11:05 - 11:26

- 11:32 - 11:40
- Application -> Home screen (Announcement API) display only 3 image issue check on live (shaziya empowerhh)  - 11:40 - 1:15
    pass hardcoded data and checked, set limit and checked, pass purticular image which not displayed and checked
- Empower HH meeting with client - 1:15 - 1:35

- Product have multiple division changes understanding with ravibhai, store division name in alias field from product sheet, In tagging pass alias name if exist - 1:35 - 1:50

- User Sync changes - role, division of user is from other csv so managed it proper - 1:50 - 2:20 , 2:36 - 2:50, 3:28 - 4:05

- Product import in db, create csv and import, Set Division Alias from Maven sheet - 4:05 - 4:22, 4:31 - 6:30

- Meeting With client, giving demo of new changes - 6:30 - 7:30


## Le Worklog 
- explain task to siddh, create siddh branch, help to setup project - 3:06 - 3:28

# ____________________________________________________________________________________________________________________

##### PENDING
- Product APIs - multiple price 

- Order APIs - "Settlement" Status - said Harshbhai (need to discuss with ravibhai)

- Use DB transaction at all - PENDING 

- Multiple Invoice Upload - PENDING

- Whatsapp OTP, Meta ma -> API Setup ma CURL thi krvanu, Credentials set kri ne - PENDING

- History (LOG) manage karavo (Mapping, Order, ) - PENDING


- SYNC data from Maven - PENDING

- Admin Panel - Order status change from "On Hold & Expired", send otp also - PENDING

- CRON (api url) set - PENDING

- Revert Order Status (Admin panel), email not working - PENDING

- Doctor not have division (department) - remove dependancy/conditions  - PENDING

- user, with hierarch sync (maven) - PENDING
- product, stockist sync (IBIS) - PENDING

- Dashboard load lye che e check krvu (su load lye e check krvu)

- Store Date timezone change - PENDING

- Product - multiple division - PENDING

---
- On_hold and Expired exact time e thava joi - (e research krvanu che) - PENDING


- le_worklog changes - Darshil pase karava

--- 

- Cost Management Project - Billable/Non-Billable pn btavu   

- Cost Management Project -  Employee Work Cost list - Display Billable/Non-Billable Hours, Billable/Non-Billable Amount (list ni pla btavu) - PENDING
- Cost Management Project -  Employee Work Cost list - Project and Emplyoee multiselect filter - PENDING 

######
