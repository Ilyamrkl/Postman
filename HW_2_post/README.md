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
2. Статус код 200
3. Спарсить response body в json.
4. Спарсить request.
5. Проверить, что name в ответе равно name s request (name забрать из request.)
6. Проверить, что age в ответе равно age s request (age забрать из request.)
7. Проверить, что salary в ответе равно salary s request (salary забрать из request.)
8. Вывести в консоль параметр family из response.
9. Проверить, что у параметра dog есть параметры name.
10. Проверить, что у параметра dog есть параметры age.
11. Проверить, что параметр name имеет значение Luky.
12. Проверить, что параметр age имеет значение 4.

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
