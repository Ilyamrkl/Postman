# HW_2 Postman


http://162.55.220.72:5005/first
 1. Отправить запрос
 
_ввожу в поле ввода `"URL"`  `http://162.55.220.72:5005/first` , далее кнопка `Send`_

__response:__

    This is the first responce from server!ss

2. Статус код 200

_перехожу `Tests ➡️  Status Code is 200 ➡️  Sand  ➡️  Test Results`_

__response:__

    Status code is 200

3. Проверить, что в body приходит правильный string.

__response:__

    This is the first responce from server!ss
____________________________________________________________________________________________________________________________________________

http://162.55.220.72:5005/user_info_3

1. Отправить запрос.

_ввожу в поле ввода `"URL"`  `http://162.55.220.72:5005/user_info_3` , далее кнопка `Send`_


2. Статус код 200

_перехожу `Tests ➡️  Status Code is 200 ➡️  Sand  ➡️  Test Results`_

__response:__

    Status code is 200

3. Спарсить response body в json.

_перехожу в  `Snippets ➡️  Response body: JSON value check`_

  `оставляю код:`
  
    let responseData = pm.response.json(); 
    pm.test("Your test name", function () {
    console.log(responseData);
    

4. Проверить, что name в ответе равно name s request (name вбить руками.)

 `оставляю код:`

    pm.test("name в запросе равен name в ответе", function () {
    pm.expect(responseData.name).to.eql("Ilya");
    
    
  __response:__
 
    PASS name в запросе равен name в ответе

5. Проверить, что age в ответе равно age s request (age вбить руками.)

`оставляю код:`

    pm.test("age в запросе равен age в ответе", function () {
    pm.expect(responseData.age).to.eql("23");
    
 __response:__
    
    PASS age в запросе равен age в ответе 


6. Проверить, что salary в ответе равно salary s request (salary вбить руками.)
 
`оставляю код:`

    pm.test("salary в запросе равен salary в ответе", function () {
    pm.expect(responseData.salary).to.eql(20000);});
    
__response:__

    PASS salary в запросе равен salary в ответе
    
7. Спарсить request.

`оставляю код:`

     let requestData = request.data;  
     console.log('request data:', requestData);
     
 __response:__
   
`Console:`  
      
     request data:{age: "23", name: "Ilya", salary: "20000"}
     
8. Проверить, что name в ответе равно name s request (name забрать из request.)

`оставляю код:`

      pm.test("значения name в ответе и в запросе совпадают", function () {
      pm.expect(responseData.name).to.eql(requestData.name);});
      
 __response:__  
 
     PASSзначения name в ответе и в запросе совпадают
     
9. Проверить, что age в ответе равно age s request (age забрать из request.)

`оставляю код:`

     pm.test("значения age в ответе и в запросе совпадают", function () {
     pm.expect(responseData.age).to.eql(requestData.age);  
     });

 __response:__  
 
    PASS значения age в ответе и в запросе совпадают
    
10. Проверить, что salary в ответе равно salary s request (salary забрать из request.)

`оставляю код:`

     pm.test("значения salary в ответе и в запросе совпадают", function () {
     pm.expect(responseData.salary).to.eql(Number(requestData.salary));  
     });

 __response:__
 
   PASS значения salary в ответе и в запросе совпадают

11. Вывести в консоль параметр family из response.

`Console:`  

    console.log('Family: ', responseDate.family)
    
 __response:__
 
  `Console:`  
  
12. Проверить что u_salary_1_5_year в ответе равно salary*4 (salary забрать из request)

`оставляю код:`

     pm.test("u_salary_1_5_year в ответе равно salary*4", function () {  
     pm.expect(responseData.family.u_salary_1_5_year).to.eql(+requestData.salary*4);   
     });
     
 __response:__  
 
       PASS u_salary_1_5_year в ответе равно salary*4
       
       
# http://162.55.220.72:5005/object_info_3

1. Отправить запрос.

ввожу в поле ввода `"URL"`  `http://162.55.220.72:5005/user_info_3` , далее кнопка `Send`_

2. Статус код 200

_перехожу `Tests ➡️  Status Code is 200 ➡️  Sand  ➡️  Test Results`_

__response:__

    Status code is 200

3. Спарсить response body в json.

_перехожу в  `Snippets ➡️  Response body: JSON value check`_

  `оставляю код:`
  
   let responseData = pm.response.json();
   console.log('Response Data:', responseData)
  
`Console:`

    {age: "23", family: {…}, name: "Ilya"…}
    
4. Спарсить request.

let requestData = pm.request.url.query.toObject()  
console.log('Request Data:', requestData);

`Console:`  

    {age: "23", name: "Ilya", salary: "10000"}

6. Проверить, что name в ответе равно name s request (name забрать из request.)
7. Проверить, что age в ответе равно age s request (age забрать из request.)
8. Проверить, что salary в ответе равно salary s request (salary забрать из request.)

 __response:__  
 
9. Вывести в консоль параметр family из response.
10. Проверить, что у параметра dog есть параметры name.
11. Проверить, что у параметра dog есть параметры age.
12. Проверить, что параметр name имеет значение Luky.
13. Проверить, что параметр age имеет значение 4.

http://162.55.220.72:5005/object_info_4
1. Отправить запрос.
2. Статус код 200
3. Спарсить response body в json.
4. Спарсить request.
5. Проверить, что name в ответе равно name s request (name забрать из request.)
6. Проверить, что age в ответе равно age из request (age забрать из request.)
7. Вывести в консоль параметр salary из request.
8. Вывести в консоль параметр salary из response.
9. Вывести в консоль 0-й элемент параметра salary из response.
10. Вывести в консоль 1-й элемент параметра salary параметр salary из response.
11. Вывести в консоль 2-й элемент параметра salary параметр salary из response.
12. Проверить, что 0-й элемент параметра salary равен salary из request (salary забрать из request.)
13. Проверить, что 1-й элемент параметра salary равен salary*2 из request (salary забрать из request.)
14. Проверить, что 2-й элемент параметра salary равен salary*3 из request (salary забрать из request.)
15. Создать в окружении переменную name
16. Создать в окружении переменную age
17. Создать в окружении переменную salary
18. Передать в окружение переменную name
19. Передать в окружение переменную age
20. Передать в окружение переменную salary
21. Написать цикл который выведет в консоль по порядку элементы списка из параметра salary.

1. Вставить параметр salary из окружения в request
2. Вставить параметр age из окружения в age
3. Вставить параметр name из окружения в name
4. Отправить запрос.
5. Статус код 200
6. Спарсить response body в json.
7. Спарсить request.
8. Проверить, что json response имеет параметр start_qa_salary
9. Проверить, что json response имеет параметр qa_salary_after_6_months
10. Проверить, что json response имеет параметр qa_salary_after_12_months
11. Проверить, что json response имеет параметр qa_salary_after_1.5_year
12. Проверить, что json response имеет параметр qa_salary_after_3.5_years
13. Проверить, что json response имеет параметр person
14. Проверить, что параметр start_qa_salary равен salary из request (salary забрать из request.)
15. Проверить, что параметр qa_salary_after_6_months равен salary*2 из request (salary забрать из request.)
16. Проверить, что параметр qa_salary_after_12_months равен salary*2.7 из request (salary забрать из request.)
17. Проверить, что параметр qa_salary_after_1.5_year равен salary*3.3 из request (salary забрать из request.)
18. Проверить, что параметр qa_salary_after_3.5_years равен salary*3.8 из request (salary забрать из request.)
19. Проверить, что в параметре person, 1-й элемент из u_name равен salary из request (salary забрать из request.)
20. Проверить, что что параметр u_age равен age из request (age забрать из request.)
21. Проверить, что параметр u_salary_5_years равен salary*4.2 из request (salary забрать из request.)
22. ***Написать цикл который выведет в консоль по порядку элементы списка из параметра person.
