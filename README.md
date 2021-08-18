### 09.05_Gitlab </br>
=======================================</br>
### Подготовка к выполнению: </br>
1) Регистрация на gitlab в saas [https://gitlab.com/murzinvit](https://gitlab.com/murzinvit)</br>
2) Создание проекта в gitlab [https://gitlab.com/evo_g/netology-6](https://gitlab.com/evo_g/netology-6)</br>
3) Перенос файлов в репозиторий [gitlab](https://github.com/murzinvit/screen/blob/0fcbe00c43537b2c3095d025215bc528a766e2fb/GITLAB/gitlab.jpg) </br>
### Основная часть </br>
### DevOps </br>
В репозитории содержится код проекта на python. Проект - RESTful API сервис. Ваша задача автоматизировать сборку Docker образа с выполнением python-скрипта: </br>
Gitlab репозиторий, ветка main [https://gitlab.com/evo_g/netology-6](https://gitlab.com/evo_g/netology-6)</br>

### Результат выполнения CI:</br>
![ci_complit](https://github.com/murzinvit/screen/blob/264a4db5925bcc9a08242e9ec016cc17b551b459/GITLAB/Git_lab_CI_complit.jpg)</br>

### Product Owner</br>
Проекту нужна бизнесовая доработка: необходимо поменять JSON ответа на вызов метода GET /rest/api/get_info, с { "message": "Already started" } на { "message": "Running"}</br>
Создал ветку [dev](https://gitlab.com/evo_g/netology-6/-/tree/dev), изменил выводимый текст, сделал сборку по ветке dev:</br>

### Результат выполнения CI:</br>
![Build_on_dev](https://github.com/murzinvit/screen/blob/50ecf0091f6815d2106e44cbd3464ccd3b86c8fa/GITLAB/Build_on_dev.jpg)</br>

### Developer </br>
Вам пришел новый Issue на доработку: </br>

### Tester </br>
Разработчики выполнили новый Issue, необходимо проверить валидность изменений: </br>
