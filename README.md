# Bash
В рамках обучения мною был изучен такой инсрумент как Bash, здесь представлены команды bash, которые я использовала для выполнения заданий

## Задание 1

- Определить имя папки, в которой вы находитесь                 
- $ pwd

- Создать внутри этой папки каталог с именем test1
- $ mkdir test1

- Перейти в папку test1
- $ cd test1

- Создать файл 1,2 и 3 внутри каталога test1
- $ touch file1.txt file2.txt file3.txt

- Проверить содержимое каталога test1
- $ ls

- Перейти в домашнюю директорию
- $ cd ..

- Создать папку test2 внутри домашней директории
- $ mkdir test2

- Удалить папку test2
- $ rmdir test2

- Удалить файл 2 из папки test1
- $ cd test1
- $ rm file2.txt

- Создать папку в домашней директории test3 и добавить в нее два файла
- $ cd ..
- $ mkdir test3
- $ cd test3
- $ touch file3.1.txt file3.2.txt

- Удалить папку test3
- $ rm -rf test3

- Создать папку test4 в домашней директории
- $ mkdir test4

- Переместить файлы 1 и 3 из папки test1 в папку test4
- $ mv test1/file1.txt test4
- $ mv test1/file3.txt test4

- Добавить в файл 1 три строки со словами line
- $ echo line > file1.tx
- $ echo line >> file1.txt
- $ echo line >> file1.txt

- Посмотреть содержимое файла 1
- $ cat file1.txt

- Добавьте в файл 3 три строки со словами line
- $ echo line > file3.txt
- $ echo line >> file3.txt
- $ echo line >> file3.txt

- Просмотрите содержимое двух файлов (1 и 3) сразу
- $ cat file1.txt file3.txt

- Используя один из редакторов замените все строки в файле 1
- $ nano file1.txt

## Задание 2

- Создать папку test 3
- $ mkdir test3

- Добавить в папку test 3 три файла 4, 5 и 6, в каждом из которых должно быть по 4 строки row1, row2, row3, row4
- $ touch file5.txt file4.txt filt6.txt
- $ echo row1 > file4.txt
- $ echo row2 >> file4.txt
- $ echo row3 >> file4.txt
- $ echo row4 >> file4.tx
- $ echo row1 > file5.txt
- $ echo row2 >> file5.txt
- $ echo row3 >> file5.txt
- $ echo row4 >> file5.txt
- $ echo row1 > file6.txt
- $ echo row2 >> file6.txt
- $ echo row3 >> file6.txt
- $ echo row4 >> file6.txt

- Найдите строку row2 в файле 5
- $ cd test3
- $ grep -i "row2" file5.txt

- Найдите строку row в папке test3
- $ grep -R "row" test3 .

- Посчитайте сколько строк с содержимым row в файле 6
- $ grep -c row file6.txt

- Найдите файл 5 внутри папки test3
- $ find test3 -name "file5.txt"

- Используя команду find, удалите файл 5
- $ find . -name "file5.txt" -delete

- Используя команду echo, добавьте слово test в файл 4
- $ echo test >> file4.txt

- Замените слово test в файле 4 на fail
- $ nano file4.txt

- Добавьте в файл 4 слово test так, чтобы сохранилось содержимое
- $ echo test >> file4.txt

- Просмотрите все процессы для юзеров не только в консоли, которые происходят в системе*
- $ ps aux

- Убейте процесс 666 в консоли
- $ kill 666

- Узнайте доступность ресурса artsiomrusau.com, используя ping
- $ ping artsiomrusau.com

- Отправьте 5 пакетов на сайт artsiomrusau.com
- $ ping -n 5 artsiomrusau.com

- Используя GET и команду curl, получите информацию о зарегистрированных питомцах на https://petstore.swagger.io/
- $ curl https://petstore.swagger.io/v2/pet/7890

- Используя POST и команду curl, создайте нового пользователя на https://petstore.swagger.io/
- $ curl -X POST -H "Content-Type: application/json" -d '{ "id": 7857, "username": "kivino", "firstName": "kivini", "lastName": "rini", "email": "kivini@mail.ru", "password": "456852", "phone": "85269874152", "userStatus": 0}' https://petstore.swagger.io/v2/user
{"code":200,"type":"unknown","message":"7857"}
