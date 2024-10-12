# Aiogram Telegram Bot in Docker

## Описание

Это пример бота на базе библиотеки Aiogram, упакованный в контейнер Docker для удобного развертывания и управления. Бот имеет как обычную кнопочную клавиатуру, так и инлайн-кнопки, которые могут быть использованы для взаимодействия с пользователем. Главная цель проекта — возможность запуска нескольких копий бота с разными токенами в отдельных контейнерах для масштабируемости и удобного управления.

## Функционал бота

- Обычные кнопочные клавиатуры для текстового общения
- Инлайн-кнопки с callback-ответами
- Удобное управление ботами через Docker
- Поддержка множества ботов с помощью отдельного контейнера для каждого токена

## Требования

- Python 3.7+
- Docker
- Файл `api_keys.txt` с токенами ботов

## Установка

1. **Склонируйте репозиторий:**

   ```bash
   git clone https://github.com/your-repo/aiogram-docker-sample.git
   cd aiogram-docker-sample

2. **Создайте Docker image:**
Выполните команду, чтобы собрать Docker image для бота:
    ```bash
   docker build -t aiogram_bot_image .
   


## **Основные команды:**
#### Запуск всех ботов:
   `python run_bots.py`

#### Остановка всех ботов:
   `python stop_bots.py`

#### Проверка активных контейнеров:
   `docker ps`

#### Просмотр логов контейнера:
   `docker logs <container_name>`

#### Остановка определённого контейнера:
   `docker stop <container_name>`
