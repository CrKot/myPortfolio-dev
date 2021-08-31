# Вступление
### Что-бы запустить проект, необходимо загрузить myPortfolio-front и myPortfolio-back в корень текущего проекта

 создать .env файлы в следующих репозиториях:
- текущем(myPortfolio-dev)
- фронтэнд(myPortfolio-dev/myPortfolio-front)
- бэкэнд(myPortfolio-dev/myPortfolio-back)

Примеры .env файлов есть в каждом репозитории

#### .env файл в umka-dev

    DB_USERNAME=<Указываем имя пользователя для базы данных mongodb>
    DB_PASSWORD=<Указываем пароль для базы данных mongodb>
    DB_DATABASE=<Указываем имя базы данных mongodb>

#### .env файл в myPortfolio-front

    BACKEND_URL=http://127.0.0.1:8080

#### .env файл в myPortfolio-back

    DB_CONNECTION=mongodb://mongodb:27017/?retryWrites=true&w=majority
    DB_NAME:<Указываем имя базы данных mongodb>
    DB_USER:<Указываем имя пользователя для базы данных mongodb>
    DB_PASSWORD:<Указываем пароль для базы данных mongodb>
    SERVER_PORT=8080
    SESSION_SECRET=<Секретное слово, например test>
    FRONTEND_URL=http://127.0.0.1:3000


# Запуск

После того как все .env файлы созданы, необходимо в коммандной строке запустить команду ***docker-compose up***
Предпологается, что на вашем сервере уже установлен Docker, в ином случае перейдите по [ссылке](https://docs.docker.com/engine/install/ubuntu/)
для получаения инструкции по установке Docker
После запуска контейнера командой ***docker-compose up***, необходимо дождаться когда установки всех образов и всех зависимостей внутри образов

# Использование

После того как установлены все образы и все зависимости внутри образов, в консоли браузера необходимо перейти по адресу [127.0.0.1:3000](https://127.0.0.1:3000) 