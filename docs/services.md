## **ngmUser**
### get()
> use       : ngmUser  
> purpose   : to get user from storage  
### set()
> use       : ngmUser  
> purpose   : to set user to storage  
### unset()
> use       : ngmUser  
> purpose   : to unset from storage  
### hasRole()
> use       : ngmUser  
> purpose   : to check user role  
### hasAnyRole()
> use       : ngmUser  
> purpose   : to match any role  
## **ngmAuth**
### register()
> use       :   ngmAuth
> purpose   :   to register new user in ReportHub
### updateProfile()
> use       :   ngmAuth
> purpose   :   to update user information
### login()
> use       :   ngmAuth
> purpose   :   to login in Reporthub
### passwordResetSend()
> use       :   ngmAuth
> purpose   :   to send request to reset password
### passwordReset()
> use       :   ngmAuth
> purpose   :   to reset password
### logout()
> use       :   ngmAuth
> purpose   :   to logout from ReportHub
### setSessionTimeout()
> use       :   ngmAuth
> purpose   :   to manage user session timeout
### grantPublicAccess
> use       :   ngmAuth
> purpose   :   to setup a public user  
### isAnonymous()
> use       :   ngmAuth
> purpose   :   to check if user is anonymus or not
### isAuthenticated()
> use       :   ngmAuth
> purpose   :  to check if user is login or not
### getUserRoleDescriptions()
> use       :   ngmAuth
> purpose   :   to get user role description
### userPermissions()
> use       :   ngmAuth
> purpose   :   to get user permissions definitions
### canDo()
> use       :   ngmAuth
> purpose   :   to checks if user can edit in input view zones
### getRouteParams()
> use       :   ngmAuth
> purpose   :   to get user route restiction params
### getMenuParams()
> use       :   ngmAuth
> purpose   :   to get user user menu params
### getEditableRoles()
> use       :   ngmAuth
> purpose   :   to get user's allowed roles to edit on users  
## **ngmPermissions**
> In ngmPermissions contain a list of a role to assign user-level access 
## **ngmClusterHelper**
### setForm()
>use        : ClusterProjectFormDetailsCtrl (Page Project Detail ).  
>purpose    :  to add some addional list and some check list based on project information

### getNewProject()
> use       : ClusterProjectDetailsCtrl (Page Project Detail ).   
> purpose   : to set new project 

### getProjectHrpCode()
> use       : ngmClusterHelper.getNewProject().    
> purpose   : to set HRP code for new project based on project admin0pcode or country

### getProjectHrpName()
> use       : ClusterProjectFormDetailsCtrl (Page Project Detail )   
> purpose   : to set HRP code for project based on project admin0pcode or country

### compileInterClusterActivities()
> use       : ClusterProjectFormDetailsCtrl (Page Project Detail )   
> purpose   : to compile all inter cluster activities selected by user 

### compileStrategicObjectives()
> use       : ClusterProjectFormDetailsCtrl (Page Project Detail )   
> purpose   : to compile all stragetic objective selected by user

### compileMpcPurpose()
> use       : ClusterProjectFormDetailsCtrl (Page Project Detail )   
> purpose   : to compile all mpc cash purpose  selected by user

### compileActivityType()
> use       : ClusterProjectFormDetailsCtrl (Page Project Detail )   
> purpose   : to compile all activity type  selected by user

### compileDonor()
> use       : ClusterProjectFormDetailsCtrl (Page Project Detail )   
> purpose   : to compile all donor  selected by user

### getCleanWarehouseLocation()
> use       : ClusterOrganizationStocksFormList (page Stocks)   
> purpose   : to set attribute for location warehouse form and delete unused atrribute/data.

### getCleanStocks()
> use       : ClusterOrganizationStockForm (page Stock Report)   
> purpose   : to  delete unused atrribute/data when add new stock report.

### getCleanTargetLocation()
> use       : ClusterProjectFormDetailsCtrl (Page Project Detail )   
> purpose   : to  set site_id ,site_lng and site_lat of target location attribute based on level location.

### getCleanReport()
> use       : ClusterProjectFormReportCtrl (Page Monthly Report )   
> purpose   : to update entire report  locations attribute ("site_id" ,"site_lng" and "site_lat" ) and beneficiary ("report_status")

### getCountryMenu()
> use       : ClusterProjectProjectsCtrl (Page Project List)  
> purpose   : provide list of country for menu  in project list page

### getRegionMenu()
> use       : ClusterProjectProjectsCtrl (Page Project List)  
> purpose   : provide list of region for menu  in project list page

### cleanCopyProject()
> use       : ClusterProjectFormDetailsCtrl (Page Project Detail )   
> purpose   : to  remove unused attribute from copied project. the attribute that remove is project "id", "updatedAt","createdAt",  
            "project_end_date","project_start_date","project_status" target location and target beneficiary "id",    "project_id" 


## **ngmClusterValidation**

### updateSelect()
> use       : ClusterOrganizationStocksFormList (Page Stocks)  
> purpose   : to update <select></select>  in DOM

### project_details_valid()
> use       : ClusterProjectFormDetailsCtrl, ngmClusterValidation   
> purpose   : to validate form Project Plan


### projectDescription()
> use       :  ngmClusterValidation   
> purpose   : to validate field Project Description in form Project Plan

### activity_type_valid()
> use       : ClusterProjectFormDetailsCtrl, ngmClusterValidation   
> purpose   : to check if user select the activity type or not

### project_donor_valid()
> use       : ClusterProjectFormDetailsCtrl, ngmClusterValidation   
> purpose   : to check if user select donor or not

### targetBeneficiariesValidate()
> use       : ClusterProjectFormDetailsCtrl, ngmClusterValidation   
> purpose   : to validate Target Beneficiary Form

### targetBeneficiaryValidate()
> use       : ngmClusterValidation   
> purpose   : to help **targetBeneficiariesValidate** function to check every attribute in target beneficiary

### targetLocationsValidate()
> use       : ClusterProjectFormDetailsCtrl, ngmClusterValidation
> purpose   : to validate Target Location Form for new form

### targetLocationValidate()
> use       : ngmClusterValidation
> purpose   : to help **targetLocationsValidate** function to check every attribue in target location

### target_locations_valid()
> use       : ClusterProjectFormDetailsCtrl, ngmClusterValidation
> purpose   : to validate Target Location Form for old form

### validatePartial()
> use       : ClusterProjectFormDetailsCtrl, ngmClusterValidation
> purpose   : to validate Target Location Form for old form

### validationInputFromFile()
> use       : ClusterProjectFormReportCtrl
> purpose   : to validate beneficiary from  upload file

### validationStockInputFromFile()
> use       : ClusterOrganizationStockForm
> purpose   : to validate stock from  upload file

### validatiOnprojectDetailsFromFile()
> use       : ClusterOrganizationStockForm
> purpose   : to validate Project Detail from  upload file

### validate()
>use        : clusterProjectFormDetailsCtrl, ngmClusterValidation
>purpose    : to validate all form in Project Plan/Detail page

### validateBeneficiaries()
>use        : ngmClusterValidation, ClusterProjectFormReportCtrl
>purpose    : to validate beneficiaries in monthly report


## **ngmClusterBeneficiaries**

### addBeneficiary()
>use        : ngmClusterBeneficiaries,ClusterProjectFormReportCtrl,ClusterProjectFormDetailsCtrl
>purpose    : to set initial property/atribute for beneficiary or target beneficiary form.

### setLocationsForm()
>use        : ngmClusterBeneficiaries,ClusterProjectFormReportCtrl,ClusterProjectFormDetailsCtrl
>purpose    : set beneficiary form for each location in monthly report using setBeneficiariesForm

### setBeneficiariesForm()
>use        : ngmClusterBeneficiaries,ClusterProjectFormReportCtrl,ClusterProjectFormDetailsCtrl
>purpose    : to set beneficiary form using setBeneficiariesInputs function

### setBeneficiariesInputs()
>use        : ngmClusterBeneficiaries,ClusterProjectFormReportCtrl,ClusterProjectFormDetailsCtrl
>purpose    : to set form for beneficiary form and select which field should show in form based on config.

### updateBeneficiaires()
>use        : ngmClusterBeneficiaries,ClusterProjectFormReportCtrl,ClusterProjectFormDetailsCtrl
>purpose    : to update value attribute of beneficiary (`total_male`,`total_female` and `total_beneficiaries`)

### beneficiaryFormComplete()
>use        : ngmClusterBeneficiaries,ClusterProjectFormReportCtrl
>purpose    : to validate old form beneficiary in monthly report

### removeBeneficiary()
>use        : ngmClusterBeneficiaries,ClusterProjectFormReportCtrl
>purpose    : to remove beneficiary in monthly report

### removeTargetBeneficiary()
>use        : ngmClusterBeneficiaries,ClusterProjectFormDetailsCtrl
>purpose    : to remove beneficiary in project plan/detail

## **ngmClusterLists**

### setLists()
>use        : ngmClusterBeneficiaries,ClusterProjectFormReportCtrl,ClusterProjectFormDetailsCtrl
>purpose    : to return lists 
### getStockLists()
>use        : ClusterOrganizationStockForm, ClusterUploadBeneficiariesStockCtrl, ngmClusterDownloads, ngmClusterLists
>purpose    : to provide lists for stock 
### setClusterLists()
>use        : ngmClusterLists
>purpose    : get list for cluster reporting from API
### setOrganizationUsersList()
>use        : ClusterProjectFormReportCtrl, ClusterProjectFormDetailsCtrl, ngmClusterLists
>purpose    : to get information about organization list user
### getIndicators()
>use        : ngmClusterLists
>purpose    : to provide indicator list for monthly report
### getDeliveryTypes()
>use        : ngmClusterLists
>purpose    : to provide delivery type list for beneficiary
### getMpcPurpose()
>use        : ngmClusterLists
>purpose    : to provide mpc purpose type list for beneficiary
### getMpcMechanismTypes()
>use        : ngmClusterLists
>purpose    : to provide mechanism type list for beneficiary
### getClusters()
>use        : ngmClusterLists
>purpose    : to provide cluster list
### getActivities()
>use        : ngmClusterLists
>purpose    : to provide activities use in project plan/detail
### filterActiveDate()
>use        : ngmClusterLists
>purpose    : to filter activities list by start and date of activity
### getProjectActivityTypes()
>use        : ngmClusterLists
>purpose    : to provide activity type list in project plan/detail
### getOrganizations()
>use        : ngmClusterLists
>purpose    :to provide organization list
### getProjectClasifications()
>use        : ngmClusterLists
>purpose    : to provide project clasification list
### getDonors()
>use        : ngmClusterLists
>purpose    : to provide donor list
### getCurrencies()
>use        : ngmClusterLists
>purpose    : to providw currencies list
### getStrategicObjectives()
>use        : ngmClusterLists
>purpose    : to provide strategic objective list
### getCategoryTypes()
>use        : ngmClusterLists
>purpose    : to provide category type list for
### getUnits()
>use        : ngmClusterLists
>purpose    : to provide unit list
### getBeneficiaries()
>use        : ngmClusterLists
>purpose    : to provide beneficiary type list
### getBeneficiariesCategories()
>use        : ngmClusterLists
>purpose    : to provide beneficiary category list
### getSiteImplementation()
>use        : ngmClusterLists
>purpose    : to provide site implementation list for location
### getSiteTypes()
>use        : ngmClusterLists
>purpose    : to provide site type list for location
### filterDuplicates()
>use        : ngmClusterLists
>purpose    : to remove duplicate object in list
### getStockTargetedGroups()
>use        : ngmClusterLists
>purpose    : to provide stock targeted list for stock
### getHrpBeneficiaries()
>use        : ngmClusterLists
>purpose    : to provide hrp beneficiary type list for beneficary
### getProjectDetails()
>use        : ngmClusterLists
>purpose    : to provide project details list

## **ngmClusterFinancial**  

### validateBudgets()
>use        : ClusterProjectFormFinancialCtrl  
>purpose    : to validate budget form in financial form using validateBudget  
### validateBudget()
>use        : ngmCLusterFinancial  
> purpose   : to validate each attribute in budget form   
### inputChange()
>use        : ngmCLusterFinancial   
>purpose    : to change label back to normal if the label is added  error class  

### updateNumber()
>use        : ngmCLusterFinancial 
>purpose    : to update certain attribute in budget form.  

## **ngmClusterLocations**

### openNewLocation()
>use        : ngmClusterLocations  
>purpose    : to open location form  and set attribute (using addLocation function) in monthly report page  

### addNewLocation()
>use        : ngmClusterLocations  
>purpose    : to add new location  in monthly report page  
### addLocation()
>use        : ngmClusterLocations, ClusterProjectFormDetailsCtrl  
>purpose    : to set attribute for location form    
### removeLocation()
>use        : ngmClusterLocations  
>purpose    : to remove location in target location  in project detail/plan    
### showReporter()
>use        : ngmClusterLocations,ngmClusterLocations, ClusterProjectFormDetailsCtrl  
>purpose    : to show list of user that make a report  
### adminOnChange()
>use        : ClusterProjectFormReportCtrl  
>purpose    : to change list if admin1, admin2 or admin3 is changing  
### updateReporter()
>use        : ngmClusterLocations,ngmClusterLocations, ClusterProjectFormDetailsCtrl  
>purpose    : to update reporter(list of user that make a report)  
### updateSiteImplementation()
>use        : ngmClusterLocations  
>purpose    : to update site implementation list in location form  
### updateSiteType()
>use        : ngmClusterLocations  
>purpose    : to update site type list in location form  
### updateAdminSite()
>use        : ngmClusterLocations  
>purpose    : to update site name list in location form  
### updateLocation()
>use        : ngmClusterLocations  
>purpose    : to update location   
### filterLocations()
>use        : ngmClusterLocations, ClusterProjectFormDetailsCtrl  
>purpose    : to filter Location admin 1,admin2,admin3,admin4,admin5 and adminsite list  
### resetLocations()
>use        : ngmClusterLocations  
>purpose    : to reset location property/attribute  
### setLocationAdminSelect()
>use        : ngmClusterLocations, ClusterProjectFormDetailsCtrl  
>purpose    : to set list Location admin1,admin2,admin3 in location form  
### setSiteTypeAndImplementationSelect()
>use        : ngmClusterLocations, ClusterProjectFormDetailsCtrl  
>purpose    : to set list of site_type && site_implementation in location form

  
  
  
  
