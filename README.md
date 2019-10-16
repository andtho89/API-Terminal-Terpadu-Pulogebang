# DOC API TERMINAL PULOGEBANG

------------

**URL :  https://api.terminalpulogebang.com**

**SECURITY : BASIC, API KEY**


------------

##### API LIST
|  API | URL  | SECURITY | GET | POST  | PUT   | DELETE |
| ------------ | ------------ | ------------ | ------------ | ------------ | ------------ |------------ |
|  /authentication |BASIC | :fa-check:   |:fa-times:   |:fa-times:  |:fa-times:    |:fa-times:  |
|  /boarding |KEY | :fa-check:   |:fa-check:   |:fa-check:   |:fa-check:   |:fa-check:  |
|  /tujuan |KEY | :fa-check:   |:fa-times:   |:fa-times:   |:fa-times:    |:fa-times:  |
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
| boarding_id  | :fa-times:  | Get boarding by id boarding  |
| ticket_id  | :fa-times:  | Get boarding by id ticket  |
| date_of_departure  | :fa-times:  | Get boarding by date of departure  |
|   |   |   | |

------------


- **POST**
*URL : **/boarding*** 

*Security : **KEY***

*Description* :  POST new boarding

**Parameter**

| Parameter  | Required  |Notes   |
| ------------ | ------------ | ------------ |
| ticket_id  |:fa-check:   |  id ticket  |
| destination_id  | :fa-check:   | destination id get from **api /tujuan** |
| date_of_departure  | :fa-check:   |  date of departure  |
| time_of_departure  | :fa-check:   | time of departure  |
|   |   |   | |

------------
- **PUT**
*URL : **/boarding*** 

*Security : **KEY***

*Description* : Edit boarding

**Parameter**

| Parameter  | Required  |Notes   |
| ------------ | ------------ | ------------ |
| ticket_id  |:fa-check:   |  id ticket  |
| destination_id  |  :fa-times:   | destination id get from **api /tujuan** |
| date_of_departure  |  :fa-times:    |  date of departure  |
| time_of_departure  | :fa-times:   | time of departure  |
|   |   |   | |

- **DELETE**
*URL : **/boarding*** 

*Security : **KEY***

*Description* :  remove boarding 

**Parameter**

| Parameter  | Required  |Notes   |
| ------------ | ------------ | ------------ |
| ticket_id  |:fa-check:   |  id ticket  |
|   |   |   | |


------------

##### /tujuan

*URL : **/authentication*** 

*Method: **GET***

*Security : **Basic***

*Description* : GET API KEY Production, Api Key Development

**Parameter**

| Parameter  | Required  |Notes   |
| ------------ | ------------ | ------------ |
| id  |:fa-times:  | get tujuan by id  |
| province  |:fa-times:  | get tujuan by province  |
| city  |:fa-times:  | get tujuan by city  |
| region  |:fa-times:  | get tujuan by region  |
|   |   |   | |
------------
