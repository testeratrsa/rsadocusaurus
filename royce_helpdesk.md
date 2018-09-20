## Helpdesk

### Project List

> ##### SQLite Information  
> Fully online, so no Table


##### Project List Webservice Request

`POST Method`

|Parameters|Values|
|---|---|
|module|getHelpDeskProjectList|


##### Project List Webservice Reponse


###### ![#c5f015](https://placehold.it/15/c5f015/000000?text=+) Correct Response:- 

```json
{
    "message": {
        "success": "true",
        "data": {
            "result": [
                {
                    "project_id": 11,
                    "project_name": "Alkepedia",
                    "project_icon": "uploads/help_logo/alkem.png",
                    "total_tickets": 28,
                    "bug": 13,
                    "support": 12,
                    "changerequest": 3,
                    "done_closed": 17,
                    "done": 0,
                    "inprocess": 0,
                    "others": 11,
                    "bug_id": 1,
                    "support_id": 2,
                    "changerequest_id": 3,
                    "done_closed_id": 6,
                    "done_id": 7,
                    "inprocess_id": 9,
                    "others_id": "others"
                },
                {
                    "project_id": 8,
                    "project_name": "Apexa",
                    "project_icon": "uploads/help_logo/apexa.png",
                    "total_tickets": 35,
                    "bug": 9,
                    "support": 25,
                    "changerequest": 1,
                    "done_closed": 20,
                    "done": 5,
                    "inprocess": 1,
                    "others": 9,
                    "bug_id": 1,
                    "support_id": 2,
                    "changerequest_id": 3,
                    "done_closed_id": 6,
                    "done_id": 7,
                    "inprocess_id": 9,
                    "others_id": "others"
                }
            ]
        }
    }
}
```

###### ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Wrong Response:- 

```json
{
    "message": {
        "success": "false",
        "data": {
            "result": [
                {
                    "message": "Invalid Module Name"
                }
            ]
        }
    }
}
```

##### Project API relation table
> No Table relation, fully online



### Project Ticket List
> ##### SQLite Information  
> Fully online, So no table


##### Project Ticket List Webservice Request

`POST Method`

|Parameters|Values|
|---|---|
|module|getHelpDeskList|
|userid `not mandatory`|629|
|project_id|11|
|ticket_type_id `not mandatory`|3|
|status_id `not mandatory`|6|

##### Project Ticket List Webservice Reponse


###### ![#c5f015](https://placehold.it/15/c5f015/000000?text=+) Correct Response:-  

```json
{
    "message": {
        "success": "true",
        "data": {
            "result": [
                {
                    "ticket_id": 37,
                    "comments": "",
                    "ticket_description": "Uploded users are not reflecting in user master",
                    "assigned_to": "User",
                    "project_name": "Alkepedia",
                    "created_date": "2018-06-20 18:39:37",
                    "platform_name": "Portal",
                    "type_name": "Service Request",
                    "module": "Adminpanel",
                    "priority_name": "Medium",
                    "status_name": "Done & Closed",
                    "instance_name": "Production",
                    "assigned_to_user": "Maharaja ",
                    "assigned_to_group": "",
                    "file_path": "",
                    "created_by": "Deepali Nehete"
                },
                {
                    "ticket_id": 233,
                    "comments": "",
                    "ticket_description": "Old issue tickets which are done and closed.",
                    "assigned_to": "User",
                    "project_name": "Alkepedia",
                    "created_date": "2018-07-21 16:58:15",
                    "platform_name": "Portal",
                    "type_name": "Service Request",
                    "module": "Done and closed tickets",
                    "priority_name": "Medium",
                    "status_name": "Done & Closed",
                    "instance_name": "Production",
                    "assigned_to_user": "Maharaja ",
                    "assigned_to_group": "",
                    "file_path": "",
                    "created_by": "Rahul Kaushik"
                }
            ]
        }
    }
}
```
###### ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Wrong Response:- 

```json
{
    "message": {
        "success": "false",
        "data": {
            "result": [
                {
                    "message": "No Available Datas"
                }
            ]
        }
    }
}
```

##### Project Ticket List API relation table  
> No Table relation, fully online


### Ticket Detail List


> ##### SQLite Information  
> Fully online, So no table


##### Ticket Detail List Webservice Request

`POST Method`

|Parameters|Values|
|---|---|
|module|getHelpDeskList|
|ticket_id|37|



##### Ticket Detail List Webservice Reponse


###### ![#c5f015](https://placehold.it/15/c5f015/000000?text=+) Correct Response:-  

```json
{
    "message": {
        "success": "true",
        "data": {
            "result": [
                {
                    "ticket_id": 37,
                    "comments": "",
                    "ticket_description": "Uploded users are not reflecting in user master",
                    "assigned_to": "User",
                    "project_name": "Alkepedia",
                    "created_date": "2018-06-20 18:39:37",
                    "platform_name": "Portal",
                    "type_name": "Service Request",
                    "module": "Adminpanel",
                    "priority_name": "Medium",
                    "status_name": "Done & Closed",
                    "instance_name": "Production",
                    "assigned_to_user": "Maharaja ",
                    "assigned_to_group": "",
                    "file_path": "",
                    "created_by": "Deepali Nehete"
                }
            ]
        }
    }
}
```

###### ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Wrong Response:- 

```json
{
    "message": {
        "success": "false",
        "data": {
            "result": [
                {
                    "message": "Invalid Module Name"
                }
            ]
        }
    }
}
```

##### Ticket Detail List API relation table  
> Fully online, So no table


### Helpdesk Picklist  

> ##### SQLite Information  
> Fully online, So no table


##### Helpdesk Picklist Webservice Request

`POST Method`

|Parameters|Values|
|---|---|
|module|getHelpDeskPickList|


##### Helpdesk Picklist Webservice Reponse


###### ![#c5f015](https://placehold.it/15/c5f015/000000?text=+) Correct Response:-  

```json
{
    "message": {
        "success": "true",
        "data": {
            "result": [
                {
                    "id": 1,
                    "name": "Edelweiss",
                    "pick_flag": "PROJECT"
                },
                {
                    "id": 2,
                    "name": "Burgerking",
                    "pick_flag": "PROJECT"
                }
            ]
        }
    }
}
```

###### ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Wrong Response:-    

```json
{
    "message": {
        "success": "false",
        "data": {
            "result": [
                {
                    "message": "Invalid Module Name"
                }
            ]
        }
    }
}
```

##### Helpdesk Picklist API relation table  
> No Table relation, fully online



### Submitting Ticket Details

> ##### SQLite Information  
> Fully online, So no table

##### Submitting Ticket Details Webservice Request

`POST Method`

|Parameters|Values|
|---|---|
|module|putHelpDeskTicket|
|data|[{"ticket_id":"257","project_name":"4","platform":"1","ticket_type":"2","module":"Attendance & Call Average","ticket_description":"Move the Attendance & Call Average report to Production server its done in UAT.","priority":"1","project_instance":"1","assigned_to":"User","assigned_to_user":"606","assigned_to_group":"","status":"6","ticketdesc":"Move the Attendance & Call Average report to Production server its done in UAT.","comments":"The HCP visit count is displaying incorrect in call average report.->created by:lilu-2018\/7\/24","user_id":"629","file_type":""}]|

##### Submitting Ticket Details Webservice Reponse


###### ![#c5f015](https://placehold.it/15/c5f015/000000?text=+) Correct Response:- 

```json
{
    "message": {
        "success": "true",
        "data": {
            "result": [
                {
                    "message": "Inserted Successfully"
                }
            ]
        }
    }
}
```

###### ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Wrong Response:-  

```json
{
    "message": {
        "success": "false",
        "data": {
            "result": [
                {
                    "message": "Invalid Module Name"
                }
            ]
        }
    }
}
```

##### Submitting Ticket Details API relation table  
> No Table relation, fully online



## Royce

### General 

#### Download Pick List

> ##### `Download Pick List` SQLite Information  
>  Database  :- tuneem.db  
   Tablename :- picklist

##### `Download Pick List` Webservice Request

`POST Method`

|Parameters|Values|
|---|---|
|module|getPickList|


##### `Download Pick List` Webservice Reponse


###### ![#c5f015](https://placehold.it/15/c5f015/000000?text=+) Correct Response:-  
```json
{
    "message": {
        "success": "true",
        "data": {
            "result": [
                {
                    "id": 1,
                    "name": "Interested",
                    "status": "Active",
                    "pick_flag": "LSTG",
                    "convert_flag": "1"
                },
                {
                    "id": 2,
                    "name": "In Progress",
                    "status": "Active",
                    "pick_flag": "LSTG",
                    "convert_flag": "0"
                },
                {
                    "id": 3,
                    "name": "Not interested",
                    "status": "Active",
                    "pick_flag": "LSTG",
                    "convert_flag": "0"
                }
            ]
        }
    }
}
```

###### ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Wrong Response:-    
```json
{
    "message": {
        "success": "false",
        "data": {
            "result": [
                {
                    "message": "Invalid Module Name"
                }
            ]
        }
    }
}
```
##### `Download Pick List` API relation table
|SQLite column name|JSON variable name|Data type|Primary key|Remarks|
|---|---|---|---|---|
|pick_list_id|id|INTEGER|||
|pick_list_name|name|TEXT|No||
|pick_list_status|status|TEXT|No||
|pick_list_flag|pick_flag|TEXT|No||
|convert_flag|convert_flag|TEXT|No||


#### Download Location Master

> ##### `Download Location` SQLite Information  
>  Database  :- tuneem.db  
   Tablename :- locationmaster

##### `Download Location` Webservice Request

`POST Method`

|Parameters|Values|
|---|---|
|module|locationmaster|
|userid|629|

##### `Download Location` Webservice Reponse


###### ![#c5f015](https://placehold.it/15/c5f015/000000?text=+) Correct Response:-  

```json
{
    "message": {
        "success": "true",
        "data": {
            "result": [
                {
                    "postal_code": "600015",
                    "area": "Tnagar",
                    "city": "Chennai",
                    "status": "Active"
                },
                {
                    "postal_code": "400404",
                    "area": "Mumbai",
                    "city": "Mumbai",
                    "status": "Active"
                }
            ]
        }
    }
}
```


###### ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Wrong Response:-    
```json
{
    "message": {
        "success": "false",
        "data": {
            "result": [
                {
                    "message": "Invalid Module Name"
                }
            ]
        }
    }
}
```

##### `Download Location` API relation table
|SQLite column name|JSON variable name|Data type|Primary key|Remarks|
|---|---|---|---|---|
|location|area|TEXT|No||
|postal_code|postal_code|INTEGER|No||
|status|status|TEXT|No||
|city|city|TEXT|No||


#### Download Product Master

> ##### `Download Product` SQLite Information  
>  Database  :- tuneem.db  
   Tablename :- productmaster


##### Webservice Request

`POST Method`

|Parameters|Values|
|---|---|
|module|productmaster|
|userid|629|


##### Webservice Reponse

###### ![#c5f015](https://placehold.it/15/c5f015/000000?text=+) Correct Response:-  
```json
{
    "message": {
        "success": "true",
        "data": {
            "result": [
                {
                    "product_id": "4",
                    "product_name": "product temp",
                    "p_cat_id": "19",
                    "p_cat_name": "Electrodes",
                    "p_uom_id": "6",
                    "p_uom_name": "Box",
                    "p_size_id": "14",
                    "size": "10.0 MM",
                    "status": "InActive"
                },
                {
                    "product_id": "4",
                    "product_name": "product temp",
                    "p_cat_id": "19",
                    "p_cat_name": "Electrodes",
                    "p_uom_id": "8",
                    "p_uom_name": "Kgs",
                    "p_size_id": "14",
                    "size": "10.0 MM",
                    "status": "InActive"
                }
            ]
        }
    }
}
```


###### ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Wrong Response:-    
```json
{
    "message": {
        "success": "false",
        "data": {
            "result": [
                {
                    "message": "Invalid Module Name"
                }
            ]
        }
    }
}
```


#####  API relation table
|SQLite column name|JSON variable name|Data type|Primary key|Remarks|
|---|---|---|---|---|
|product_id|product_id|INTEGER|No||
|product_name|product_name|TEXT|No||
|p_cat_id|p_cat_id|INTEGER|No||
|p_cat_name|p_cat_name|TEXT|No||
|p_uom_id|p_uom_id|INTEGER|No||
|p_uom_name|p_uom_name|TEXT|No||
|p_size_id|p_size_id|INTEGER|No||
|size|size|TEXT|No||
|status|status|TEXT|No||


#### Joint Call

> ##### `Joint Call` SQLite Information  
> Database  :- tuneem.db  
  Tablename :- joint_call

##### `Joint Call` Webservice Request

`POST Method`

|Parameters|Values|
|---|---|
|module|joint_call|
|userid|629|



##### `Joint Call` Webservice Reponse


###### ![#c5f015](https://placehold.it/15/c5f015/000000?text=+) Correct Response:-  
```json
{
    "message": {
        "success": "true",
        "data": {
            "result": [
                {
                    "role": "Ticket Reviewer",
                    "user_id": "629"
                }
            ]
        }
    }
}
```

###### ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Wrong Response:-    
```json
{
    "message": {
        "success": "false",
        "data": {
            "result": [
                {
                    "message": "Invalid Module Name"
                }
            ]
        }
    }
}
```


##### `Joint Call` API relation table
|SQLite column name|JSON variable name|Data type|Primary key|Remarks|
|---|---|---|---|---|
|role|role|TEXT|No||
|user_id|user_id|INTEGER|No||


#### Visit Type 

> ##### `Visit Type` SQLite Information  
> Database  :- tuneem.db  
  Tablename :- visit_reason

##### `Visit Type` Webservice Request

`POST Method`

|Parameters|Values|
|---|---|
|module|visit_reason|
|userid|629|


##### `Visit Type` Webservice Reponse


###### ![#c5f015](https://placehold.it/15/c5f015/000000?text=+) Correct Response:-  

```json
{
    "message": {
        "success": "true",
        "data": {
            "result": [
                {
                    "id": "1",
                    "visit_reason": "Order Booking",
                    "status": "Active"
                },
                {
                    "id": "2",
                    "visit_reason": "Engagement",
                    "status": "Active"
                },
                {
                    "id": "3",
                    "visit_reason": "Followup",
                    "status": "Active"
                }
            ]
        }
    }
}
```

###### ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Wrong Response:-    
```json
{
    "message": {
        "success": "false",
        "data": {
            "result": [
                {
                    "message": "Invalid Module Name"
                }
            ]
        }
    }
}
```
##### `Visit Type` API relation table
|SQLite column name|JSON variable name|Data type|Primary key|Remarks|
|---|---|---|---|---|
|visit_res_id|id|INTEGER|No||
|visit_reason|visit_reason|TEXT|No||
|status|status|TEXT|No||


### Lead Opportunity   

#### Get Lead Opportunity   

> ##### SQLite Information  
> Database :- tuneem.db  
  Tablename :- lead_opp

##### `Get Lead Opportunity ` Webservice Request :

`POST Method`

|Parameters|Values|
|---|---|
|module|getLeadOpp|
|userid|629|


##### `Get Lead Opportunity ` Webservice Reponse :


###### ![#c5f015](https://placehold.it/15/c5f015/000000?text=+) Correct Response:-  

```json
{
    "message": {
        "success": "true",
        "data": {
            "result": [
                {
                    "tuneemLeadId": "320",
                    "customerName": "ssri",
                    "lead_flag": "2",
                    "lead_stage": "16",
                    "name": "Final",
                    "contactPerson": "sddf",
                    "mobile": "4780965231",
                    "area": "Adambakkam",
                    "cutomerDesignation": "",
                    "customer_type": "1",
                    "email": "as@m.n",
                    "industry": "",
                    "leadSource": "5",
                    "productId": "9",
                    "leadStage": "16",
                    "salesActivity": "7",
                    "industrytype": "6",
                    "nextInteractionDate": "0000-00-00 00:00:00",
                    "city": "Chennai",
                    "pincode": "600088",
                    "address": "sss",
                    "remark": "sss",
                    "createdDate": "2018-09-04 16:57:47",
                    "modifiedDate": "2018-09-04 16:57:47",
                    "callDate": "2018-09-04 16:57:47",
                    "createdBy": "629",
                    "modifiedBy": "629",
                    "assignedTo": "629",
                    "latitude": "37.421998333333335",
                    "longitude": "-122.08400000000002",
                    "status": "Active",
                    "filePath": "uploads/roycenull",
                    "filePath1": "uploads/roycenull",
                    "filePath2": "uploads/roycenull",
                    "sync_status": "0",
                    "lstgPickFlag": "CUSTOMER"
                },
                {
                    "tuneemLeadId": "323",
                    "customerName": "kiu",
                    "lead_flag": "2",
                    "lead_stage": "16",
                    "name": "Final",
                    "contactPerson": "ss",
                    "mobile": "8096547123",
                    "area": "Tnagar",
                    "cutomerDesignation": "",
                    "customer_type": "5",
                    "email": "as@s.m",
                    "industry": "",
                    "leadSource": "6",
                    "productId": "0",
                    "leadStage": "16",
                    "salesActivity": "4",
                    "industrytype": "5",
                    "nextInteractionDate": "0000-00-00 00:00:00",
                    "city": "Chennai",
                    "pincode": "600015",
                    "address": "ee",
                    "remark": "ddd",
                    "createdDate": "2018-09-04 17:12:11",
                    "modifiedDate": "2018-09-04 17:12:11",
                    "callDate": "0000-00-00 00:00:00",
                    "createdBy": "",
                    "modifiedBy": "",
                    "assignedTo": "629",
                    "latitude": "37.421998333333335",
                    "longitude": "-122.08400000000002",
                    "status": "Active",
                    "filePath": "uploads/roycenull",
                    "filePath1": "uploads/roycenull",
                    "filePath2": "uploads/roycenull",
                    "sync_status": "0",
                    "lstgPickFlag": "CUSTOMER"
                }             
            ]
        }
    }
}
```

###### ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Wrong Response:-  

```json
{
    "message": {
        "success": "false",
        "data": {
            "result": [
                {
                    "message": "Invalid Module Name"
                }
            ]
        }
    }
}
```


##### `Get Lead Opportunity` API relation table :-
|SQLite column name|JSON variable name|Data type|Primary key|Remarks|
|---|---|---|---|---|
|tuneemLeadId|tuneemLeadId|TEXT|NO||
|customername|customerName|TEXT|NO||
|contactperson|contactPerson|TEXT|NO||
|mobile|mobile|TEXT|NO||
|area|area|TEXT|NO||
|cutomerdesignation|cutomerDesignation|TEXT|NO||
|customer_type|customer_type|TEXT|NO||
|email|email|TEXT|NO||
|industry|industry|TEXT|NO||
|leadsource|leadSource|TEXT|NO||
|productid|productId|TEXT|NO||
|leadstage|leadStage|TEXT|NO||
|salesactivity|salesActivity|TEXT|NO||
|industrytype|industrytype|TEXT|NO||
|nextinteractiondate|nextInteractionDate|TEXT|NO||
|city|city|TEXT|NO||
|pincode|pincode|TEXT|NO||
|address|address|TEXT|NO||
|remark|remark|TEXT|NO||
|createddate|createdDate|TEXT|NO||
|modifieddate|modifiedDate|TEXT|NO||
|calldate|callDate|TEXT|NO||
|createdby|createdBy|TEXT|NO||
|modifiedby|modifiedBy|TEXT|NO||
|assignedto|assignedTo|TEXT|NO||
|latitude|latitude|TEXT|NO||
|longitude|longitude|TEXT|NO||
|status|status|TEXT|NO||
|filepath|filePath|TEXT|NO||
|filepath1|filePath1|TEXT|NO||
|filepath2|filePath2|TEXT|NO||
|syncstatus|syncStatus|TEXT|NO||
|lstgpickflag|lstgPickFlag|TEXT|NO||
|lead_flag|lead_flag|TEXT|NO||
|name|name|TEXT|NO||


#### Upload Lead Opportunity   

> ##### SQLite Information  
> Database :- tuneem.db  
  Tablename :- lead_opp

##### `Upload Lead Opportunity` Webservice Request :

`POST Method`

|Parameters|Values|
|---|---|
|module|putLeadOpp|
|data|{"mob_p_id":"31","customer_name":"Linnel Messi","contact_person":"Messi","mobile":"7531598524","area":"Mumbai","customer_type":"3","email":"lionelmessi@rsalesarm.com","lead_source":"5","product_id":"5","lead_stage":"1","sales_activity":"4","industry_type":"0","next_interaction_date":"2018\/09\/18 ","city":"Mumbai","pincode":"400404","address":"Mahaballaipuram","remark":"Excellent work dude","status":"Active","latitude":"37.421998333333335","longitude":"-122.08400000000002","user_id":"629","filepath":"uploads\/roycenull","filepath1":"uploads\/roycenull","filepath2":"uploads\/roycenull","sync_status":"1"}|


##### `Upload Lead Opportunity` Webservice Reponse :


###### ![#c5f015](https://placehold.it/15/c5f015/000000?text=+) Correct Response:-  
```json
{
    "message": {
        "success": "true",
        "data": {
            "result": [
                {
                    "mob_p_id": "",
                    "tuneem_lead_id": "364",
                    "status": "Inserted"
                }
            ]
        }
    }
}
```

###### ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Wrong Response:-    
```json
{
    "message": {
        "success": "false",
        "data": {
            "result": [
                {
                    "message": "Invalid Module Name"
                }
            ]
        }
    }
}
```

##### `Upload Lead Opportunity` API relation table :-

|SQLite column name|JSON variable name|Data type|Primary key|Remarks|
|---|---|---|---|---|
|ID|mob_p_id|Integer|Yes||
|tuneemLeadId|tuneem_lead_id|TEXT|NO||
|customername|customer_name|TEXT|NO||
|contactperson|contact_person|TEXT|NO||
|mobile|mobile|TEXT|NO||
|area|area|TEXT|NO||
|cutomerdesignation|designation|TEXT|NO||
|customer_type|customer_type|TEXT|NO||
|email|email|TEXT|NO||
|industry|industry|TEXT|NO||
|leadsource|lead_source|TEXT|NO||
|productid|product_id|TEXT|NO||
|leadstage|lead_stage|TEXT|NO||
|salesactivity|sales_activity|TEXT|NO||
|industrytype|industry_type|TEXT|NO||
|nextinteractiondate|next_interaction_date|TEXT|NO||
|city|city|TEXT|NO||
|pincode|pincode|TEXT|NO||
|address|address|TEXT|NO||
|remark|remark|TEXT|NO||
|status|status|TEXT|NO||
|latitude|latitude|TEXT|NO||
|longitude|longitude|TEXT|NO||
|assignedto|user_id|TEXT|NO||
|filepath|filepath|TEXT|NO||
|filepath1|filepath1|TEXT|NO||
|filepath2|filepath2|TEXT|NO||
|syncstatus|sync_status|TEXT|NO||

### Customer List

> ##### `Customer List` SQLite Information  
> database  :- tuneem.db  
  tablename :- customermaster

##### `Customer List` Webservice Request

`POST Method`

|Parameters|Values|
|---|---|
|module|customermaster|
|userid|669|

##### `Customer List` Webservice Reponse


###### ![#c5f015](https://placehold.it/15/c5f015/000000?text=+) Correct Response:-  
```json
{
    "message": {
        "success": "true",
        "data": {
            "result": [
                {
                    "cat_id": "4",
                    "category": "Royce",
                    "cm_id": "10",
                    "customer_name": "mukundhan",
                    "customer_mobile": "1144477775",
                    "industry_id": "0",
                    "industry_name": null,
                    "postal_code": "9",
                    "customer_addr_id": "10",
                    "address_line1": "",
                    "city": "Rewa",
                    "state": "MadhyaPradesh",
                    "region": "Central",
                    "country": "India",
                    "status": "Active",
                    "con_per_name": "muki",
                    "con_per_mobile": ""
                },
                {
                    "cat_id": "4",
                    "category": "Royce",
                    "cm_id": "11",
                    "customer_name": "quikly",
                    "customer_mobile": "9811199946",
                    "industry_id": "0",
                    "industry_name": null,
                    "postal_code": "8",
                    "customer_addr_id": "11",
                    "address_line1": "",
                    "city": "Satna",
                    "state": "MadhyaPradesh",
                    "region": "Central",
                    "country": "India",
                    "status": "Active",
                    "con_per_name": "quiclky",
                    "con_per_mobile": ""
                }
            ]
        }
    }
}
```
###### ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Wrong Response:-   

```json 
{
    "message": {
        "success": "false",
        "data": {
            "result": [
                {
                    "message": "Invalid Module Name"
                }
            ]
        }
    }
}
```

##### `Customer List` API relation table
|SQLite column name|JSON variable name|Data type|Primary key|Remarks|
|---|---|---|---|---|
|user_id|Nil|TEXT|No||
|cat_id|cat_id|INTEGER|No||
|category|category|TEXT|No||
|customer_id|cat_id|INTEGER|No||
|customer_name|customer_name|TEXT|No||
|customer_mobile|customer_mobile|TEXT|No||
|cp_name|con_per_name|TEXT|No||
|cp_mobile|con_per_mobile|TEXT|No||
|industry_id|industry_id|INTEGER|No||
|industry_name|industry_name|TEXT|No||
|postal_code|postal_code|INTEGER|No||
|status|status|TEXT|No||
|customer_addr_id|customer_addr_id|TEXT|No||
|address|address_line1|TEXT|No||
|city|city|TEXT|No||
|state|state|TEXT|No||
|region|region|TEXT|No||
|country|country|TEXT|No||


### Customer Visit

> + Download customer visit is not written  
> + Point to two different webservices  
> + Customer department is dropped and customer department product depends upon Department primary id.  
> + So documentation is Kept on hold as of now.  

### Expense Statement 

> ##### `Expense Statement` SQLite Information  
> Fully online, so no Table

##### `Expense Statement` Webservice Request

`POST Method`

|Parameters|Values|
|---|---|
|module|putExpense|
|data|[{"user_id":"629","expense_statement_name":"computer expense","expense_others":"motherboard purchase","expense_amount":"50000","remarks":"set of ram was bought","expense_type":"6","latitude":"13.0396144","longitude":"80.2429993","file_path":"uploads\/royce\/IMG_20180919_125354.jpg"}]|


##### `Expense Statement` Webservice Reponse


###### ![#c5f015](https://placehold.it/15/c5f015/000000?text=+) Correct Response:-  
```json
{
    "message": {
        "success": "true",
        "data": {
            "result": [
                {
                    "message": "Inserted Successfully"
                }
            ]
        }
    }
}
```
###### ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Wrong Response:-    

```json
{
    "message": {
        "success": "false",
        "data": {
            "result": [
                {
                    "message": "Invalid Module Name"
                }
            ]
        }
    }
}
```


##### `Expense Statement` API relation table  
> No Table relation, fully online  


### Demo

> ##### `Demo` SQLite Information  
> Fully online, so no Table

##### `Demo` Webservice Request

`POST Method`

|Parameters|Values|
|---|---|
|module|getProductDemo|
|userid|629|

##### `Demo` Webservice Reponse


###### ![#c5f015](https://placehold.it/15/c5f015/000000?text=+) Correct Response:-  

```json
{
    "message": {
        "success": "true",
        "data": {
            "result": [
                {
                    "title": "jesus",
                    "description": "jesus",
                    "filename": "13Screenshot from 2018-03-09 12-59-14.png",
                    "filepath": "uploads/13Screenshot from 2018-03-09 12-59-14.png",
                    "status": "Active"
                },
                {
                    "title": "Tuneem",
                    "description": "Tuneem",
                    "filename": "11Rechargeuniversalcharger.mp4",
                    "filepath": "uploads/11Rechargeuniversalcharger.mp4",
                    "status": "Active"
                }
            ]
        }
    }
}
```


###### ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Wrong Response:-    
```json
{
    "message": {
        "success": "false",
        "data": {
            "result": [
                {
                    "message": "Invalid Module Name"
                }
            ]
        }
    }
}
```


##### `Demo` API relation table
> No Table relation, fully online  


### Collection and Deposit

#### Download Collection and Deposit

> ##### SQLite Information  
> Database  :- tuneem.db  
  Tablename :- collection_deposit  

##### Webservice Request

`POST Method`

|Parameters|Values|
|---|---|
|module|getCollectionDeposit|
|userid|629|



##### Webservice Reponse


###### ![#c5f015](https://placehold.it/15/c5f015/000000?text=+) Correct Response:-  

###### ![#f03c15](https://placehold.it/15/f03c15/000000?text=+) Wrong Response:-    

#####  API relation table
|SQLite column name|JSON variable name|Data type|Primary key|Remarks|
|---|---|---|---|---|
||||||


