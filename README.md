# HW_1

# Создать запросы в Postman.

Protocol: http

IP: 162.55.220.72

Port: 5007


в поле ввода `URL` ввожу http://162.55.220.72:5007/ и нажимаю Save

 # EP_1
 
 Method: GET
 
 EndPoint: /get_method
 
 request url params: 
 
 name: str
 
 age: int


1. Создаю новый request `команда "Add Request"`
2. Выбираю `method get`
3. Дописываю  в поле ввода `URL`  "/get_method"
4. Перехожу в режим `"Params"`
5. В строках " KEY and Value " ввожу нужные значения 
6. Нажимаю `SEND`

response:: 

[

    "Ilya",
    "23"
    
]
 
# Method: POST

# EP_2

EndPoint: /user_info_3
request form data:
name: str
age: int
salary: int

1. Создаю новый request `команда "Add Request"`
2. Выбираю метод `Postt`
3. Дописываю  в поле ввода `URL`  "user_info_3"
4. Перехожу во вкладку `"Body"` далее `"Form-date"`
5. В строках " KEY, Value, Salary " ввожу нужные значения 
6. Нажимаю `SEND`

# Method: GET 

# EP_3

EndPoint: /object_info_1
request url params: 
name: str
age: int
weight: int

1. Создаю новый request `команда "Add Request"`
2. Выбираю метод `Postt`
3. Дописываю  в поле ввода `URL`  "object_info_1"
4. Перехожу в режим `"Params"`
5. В строках " KEY, Value, Weigt " ввожу нужные значения 
6. Нажимаю `SEND`

response:
ответ

