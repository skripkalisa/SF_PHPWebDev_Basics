# Создание локального репозитория

## Первоначальные настройки GIT

### **Имя и Email**

Без этих настроек вы просто не сможете работать, GIT их запрашивает в самом начале в принудительном порядке.

Задать email для всех своих репозиториев:

    > git config --global user.email  "email@example.com"

Задать имя:

    > git config --global user.name "John"

Посмотреть текущий email:

    > git config --global user.email

### **Запомнить учетные данные**

Это замечание касается работы через HTTPS-протокол.

Чтобы при отправке изменений на **GitHub** каждый раз не вводить имя и пароль, имеет смысл перед выполнением команды **push** попросить запомнить ваши данные:

    > git config credential.helper store

Потом выполнить отправку с указанием имени и пароля:

    > git push https://github.com/javakitt/example
    > Username: <type your username>
    > Password: <type your password>

И уже в следующий раз вводить имя пароль не придется



## **Для того чтобы создать репозиторий:**
1. Создайте папку, в которой он будет располагаться. Например, это будет каталог с названием ***repo***.

Windows, MacOS, Linux:

    > mkdir repo

2. Теперь перейдем в этот каталог.

Windows, MacOS, Linux:

    >cd repo
3. Создадим в нем пустой git репозиторий.

    > git init

Проверить состояния репозитория можно командой: 

    > git status
    On branch master

    Initial commit

    nothing to commit (create/copy files and use "git add" to track)

Посмотреть список внесённых изменений (коммитов) можно командой:

    > git log
    fatal: your current branch 'master' does not have any commits yet