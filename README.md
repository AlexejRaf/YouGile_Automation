# Дипломный проект: Автотесты для YouGile

## Описание

Дипломный проект по автоматизации тестирования сервиса **YouGile**.
Проект включает:
- **API-тесты** (5 штук) — проверка работы REST API.
- **UI-тесты** (6 штук) — проверка интерфейса через Selenium.

Объект тестирования:
- Создание, получение, обновление задач через API.
- Авторизация через веб-интерфейс.

## Стек
- Python 3.10+
- pytest, requests, selenium, allure-pytest, python-dotenv

## Установка
1. Клонировать репозиторий.
2. `pip install -r requirements.txt`
3. Скопировать `.env.example` в `.env` и заполнить своими данными.

## Настройка окружения

В файле `.env` (создаётся из `.env.example`) нужно указать:
- `BASE_URL` — базовый URL API
- `API_TOKEN` — API-ключ YouGile
- `UI_URL` — URL главной страницы
- `UI_USERNAME` — email для входа
- `UI_PASSWORD` — пароль
- `COLUMN_ID` — ID колонки для создания задач
- `BOARD_ID` — ID доски
- `ASSIGNEE_ID` — ID исполнителя

## Запуск
- API-тесты: `pytest api_tests/ -v`
- UI-тесты: `pytest ui_tests/ -v`
- Все: `pytest -v`

## Отчёт Allure
1. `pytest --alluredir=allure-results`
2. `allure serve allure-results`

## Структура проекта
API-тесты: 5 тестов
Пройдено: 5/5

UI-тесты: 6 тестов
Пройдено: 6/6

Всего 11 тестов
Пройдено: 11/11

## **【Ссылка на полный отчёт в Yonote] 
(https://moytestit.yonote.ru/doc/test-plan-yougile-api-Rz9SXXgbC2#h-vyvody-i-rekomendacii)**
(Тест-план, документация, результаты и рекомендации)
