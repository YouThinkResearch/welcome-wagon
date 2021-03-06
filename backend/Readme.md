# Backend test

Что нужно сделать:

1. Использовать `typescript`, `workspaces`
2. Сделать аутенфикацию с `bcrypt`, емаилами-паролями и JWT токенами (сервер принимает токены через `Authorization: Bearer <token>`). Нужно использовать PostgreSQL и TypeORM как бэкенд. Можно использовать NestJS.
3. Сделать разделение по ролям: admin и manager. Admin может создавать новых пользователей, а manager – нет, но может делать все остальное.
4. Добавить новую `entity` – `surveys`, с полями `manager`, `name`, `link` и пагинацией. Поле `manager` может менять только `admin`; а если опрос создан менеджером, то в поле `manager` сохраняется айди текущего менеджера, который отправляет запрос. Так же `editSurvey`, `getSurveyById`, `listSurveys`
5. Добавить запрос `me`, `profiles`, `surveys` и другие запросы, которые нужны (например логин)
6. Все действия должны логироваться.
7. Нужно применять валидацию и другие best practices, где необходимо.

(бонусом можно сделать 2FA)
