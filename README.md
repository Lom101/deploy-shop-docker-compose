# Deploy shop docker compose

## Описание

Этот репозиторий предназначен для запуска приложения "Shop" с помощью Docker Compose на production. Docker compose вытягивает образы из Docker Hub, для возможности изменить, просмотреть код используйте другой репозиторий: 
- https://github.com/Lom101/localhost-shop-docker-compose.git

## Структура проекта

Проект состоит из docker-compose.yml..

## Требования

- Docker
- Docker Compose

## Установка

1. **Клонируйте репозиторий с подмодулями**:

   ```bash
   git clone https://github.com/Lom101/deploy-shop-docker-compose.git
   ```

2. **Создайте файл .env**:

    Скопируйте файл .env.example в .env:
    ```bash
    cp .env.example .env
    ```
    Заполните переменные в .env необходимыми значениями.

## Запуск приложения

Чтобы запустить приложение, выполните следующую команду в корневой директории проекта:

```bash
docker-compose up --build
```

Эта команда соберет необходимые образы и запустит все сервисы.

## Доступ к приложению

Вместо localhost может быть ip вашего сервера

- Web API: http://localhost:5000/swagger/index.html
- Фронтенд: http://localhost

## Остановка приложения

Чтобы остановить приложение, нажмите `Ctrl+C` в терминале, где запущен `docker-compose`. Вы также можете выполнить команду:

```bash
docker-compose down
```

## Поддержка

Если у вас возникли вопросы или проблемы, пожалуйста, откройте issue в этом репозитории.
