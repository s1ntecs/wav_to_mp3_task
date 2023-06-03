# wav_to_mp3_task
## тестовое задание №2 на вакансию Python разработчик, FastAPI quiz

Для запуска приложения необходимо сделать следующие действия:
  1. Скопируйте репозиторий
  ```
  git clone https://github.com/s1ntecs/wav_to_mp3_task.git
  ```
  2. Разверните приложение с помощью docker-compose, выполнив команду:
  ```
  docker-compose up --build
  ```
  3.  Создайте пользователя, отправив POST-запрос с помощью curl. Пример команды
  ```
  curl -X 'POST' \
    'http://127.0.0.1:8080/user/signup' \
    -H 'accept: application/json' \
    -H 'Content-Type: application/json' \
    -d '{
    "username": "lexa"
    }'
  ```
  4. Отправьте запрос на конвертацию WAV файла в MP3. Используйте команду curl, указав путь к WAV файлу, идентификатор пользователя и токен пользователя. Пример команды:
  ```
  $ curl -X POST -F "file=@example.wav" -F "user_id=идентификатор пользователя" -F "token=Токенпользователя" http://localhost:8080/file/upload/
  ```
  5. После обработки запроса вы получите ссылку для скачивания файла в формате MP3.

## Запросы вы можете сделать используя документацию http://127.0.0.1:8080/docs#
