# Banking_manager_UI

#### Примечание:
Проект был выполнен в рамках участия в SDET практикуме, где одним из дополнительных требований было наличие возможности запуска в системе CI/CD. Из-за этого было решено реализовать его в gitlab.

---

#### Ссылки на документацию:


[Посмотреть задание](https://gitlab.com/evge_qa/banking_manager/-/blob/main/documentation/task.md)

[Посмотреть тест кейсы](https://gitlab.com/evge_qa/banking_manager/-/blob/main/documentation/testcases.md)

[Посмотреть отчет Allure](https://evge_qa.gitlab.io/-/banking_manager/-/jobs/6424598250/artifacts/allure-report/index.html)

---

### Запуск проекта
#### Настройка:
- Клонируйте репозиторий на свой компьютер
```
git clone https://gitlab.com/evge_qa/banking_manager.git
```
- Перейдите в корневую папку проекта

- Создайте виртуальное окружение:
```
python -m venv venv
```

- Активируйте виртуальное окружение:

Windows:
```
.\venv\Scripts\activate
```
macOS и Linux:
```
source venv/bin/activate
```
#### Зависимости:

- Установите зависимости:
```
pip install -r requirements.txt
```

#### Запуск автотестов

- Выполните команду для запуска тестов:
```
pytest -s -v
```
- Выполните команду для параллельного запуска тестов:
```
pytest -s -v --dist loadgroup   
```

#### Генерация и запуск отчетов Allure

- Выполните команду для запуска тестов:
```
pytest -s -v --alluredir allure-results
```
- Выполните команду для параллельного запуска тестов:
```
pytest -s -v --dist loadgroup --alluredir allure-results
```
- Выполните команду для просмотра отчета:
```
allure serve allure-results
```
