### 09.05_Gitlab </br>
=======================================</br>
### Подготовка к выполнению: </br>
1) Регистрация на gitlab в saas [https://gitlab.com/murzinvit](https://gitlab.com/murzinvit)</br>
2) Создание проекта в gitlab [https://gitlab.com/evo_g/netology-6](https://gitlab.com/evo_g/netology-6)</br>
3) Перенос файлов в репозиторий [gitlab](https://github.com/murzinvit/screen/blob/0fcbe00c43537b2c3095d025215bc528a766e2fb/GITLAB/gitlab.jpg) </br>
4) Добавление ssh ключа - Login -> preferences. </br>

### Основная часть </br>
### DevOps </br>
В репозитории содержится код проекта на python. Проект - RESTful API сервис. Ваша задача автоматизировать сборку Docker образа с выполнением python-скрипта: </br>
Gitlab репозиторий, ветка main [https://gitlab.com/evo_g/netology-6](https://gitlab.com/evo_g/netology-6)</br>

### Результат выполнения CI:</br>
![ci_complit](https://github.com/murzinvit/screen/blob/264a4db5925bcc9a08242e9ec016cc17b551b459/GITLAB/Git_lab_CI_complit.jpg)</br>

### Product Owner</br>
Проекту нужна бизнесовая доработка: необходимо поменять JSON ответа на вызов метода GET /rest/api/get_info, с { "message": "Already started" } на { "message": "Running"}</br>
В issue создал ветку [1-modify-get_info](https://gitlab.com/evo_g/netology-6/-/tree/dev), изменил выводимый текст, далее сборка по ветке 1-modify-get_info:</br>

### Результат выполнения CI:</br>
![Build_on_1-modify-get_info](https://github.com/murzinvit/screen/blob/ac22bbcf6de8c2ef57d7b3034b38186543cae306/GITLAB/Build_in_dev_branch.jpg)</br>

### Результат Merge request: </br>
![Merged](https://github.com/murzinvit/screen/blob/f8c99c101ec09581521879f7deaa765649786e8a/GITLAB/Merged.jpg) </br>
### Результат Build </br>
![Result](https://github.com/murzinvit/screen/blob/0feaae0ae6bdcbdfc9a48ae7e0026ec4b99d6e3c/GITLAB/Build_merged_result.jpg) </br>

### Developer </br>
Вам пришел новый Issue на доработку: </br>

### Tester </br>
Разработчики выполнили новый Issue, необходимо проверить валидность изменений, поднять контейнер проверить вывод метода get_info: </br>
1) docker pull registry.gitlab.com/evo_g/netology-6/python-api </br>
2) docker run -d --name netology -p 5290:5290 registry.gitlab.com/evo_g/netology-6/python-api:latest </br>
