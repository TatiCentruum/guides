# Создание токена для работы с GitHub

1. Подтвердите свой адрес электронной почты, если он еще не подтвержден.

2. В правом верхнем углу любой страницы щелкните фотографию своего профиля, затем нажмите **Settings** (Настройки). 

![Пункт Settings](images/userbar-account-settings.png)

3. На левой боковой панели нажмите **Developer settings** (Настройки разработчика). 
   
![Настройки разработчика](images/developer-settings.png)


4. На левой боковой панели щелкните **Personal access tokens** (Личные токены доступа).

![Токены личного доступа](images/personal_access_tokens_tab.png)


5. Щелкните **Generate new token** (Создать новый токен).

![Кнопка создания нового токена](images/generate_new_token.png)


6. Дайте вашему токену описательное имя (любое, удобное Вам).

![Поле описания токена](images/token_description.png)


7. Выберите области или разрешения, которые вы хотите предоставить этому токену. Чтобы использовать свой токен для доступа к репозиториям из командной строки, выберите **repo**.

![Выбор областей действия токенов](images/token_scopes.gif)


8. Щелкните **Generate token** (Создать токен).

![Кнопка создания токена](images/generate_token.png)


9. Щелкните кнопку ![Недавно созданный токен](images/personal_access_tokens.png), чтобы скопировать токен в буфер обмена. По соображениям безопасности после того, как вы покинете страницу, вы больше не сможете увидеть токен. Сохраните его в удобном и надёжном месте, чтобы не потерять.

![Недавно созданный токен](images/personal_access_tokens1.png)


10. В дальнейшем, при запросе учетных данных (логина и пароля), вместо пароля указывайте этот токен.

```
$ git clone https://github.com/username/repo.git
Username: ваш юзернейм
Password: токен, который вы сгенерировали
```

> Предупреждение: относитесь к своим токенам как к паролям и держите их в секрете. Обязательно сохраните токен и не теряйте его! При утере проделайте все шаги заново.

[Оригинал](https://docs.github.com/en/github/authenticating-to-github/keeping-your-account-and-data-secure/creating-a-personal-access-token)