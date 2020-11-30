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
  
   

  
  
  
  
