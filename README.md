# HW_1"  
💁‍♂️

# Создать запросы в Рostmаn

 _Protocol: http_
 
 _IP: 162.55.220.72_
 
 _Port: 5007_


__в поле ввода `URL` ввожу http://162.55.220.72:5007/ и нажимаю Save__

------------------------------------------------------------------------------------------------------------------------
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

---------------------------------------------------------------------------------------------------------------
# Method: POST

# EP_2

_EndPoint: /user_info_3_

_request form data:_

_name: str_

_age: int_

_salary: int_


1. Создаю новый request `команда "Add Request"`
2. Выбираю метод `Post`
3. Дописываю  в поле ввода `URL`  "user_info_3"
4. Перехожу во вкладку `"Body"` далее `"Form-date"`
5. В строках " KEY, Value, Salary " ввожу нужные значения 
6. Нажимаю `SEND`

_response:_

{

    "age": "23",
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
        "u_salary_1_5_year": 80000
    },
    "name": "Ilya",
    "salary": 20000
    
}

---------------------------------------------------------------------------------------------------------------
# Method: GET 

# EP_3

_EndPoint: /object_info_1_

_request url params:_ 

_name: str_

_age: int_

_weight: int_


1. Создаю новый request `команда "Add Request"`
2. Выбираю метод `Get`
3. Дописываю  в поле ввода `URL`  "object_info_1"
4. Перехожу в режим `"Params"`
5. В строках " KEY, Value, Weigt " ввожу нужные значения 
6. Нажимаю `SEND`

_response:_

{

    "age": 23,
    "daily_food": 0.84,
    "daily_sleep": 175.0,
    "name": "Ilya"
    
}

---------------------------------------------------------------------------------------------------------------

# Method: GET

# EP_4

_EndPoint: /object_info_2_

_request url params:_ 

_name: str_

_age: int_

_salary: int_


1. Создаю новый request `команда "Add Request"`
2. Выбираю метод `Get`
3. Дописываю  в поле ввода `URL`  "object_info_2"
4. Перехожу в режим `"Params"`
5. В строках " KEY, Value, Salary " ввожу нужные значения 
6. Нажимаю `SEND`

_response:_

{
   
   "person": {
   
        "u_age": 23,
        "u_name": [
            "Ilya",
            100,
            23
        ],
        "u_salary_5_years": 420.0
    },
    "qa_salary_after_1.5_year": 330.0,
    "qa_salary_after_12_months": 270.0,
    "qa_salary_after_3.5_years": 380.0,
    "qa_salary_after_6_months": 200,
    "start_qa_salary": 100
    
   
}

---------------------------------------------------------------------------------------------------------------

# Method: GET

# EP_5

_EndPoint: /object_info_3_

_request url params:_ 

 _name: str_
 
 _age: int_
 
 _salary: int_

1. Создаю новый request `команда "Add Request"`
2. Выбираю метод `Get`
3. Дописываю  в поле ввода `URL`  "object_info_3"
4. Перехожу в режим `"Params"`
5. В строках " KEY, Value, Salary " ввожу нужные значения 
6. Нажимаю `SEND`

_response:_

{
   
   "age": "23",
   
   "family": 
   
    {"children": [["Alex", 24], ["Kate", 12]],
    
               "pets": {"cat": {"age": 3, "name": "Sunny"},
               
                        "dog": {"age": 4, "name": "Luky"}},
                        
               "u_salary_1_5_year": 40000},"name": "Ilya", "salary": 10000
               
}

---------------------------------------------------------------------------------------------------------------

# Method: GET

# EP_6

_EndPoint: /object_info_4_

_request url params:_ 

 _name: str_
 
 _age: int_
 
 _salary: int_
 
1. Создаю новый request `команда "Add Request"`
2. Выбираю метод `Get`
3. Дописываю  в поле ввода `URL`  "object_info_4"
4. Перехожу в режим `"Params"`
5. В строках " KEY, Value, Salary " ввожу нужные значения 
6. Нажимаю `SEND`

_response:_

{
    
    "age": 23,
    "name": "Ilya",
    "salary": [
        100,
        "200",
        "300"
        
    ]
}

---------------------------------------------------------------------------------------------------------------

# Method: POST

# EP_7

_EndPoint: /user_info_2_

_request form data:_ 

 _name: str_
 
 _age: int_
 
 _salary: int_


1. Создаю новый request `команда "Add Request"`
2. Выбираю метод `Post`
3. Дописываю  в поле ввода `URL`  "user_info_2"
4. Перехожу во вкладку `"Body"` далее `"Form-date"`
5. В строках " KEY, Value, Salary " ввожу нужные значения 
6. Нажимаю `SEND`

_response:_


{
   
   "person": {
       
       "u_age": 23,
        "u_name": [
            "Ilya",
            20000,
            23
       
       ],
        "u_salary_5_years": 84000.0
    },
    "qa_salary_after_1.5_year": 66000.0,
    "qa_salary_after_12_months": 54000.0,
    "qa_salary_after_3.5_years": 76000.0,
    "qa_salary_after_6_months": 40000,
    "start_qa_salary": 20000
    
}
