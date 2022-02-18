# H_W
Первое ДЗ 
Linux terminal (GitBash) commands

1) Посмотреть где я
 + pwd
 
2) Создать папку 
+ mkdir folder

3) Зайти в папку
+ cd folder

4) Создать 3 папки 
+ mkdir folder1 folder2 folder3

5) Зайти в любоую папку
+ cd folder3

6) Создать 5 файлов (3 txt, 2 json)  
+ touch t1.txt t2.txt t3.txt j1.json j2.json

7) Создать 3 папки 
+ mkdir folder4 folder5 folder6

8. Вывести список содержимого папки 
+ ls
+ ls -l
+ ls -la

9) + Открыть любой txt файл 
+ vim t1.txt

10) + написать туда что-нибудь, любой текст. 
+ i привет

11) + сохранить и выйти.  
+ Esc 
+ : wq 

12) Выйти из папки на уровень выше 
+ cd ..

13) переместить любые 2 файла, которые вы создали, в любую другую папку.

а) по одному

+ mv folder3/t1.txt folder1
mv folder3/j1.json folder1

б) два файла

+ mv folder3/t1.txt folder3/j1.json folder1

в) все файлы

+ mv folder3/* folder2

14) скопировать любые 2 файла, которые вы создали, в любую другую папку. 

а) по одному

+  folder3/t2.txt folder3/folder2
cp folder1/t1.txt folder2

б)два файла

+  folder3/t2.txt folder1/t1.txt folder2

в)все файлы

+ cp folder3/* folder2

15) Найти файл по имени
+ find -name t2.txt

16) просмотреть содержимое в реальном времени (команда grep) изучите как она работает.
+ tail -f t1.txt
+ tail -f test.txt | grep vika  (сортировка в файле test.txt по слову vika)

17) вывести несколько первых строк из текстового файла

а)вывести 10 первых строк

+ head t1.txt

б)вывести первых 3 строчки

+ head -3 t1.txt

18) вывести несколько последних строк из текстового файла

а)вывести 10 последних строк

+ tail t1.txt

б)вывести 3 последние строки файла

+ tail -3 t1.txt

19) просмотреть содержимое длинного файла (команда less) изучите как она работает.
+ less t1.txt

20) вывести дату и время -date

=========

Задание *

1) Отправить http запрос на сервер. http://162.55.220.72:5005/terminal-hw-request

а) curl http://162.55.220.72:5005/terminal-hw-request

б) curl "http://162.55.220.72:5005/get_method?name=alex&age=20"

в) ["alex","20"]

2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13
+ touch script.sh

```
#!/bin/bash
cd folder
mkdir folder1 folder2 folder3
cd folder3
touch t1.txt t2.txt t3.txt j1.json j2.json
mkdir folder4 folder5 folder6
ls -la
mv t1.txt folder4
mv j1.json folder5
```

+ chmod +x ./script
+ ./script
