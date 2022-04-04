1) Посмотреть где я — `pwd`
2) Создать папку — `mkdir hmwrk`
3) Зайти в папку — `cd hmwrk`
4) Создать 3 папки — `mkdir folder1 folder2 folder3`
5) Зайти в любоую папку — `cd folder1`
6) Создать 5 файлов (3 txt, 2 json) — `touch file1.txt file2.txt file3.txt file1.json file2.json`
7) Создать 3 папки — `mkdir f_1 f_2 f_3`
8) Вывести список содержимого папки — `ls -la`
9) Открыть любой txt файл — `vim file1.txt`
10) Написать туда что-нибудь, любой текст. — `(i) hello`
11) Сохранить и выйти. — `(esc) :wq`
12) Выйти из папки на уровень выше — `cd ..`
13) Переместить любые 2 файла, которые вы создали, в любую другую папку. — `mv file2.txt file3.txt ~/Desktop/GB/hmwrk/folder2`
14) Скопировать любые 2 файла, которые вы создали, в любую другую папку. — 
`cp ~/Desktop/GB/hmwrk/folder2/file2.txt ~/Desktop/GB/hmwrk/folder2/file3.txt ~/Desktop/GB/hmwrk/folder3`
15) Найти файл по имени — `find . -name "file2.txt"`
16) Просмотреть содержимое в реальном времени (команда grep) изучите как она работает. — `tail -f ./folder2/file2.txt | grep 7`
17) Вывести несколько первых строк из текстового файла — `head -n 3 file1.txt`
18) Вывести несколько последних строк из текстового файла — `tail -n 3 file1.txt`
19) Просмотреть содержимое длинного файла (команда less) изучите как она работает. — `less ./folder2/file2.txt`
20) Вывести дату и время — `date`
---
Задание *
1) Отправить http запрос на сервер http://162.55.220.72:5005/terminal-hw-request 
+ `curl http://162.55.220.72:5005/terminal-hw-request`
+ Response 1 — Intro":"Hello!! This is your the first response from server","Tasks":{"Task_1":"Send the next URL in terminal: http://162.55.220.72:5005/get_method?name=(set_your_String)&age=(set_your_number)","result":["Your_String","Your_number"]}}
+ Task_1 — `curl "http://162.55.220.72:5005/get_method?name=daniil&age=27"`
+ Response 2 — ["daniil","27"]

2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13 —

```
vim script_hw.bash
(i)
#!/bin/bash
mkdir hmwrk_script
cd hmwrk_script
mkdir folder1 folder2 folder3
cd folder1
touch file1.txt file2.txt file3.txt file1.json file2.json
mkdir f_1 f_2 f_3
ls -la
mv file2.txt file3.txt ~/Desktop/GB/hmwrk_script/folder2
(esq) :wq
chmod +x ./script_hw.bash
./script_hw.bash
```
