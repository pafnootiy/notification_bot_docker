#  Телеграмм бот для проверки статуса работ на Devman notification_bot_docker
### Как пользоваться

## Подготовка

- Убедитесь, что Docker установлен на вашей системе. Вы можете скачать и установить Docker с официального веб-сайта: [https://www.docker.com/get-started](https://www.docker.com/get-started)


* Клонируйте репозиторий: `git clone https://github.com/ваш-пользователь/notification_bot_docker.git`


* Перейдите в директорию проекта  `cd notification_bot_docker`
* Создайте файл .env и укажите необходимые переменные окружения:

  ` touch .env
  echo "TG_BOT_TOKEN=1929883349:AAHydfdZd3hdDZiuXVkyvHr4izyNQ1c0nGU" >> .env `
   
* Соберите Docker-образ:  `docker build -t notification_bot .`
* Запустите Docker-контейнер:  `docker run -d --name notification_bot_container notification_bot
`
* Убедитесь, что контейнер успешно запущен: `docker ps`
* Чтобы остановить контейнер: `docker stop notification_bot_container`

* Получите персональный чат ID. Для этого необходимо отправить сообщение боту https://t.me/userinfobot 
  
  Пример ответа от бота:
  
  @user7\
  Id: 232434172\
  First: Ivan\
  Last: Ivanov\
  Lang: ru


 
 



### Цель проекта
Код написан в образовательных целях на онлайн-курсе для веб-разработчиков Devman
 
