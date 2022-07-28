# Postman

## HW_1
Создать запросы в Postman.

Protocol: http  
IP: 162.55.220.72  
Port: 5005  

*в поле "Enter request URL" вписать http://162.55.220.72:5005*

----------
**EP_1**  
Method: GET    
EndPoint: /get_method    
request url params:  
 name: str  
 age: int  
  

*Переименовать "New Request" в "EP_1" ->*  
*Выбрать метод GET ->*  
*В поле "Enter request URL" добавить EndPoint "/get_method", чтобы получилось http://162.55.220.72:5005/get_method ->*  
*Во вкладке Params заполнить компоненты ключ:значение "name":"Svetlana" и "age":"39" ->*  
*Save -> Send*  

*response:*
```
[
    "Svetlana",
    "39"
]
```
-----

**EP_2**  
Method: POST  
EndPoint: /user_info_3  
request form data:  
 name: str  
 age: int  
 salary: int  


*Скопировать предыдущий запрос (Duplicate) ->*  
*Переименовать "EP_1 Copy" в "EP_2" ->*. 
*Выбрать метод POST ->*  
*В поле "Enter request URL" заменить EndPoint "/get_method" на "/user_info_3", чтобы получилось http://162.55.220.72:5005/user_info_3 ->*  
*Во вкладке Body заполнить из выподающего списка выбрать form-data. Заполнить компоненты ключ:значение "name":"Svetlana"; "age":"39"; "salary":"50000" ->*  
*Save -> Send*  

*response:*  
```
{
    "age": "39",
    "family": {
        "children": [
            [
                "Alex",
                24
            ],
            [
                "Kate",
                12
            ]
        ],
        "u_salary_1_5_year": 200000
    },
    "name": "Svetlana",
    "salary": 50000
}
```
-----

**EP_3**  
Method: GET  
EndPoint: /object_info_1  
request url params:  
 name: str  
 age: int  
 weight: int   


*Скопировать предыдущий запрос (Duplicate) ->*  
*Переименовать "EP_2 Copy" в "EP_3" ->*. 
*Выбрать метод GET ->*  
*В поле "Enter request URL" заменить EndPoint "/user_info_3" на "/object_info_1", чтобы получилось http://162.55.220.72:5005/object_info_1 ->*  
*Во вкладке Params заполнить компоненты ключ:значение "name":"Svetlana"; "age":"39"; "weight":"52" ->*  
*Save -> Send*  

*response:*  
```
{
    "age": 39,
    "daily_food": 0.624,
    "daily_sleep": 130.0,
    "name": "Svetlana"
}
```
-----

**EP_4**  
Method: GET  
EndPoint: /object_info_2  
request url params:  
 name: str  
 age: int  
 salary: int  


*Скопировать предыдущий запрос (Duplicate) ->*  
*Переименовать "EP_3 Copy" в "EP_4" ->*. 
*Выбрать метод GET ->*  
*В поле "Enter request URL" заменить EndPoint "/object_info_1" на "/object_info_2", чтобы получилось http://162.55.220.72:5005/object_info_2 ->*  
*Во вкладке Params заполнить компоненты ключ:значение "name":"Svetlana"; "age":"39"; "salary":"50000" ->*  
*Save -> Send*  

*response:*  
```
{
    "person": {
        "u_age": 39,
        "u_name": [
            "Svetlana",
            50000,
            39
        ],
        "u_salary_5_years": 210000.0
    },
    "qa_salary_after_1.5_year": 165000.0,
    "qa_salary_after_12_months": 135000.0,
    "qa_salary_after_3.5_years": 190000.0,
    "qa_salary_after_6_months": 100000,
    "start_qa_salary": 50000
}
```
-----

**EP_5**  
Method: GET  
EndPoint: /object_info_3  
request url params:  
 name: str  
 age: int  
 salary: int   


*Скопировать предыдущий запрос (Duplicate) ->*  
*Переименовать "EP_4 Copy" в "EP_5" ->*. 
*Выбрать метод GET ->*  
*В поле "Enter request URL" заменить EndPoint "/object_info_2" на "/object_info_3", чтобы получилось http://162.55.220.72:5005/object_info_3 ->*  
*Во вкладке Params заполнить компоненты ключ:значение "name":"Svetlana"; "age":"39"; "salary":"50000" ->*  
*Save -> Send*  

*response:*  
```
{
    "age": "39",
    "family": {
        "children": [
            [
                "Alex",
                24
            ],
            [
                "Kate",
                12
            ]
        ],
        "pets": {
            "cat": {
                "age": 3,
                "name": "Sunny"
            },
            "dog": {
                "age": 4,
                "name": "Luky"
            }
        },
        "u_salary_1_5_year": 200000
    },
    "name": "Svetlana",
    "salary": 50000
}
```
-----

**EP_6**  
Method: GET  
EndPoint: /object_info_4  
request url params:  
 name: str  
 age: int  
 salary: int   


*Скопировать предыдущий запрос (Duplicate) ->*  
*Переименовать "EP_5 Copy" в "EP_6" ->*. 
*Выбрать метод GET ->*  
*В поле "Enter request URL" заменить EndPoint "/object_info_3" на "/object_info_4", чтобы получилось http://162.55.220.72:5005/object_info_4 ->*  
*Во вкладке Params заполнить компоненты ключ:значение "name":"Svetlana"; "age":"39"; "salary":"50000" ->*  
*Save -> Send*  

*response:*  
```
{
    "age": 39,
    "name": "Svetlana",
    "salary": [
        50000,
        "100000",
        "150000"
    ]
}
```
-----

**EP_7**  
Method: POST  
EndPoint: /user_info_2  
request form data:  
 name: str  
 age: int  
 salary: int     


*Скопировать предыдущий запрос (Duplicate) ->*  
*Переименовать "EP_6 Copy" в "EP_7" ->*. 
*Выбрать метод POST ->*  
*В поле "Enter request URL" заменить EndPoint "/object_info_4" на "/user_info_2", чтобы получилось http://162.55.220.72:5005/user_info_2 ->*  
*Во вкладке Body из выподающего списка выбрать form-data. Заполнить компоненты ключ:значение "name":"Svetlana"; "age":"39"; "salary":"50000" ->*  
*Save -> Send*  

*response:*  
```
{
    "person": {
        "u_age": 39,
        "u_name": [
            "Svetlana",
            50000,
            39
        ],
        "u_salary_5_years": 210000.0
    },
    "qa_salary_after_1.5_year": 165000.0,
    "qa_salary_after_12_months": 135000.0,
    "qa_salary_after_3.5_years": 190000.0,
    "qa_salary_after_6_months": 100000,
    "start_qa_salary": 50000
}
```
-----




