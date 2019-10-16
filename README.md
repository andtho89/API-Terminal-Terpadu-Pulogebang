# DOC API TERMINAL PULOGEBANG
https://documenter.getpostman.com/view/3787169/SVtYT7Xv
------------

**URL :  https://api.terminalpulogebang.com**

**SECURITY : BASIC, API KEY**


------------

##### API LIST
|  API | URL  | SECURITY | GET | POST  | PUT   | DELETE |
| ------------ | ------------ | ------------ | ------------ | ------------ | ------------ |------------ |
|  /authentication |BASIC | :heavy_check_mark:  |:x:  |:x: |:x:   |:x: |
|  /boarding |KEY | :heavy_check_mark:  |:heavy_check_mark:   |:heavy_check_mark:   |:heavy_check_mark:   |:heavy_check_mark:  |
|  /tujuan |KEY | :heavy_check_mark:   |:x:  |:x:  |:x:   |:x: |
|  /po |KEY | :heavy_check_mark:   |:x:  |:x:  |:x:   |:x: |
|   |   |   |   |   | | ||

------------

**api-key get from api /authentication with basic authentication**

** to get a username and password please contact Terminal Terpadu Pulogebang**

------------

##### /AUTHENTICATION
*URL : **/authentication***

*Method: **GET***

*Security : **Basic***

*Description* : GET API KEY Production, Api Key Development

------------



##### /BOARDING {GET, POST, PUT, DELETE}
- **GET**
*URL : **/boarding*** 

*Security : **KEY***

*Description* : Get boarding list user

**Parameter**

| Parameter  | Required  |Notes   |
| ------------ | ------------ | ------------ |
| boarding_id  | :x: | Get boarding by id boarding  |
| po_id  |:x:   |  id PO get from **API /po**  |
| ticket_id  | :x: | Get boarding by id ticket  |
| date_of_departure  | :x: | Get boarding by date of departure  |
|   |   |   | |

------------


- **POST**
*URL : **/boarding*** 

*Security : **KEY***

*Description* :  POST new boarding

**Parameter**

| Parameter  | Required  |Notes   |
| ------------ | ------------ | ------------ |
| ticket_id  |:heavy_check_mark:   |  id ticket  |
| po_id  |:heavy_check_mark:  |  id PO get from **API /po**  |
| destination_id  | :heavy_check_mark:   | destination id get from **api /tujuan** |
| date_of_departure  | :heavy_check_mark:   |  date of departure  |
| time_of_departure  | :heavy_check_mark:   | time of departure  |
|   |   |   | |

------------
- **PUT**
*URL : **/boarding*** 

*Security : **KEY***

*Description* : Edit boarding

**Parameter**

| Parameter  | Required  |Notes   |
| ------------ | ------------ | ------------ |
| ticket_id  |:heavy_check_mark:   |  id ticket  |
| po_id  |:x:   |  id PO get from **API /po**  |
| destination_id  |  :x:  | destination id get from **api /tujuan** |
| date_of_departure  |  :x:   |  date of departure  |
| time_of_departure  | :x:  | time of departure  |
|   |   |   | |

- **DELETE**

*URL : **/boarding*** 

*Security : **KEY***

*Description* :  remove boarding 

**Parameter**

| Parameter  | Required  |Notes   |
| ------------ | ------------ | ------------ |
| ticket_id  |:heavy_check_mark:   |  id ticket  |
|   |   |   | |


------------

##### /tujuan

*URL : **/tujuan*** 

*Method: **GET***

*Security : **KEY***

*Description* : GET list tujuan

**Parameter**

| Parameter  | Required  |Notes   |
| ------------ | ------------ | ------------ |
| id  |:x: | get tujuan by id  |
| province  |:x: | get tujuan by province  |
| city  |:x: | get tujuan by city  |
| region  |:x: | get tujuan by region  |
|   |   |   | |
------------

##### /po

*URL : **/po*** 

*Method: **GET***

*Security : **KEY***

*Description* : Get list po


**Parameter**

| Parameter  | Required  |Notes   |
| ------------ | ------------ | ------------ |
| id  |:x: | get po by id  |
| name  |:x: | get po by name  |
|   |   |   | |
------------

