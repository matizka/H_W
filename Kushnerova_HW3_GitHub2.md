GitHub. HW_2
1. На локальном репозитории сделать ветки для:

Postman
+ git branch Postman

Jmeter
+ git branch Jmeter
CheckLists
+ git branch CheckLists
Bag Reports
+ git branch Bag_Reports
SQL
+ git branch  SQL
Charles
+ git branch Charles
Mobile testing
+ git branch Mobile_testing

2. Запушить все ветки на внешний репозиторий
+ git push -u origin --all

3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта
+ git checkout Bag_Reports - переходим на ветку Bag_Reports
+ touch bag.txt
+ vim bag.txt

ID- номер  
Summary (заголовок)    
Description (описание)  
Actual/expected result (фактический/ожидаемый результат)  
Attachments (вложения)  
Priority (приоритет)  
Severity (серьёзность)  
Status (статус)   

4. Запушить структуру багрепорта на внешний репозиторий
+ git add bag.txt
+ git commit -m "add text"
+ git push

5. Вмержить ветку Bag Reports в Main
+ git checkout main (перейти в ветку main)
+ git merge Bag_Reports

6. Запушить main на внешний репозиторий.
+ git push

7. В ветке CheckLists набросать структуру чек листа.
+ git checkout CheckLists (перейти в ветку CheckLists)
+ touch checklist.txt
+ vim checklist.txt

-ID («Номер»)  
-Tester Actions («Проверка», «Действия тестировщика»)  
-Actual Result («Результат»)  
-Comment («Комментарий»)  

8. Запушить структуру на внешний репозиторий
+ git add . ; git commit -m "add checklist.txt" ; git push

9. На внешнем репозитории сделать Pull Request ветки CheckLists в main

+ на сайте https://github.com выбираем репозиторий CheckLists 
+ на вкладке Pull requests нажать Compare&pull request -> create pull request

10. Синхронизировать Внешнюю и Локальную ветки Main
+ git checkout main (перейти в ветку main)
+ git pull
