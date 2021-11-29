## **Custom Filter in Reporthub**

### 1. Slice
>purpose : to copy of a portion of an array/string into a new array/string object selected from start to end

>snippet : `| slice:start:end`  
Example :

```
<div align="left" style="padding: 20px;" ng-if="panel.minimize.open">
		<a style="margin:5px;" ng-repeat="form in panel.forms" href="{{ form.form_url }}" target="_blank" title="Go To {{ form.form_title }}" class="waves-effect waves-light btn">
        <i class="material-icons left">assignment_ind</i>
        <!-- You can use it like this -->
        FORM: {{ form.form_title | slice:18:100 }}
        </a>
	</div>
```
### 2. Split
>purpose :  to divide string based on input character and index put by user  

> snippet: `| split:'char ':index`
Example :

```
<td data-title="'Block'" sortable="'admin4name'">
									<div ng-if="row.admin4name">
										Block {{ row.admin4name | split:'Block ':1 }}
									</div>
								</td>
```
### 3. Reverse
>purpose : to reverse an array

>snippet : `| reverse `
Example :

```
 <div ng-repeat="location in project.definition.target_locations | orderBy:'createdAt' | reverse track by $index"
                        ng-class="{'add-padding': !detailLocation[$index]}">
 </div>
```
### 4. SumByKey
> purpose :  to sum object by key  
> snippet : ` data|sumByKey:'key'   
`
Example :

```
<td><b>{{ modal.data|sumByKey:'u5male' }}</b></td>
```
### 5. SumByKeys
> purpose :  to sum object by more than one key
> snippet : `data|sumByKey:['key','key']`

Example :

```
<td><b>{{ modal.data|sumByKey:['u5male','u6female'] }}</b></td>

```
### 6. SumArrrayByKeys
>purpose : to sum array of objects by keys
> snippet:  object | sumArrayByKeys:'key1':{ 'keys': 0,'keys': 0 }:skip

Example :

```
<div class="beneficiary-count right">
										<span style="font-size:1.2rem;">
											<i class="material-icons" style="padding-right:10px;">group</i></span>
												<!-- filter in app/services/ngmHelper.js -->
                                                <!-- You can use it like this -->
												{{ location | sumArrayByKeys:'beneficiaries':{ 'total_beneficiaries': 0 }:project.lists.skip | number }}
									</div>
```
### 7. SumArrayofArraysByKeys
>purpose : sum of array of object by keys with max target 2 object

> snippet : object | sumArrayByKeys:'key1': 'key2':{ 'keys': 0,'keys': 0 }:skip
Example :

```
<div class="beneficiary-count right">
										<span style="font-size:1.2rem;">
											<i class="material-icons" style="padding-right:10px;">group</i></span>
												<!-- filter in app/services/ngmHelper.js -->
                                                <!-- You can use it like this -->
												{{ location | sumArrayByKeys:'beneficiaries':'details':{ 'total_beneficiaries': 0 }:project.lists.skip | number }}
									</div>
```
### 8. FilterByArray
>purpose : 

Example :

```

```
### 9. FilterBeneficiary
>purpose : 

Example :

```
<div ng-repeat="beneficiary in project.definition.target_beneficiaries | orderBy:'createdAt' | filterBeneficiary:project.filter" ng-class="{'add-padding': !detailBeneficiaries[$index]}">
</div>
```