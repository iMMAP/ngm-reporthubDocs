## Cluster Module

Inside Cluster Module there are Dashboard Feature and Reports Feature.

Dashboard Feature purpose  to summarize all data collected by ReportHub and then show it to user
Report Feature is to create report based on project and record every progress of the project by user

### Reports
 
Report Have 3 main funtion

#### 1. Project Plan/Detail
Controller: ClusterProjectDetailsCtrl

![title](img/project_detail_diagram1.png)

The purpose of this controller is to make new  Project Detail/Plan or to retrieve Project Detail/Plan that already made. In the Project Detail there are 3 main form

-	From Project Plan (mandatory)
-	Form Target Location ( mandatory)
-	Form  Target Beneficiaries (optional)
-	Etc.

All form above manage by  ClusterProjectFormDetailsCtrl.

Controller : ClusterProjectFormDetailsCtrl

![title](img/project_detail_diagram2.png)

Within this controller there are several services used, are as follows

- ngmClusterLists : to provide list that used in the form like list activities, list clusters and many more
- ngmClusterHelper : to create or set up new project 
- ngmClusterBeneficiaries: to set form for target beneficiaries 
- ngmClusterLocations: to set up the location in target location form
- ngmClusterValidation : to validate form 

Function in this controller

- addLocation           :  function to add location in target location form. this function get the template attribute from function addLocation     
                           **ngmClusterLocations**.
                           and set list Admin1,2,3 (Province,district and etc.) for the form using function filterLocations() in **ngmClusterLocations**.
- addLocationFromFile   :  function to add location by uploading file (CSV or Excel). 
- addBeneficiary        :  to add target beenficiary for the project . this function get the template attribute from 
                           addBeneficiary **ngmClusterBeneficiaries**. and set the list for input in target beneficiary form. 
- validate              : function to validate all form  using ** [ngmClusterValidation validate](/services/#validate "Title") ** function.




#### 2. Financial 
#### 3. Monthly Report



<!-- ## Custom Module -->

<!-- ![title](img/test.png)

Custom Module are Module to make an instant module for specific project or program -->
