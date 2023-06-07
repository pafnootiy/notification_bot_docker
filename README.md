#  Телеграмм бот для проверки статуса работ на Devman notification_bot_docker
### Как пользоваться

## Подготовка

- Убедитесь, что Docker установлен на вашей системе. Вы можете скачать и установить Docker с официального веб-сайта: [https://www.docker.com/get-started](https://www.docker.com/get-started)


* Клонируйте репозиторий: `git clone https://github.com/ваш-пользователь/notification_bot_docker.git`


* Перейдите в директорию проекта  `cd notification_bot_docker`
* Соберите Docker-образ:  `docker build -t notification_bot .`
* Запустите Docker-контейнер:  `docker run -d --name notification_bot_container notification_bot
`
* Убедитесь, что контейнер успешно запущен: `docker ps`
* Чтобы остановить контейнер: `docker stop notification_bot_container`

* Добавьте переменные окружения.\
  Для работы со скриптом  создайте и настройте файл с переменными окуржения `*.env`.\
  В данный файл необходимо внести токены
  
  Пример
  
    `DEVMAN_TOKEN=Token 1173ebb27few245sdfdfa91b53b5a2c5491`
    
    `TG_BOT_TOKEN=1929883349:AAHydfdZdfdfrr5gHr4izyNQ1c0nGU`
    
    `TG_CHAT_ID=232434172`
 


* Получите персональный чат ID. Для этого необходимо отправить сообщение боту https://t.me/userinfobot 
  
  Пример ответа от бота:
  
  @user7\
  Id: 232434172\
  First: Ivan\
  Last: Ivanov\
  Lang: ru


 
 



### Цель проекта
Код написан в образовательных целях на онлайн-курсе для веб-разработчиков Devman
 
