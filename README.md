# HW_1

# Создать запросы в Postman.

 _Protocol: http_
 
 _IP: 162.55.220.72_
 
 _Port: 5007_


__в поле ввода `URL` ввожу http://162.55.220.72:5007/ и нажимаю Save__


 # Method: GET
 
 # EP_1
 
 
 _EndPoint: /get_method_
 
 _request url params:_ 
 
 _name: str_
 
 _age: int_


1. Создаю новый request `команда "Add Request"`
2. Выбираю `method get`
3. Дописываю  в поле ввода `URL`  "/get_method"
4. Перехожу в режим `"Params"`
5. В строках " KEY and Value " ввожу нужные значения 
6. Нажимаю `SEND`

_response:_ 

[

    "Ilya",
    "23"
    
]
 
# Method: POST

# EP_2

_EndPoint: /user_info_3_

_request form data:_

_name: str_

_age: int_

_salary: int_


1. Создаю новый request `команда "Add Request"`
2. Выбираю метод `Postt`
3. Дописываю  в поле ввода `URL`  "user_info_3"
4. Перехожу во вкладку `"Body"` далее `"Form-date"`
5. В строках " KEY, Value, Salary " ввожу нужные значения 
6. Нажимаю `SEND`

# Method: GET 

# EP_3

_EndPoint: /object_info_1_

_request url params:_ 

_name: str_

_age: int_

_weight: int_


1. Создаю новый request `команда "Add Request"`
2. Выбираю метод `Postt`
3. Дописываю  в поле ввода `URL`  "object_info_1"
4. Перехожу в режим `"Params"`
5. В строках " KEY, Value, Weigt " ввожу нужные значения 
6. Нажимаю `SEND`

_response:_


