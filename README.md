   # Diplom_Project
Этот проект представляет собой автоматизированный тестовый фреймворк на базе pytest, selenium и allure для проверки API и UI веб-приложения Кинопоиск.

  ## Используемые библиотеки

pytest
selenium
allure-pytest
requests
webdriver-manager
flake8

   ## Возможности

API тестирование публичного REST API
UI тестирование через Selenium WebDriver
Генерация отчетов с помощью Allure
Структурированная архитектура (Page Object Model)

   ## Структура проекта
config/  settings.py # Настройки проекта (BASE_URL, API ключ и т.д.) 

search_page.py # PageObject для страницы поиска 

movie_page.py # PageObject для страницы фильма 

base_page.py # Базовый класс страницы

tests/  test_api.py # API тесты 

test_ui.py # UI тесты

Запуск тестов API тесты: bash pytest tests/test_api.py --alluredir=allure-results

UI тесты: bash pytest tests/test_ui.py --alluredir=allure-results


Для запуска в видимом режиме — закомментируйте или удалите --headless=new в conftest.py.


### Полезные ссылки
- [Гайд по Markdown] (https://www.markdownguide.org/basic-syntax/)
- [Генератор файлов .gitignore] (https://www.toptal.com/developers/gitignore.)
- [Про pip freez] (https://pip.pypa.io/en/stable/cli/pip_freeze/)