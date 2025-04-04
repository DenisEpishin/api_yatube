# CRUD для Yatube

## Описание
Реализация API для всех моделей приложения Yatube

## Установка
Для установки и запуска проекта выполните следующие шаги:

1. Клонируйте репозиторий:
    ```bash
    git clone https://github.com/DenisEpishin/api_yatube
    ```
2. Перейдите в директорию проекта:
    ```bash
    cd api_yatube
    ```
3. Создайте виртуальное окружение:
    ```bash
    python -m venv venv
    ```
4. Активируйте виртуальное окружение:
    - Для Windows:
        ```bash
        venv\Scripts\activate
        ```
    - Для macOS и Linux:
        ```bash
        source venv/bin/activate
        ```
5. Установите необходимые зависимости:
    ```bash
    pip install -r requirements.txt
    ```

6. Проведите миграции:
    ```bash
    python yatube_api/manage.py makemigrations
    python yatube_api/manage.py migrate
    ```

8. Создайте суперпользователя:
    ```bash
    python yatube_api/manage.py createsuperuser
    ```

## Запуск
Для запуска сервера разработки выполните команду:
```bash
python yatube_api/manage.py runserver
```

## Тестирование
Проект содержит набор тестов, которые можно запустить с помощью pytest. Для этого из папки api_yatube выполните:
```bash
pytest
```
