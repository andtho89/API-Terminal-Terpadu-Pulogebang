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
|   |   |   |   |   | | ||

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

*Security : **Basic***

*Description* : GET API KEY Production, Api Key Development

**Parameter**

| Parameter  | Required  |Notes   |
| ------------ | ------------ | ------------ |
| id  |:x: | get tujuan by id  |
| province  |:x: | get tujuan by province  |
| city  |:x: | get tujuan by city  |
| region  |:x: | get tujuan by region  |
|   |   |   | |
------------
