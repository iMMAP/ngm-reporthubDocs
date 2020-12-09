## **Make New Layout**

## Template layout
To make a new layout in ReportHub there are structure model that need to follow.  
Here the structure :
```
$scope.model       ={
                        name: '',
                        header: {
                            div: {
                                'class': '',
                                style: ''
                            },
                            title: {
                                'class': '',
                                style: '',
                                title: ''
                            },
                            subtitle: {
                                'class': '',
                                title: ''
                            }
                        },
                        rows: [{
                            columns: [{
                                styleClass: '',
                                widgets: []
                        }]
                        },{
                            columns: [{
                                styleClass: 's12 m12 l12',
                                widgets: []
                            }]
                        }]
                    }
```
**Description :**

- **name** : name of the model  
- **header**: Header of the layout  
- **header.div.style** : to style the header
- **header.title**     : to put title text  for header  
- **header.title.style**     : to put style on title text   
- **header.subtitle**  : to put subtitle for header  
- **header.title.style**     : to put style on subtitle text  
- **rows**                   : the container to put columns in one row
- **column**                 : the place to put a component in layout 


For example :
```
$scope.model       ={
                        name: 'tes',
                        header: {
						div: {
							'class': 'col s12 m12 l12 report-header',
							style: 'border-bottom: 3px  solid;'
						},
						title: {
							'class': 'col s12 m12 l12 report-title truncate',
							style: 'color: blue' ,
							title: 'Testing'
						},
						subtitle: {
							'class': 'col s12 m12 l12 report-subtitle hide-on-small-only',
							title: 'testing'
						}
					},
                        rows: [{
                            columns: [{
                                styleClass: '',
                                widgets: [{
									type: 'html',
									card: 'card-panel',
									style: 'padding:0px; height: 90px; padding-top:10px;',
									config: {
										*optional*
									}
								}]
                        }]
                        }]
                    }
```
In example above the ngm-html widget is component that we call
