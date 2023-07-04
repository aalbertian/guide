<!--|2|-->
# Руководство пользователя
## Интерфейс
### Вход в платформу
Для входа в платформу необходимо ввести логин и пароль. При ошибке аутентификации:
* проверьте введенные данные,
* обратитесь в IT-службу для проверки наличия учетной записи и соответствующих прав доступа.

> Предполагается, что учетные записи создаются при установке платформы (к примеру, через интеграцию с корпоративным AD) и авторизуются предварительно IT-службой – на основе внутренних политик безопасности конкретной компании.

![Вход_в_систему](/Images/login_to_the_platform.png)

### Меню и навигация

![Меню_и_нафигация](/Images/Menu_and_navigation.png)

Пояснения к меню:
1. Пункт основного меню.
2. Пункт меню второго уровня (подменю).
3. Вкладка внутри экрана.
4. Навигационный путь (проекты – проект – раздел – экран).
5. Верхнее меню (фиксированное меню).
6. Профиль авторизованного пользователя.
7. Завершение сеанса.

### Элементы экранных форм

Экранные формы Dognauts построены на компонентах фреймворка React. Помимо базовых элементов (таких как поля ввода, выпадающие списки, переключатели, загрузчики файлов и др.) – для ряда сценариев платформа использует мастер-формы (wizards), а также для ряда ключевых событий генерирует оповещения (см. главу ***Оповещения***) и всплывающие нотификации разного типа:

![Экранные формы](/Images/screen_form.png)
![Оповещения](/Images/notify.png)

### Валидация пользовательского ввода

Платформа предлагает проверку корректности заполнения полей – при возникновении ошибок пользователь увидит соответствующее предупреждение. При этом кнопки отправки (сохранения, обновления) таких форм будут неактивны до момента внесения корректных изменений, а также заполнения обязательных полей (помеченных *).

Кроме того, часть полей сопровождается бизнес-проверками – например, на правильность содержимого или связи со значением из соседнего поля. Такие бизнес-ошибки также отображаются пользователям под соответствующими полями в процессе их заполнения.

Несколько примеров ниже:
![Корректность_заполнения_полей](/Images/Correct_comment.png)