# Дипломный проект профессии «Тестировщик»

Запуск SUT, авто-тестов и генерация репорта
Подключение SUT к PostgreSQL
Запустить Docker Desktop
Открыть проект в IntelliJ IDEA
В терминале в корне проекта запустить контейнеры:
docker-compose up -d

Запустить приложение:
java -jar .\artifacts\aqa-shop\aqa-shop.jar --spring.datasource.url=jdbc:postgresql://localhost:5432/app
Открыть второй терминал

Запустить тесты:
.\gradlew clean test -DdbUrl=jdbc:postgresql://localhost:5432/app
Создать отчёт Allure и открыть в браузере
.\gradlew allureServe

Закрыть отчёт:
CTRL + C -> y -> Enter

Перейти в первый терминал

Остановить приложение:
CTRL + C

Остановить контейнеры:
docker-compose down

Подключение SUT к MySQL
Запустить Docker Desktop
Открыть проект в IntelliJ IDEA
В терминале в корне проекта запустить контейнеры:
docker-compose up -d

Запустить приложение:
java -jar .\artifacts\aqa-shop\aqa-shop.jar --spring.datasource.url=jdbc:mysql://localhost:3306/app
Открыть второй терминал

Запустить тесты:
.\gradlew clean test -DdbUrl=jdbc:mysql://localhost:3306/app
Создать отчёт Allure и открыть в браузере
.\gradlew allureServe

Закрыть отчёт:
CTRL + C -> y -> Enter
Перейти в первый терминал

Остановить приложение:
CTRL + C

Остановить контейнеры:
docker-compose down

# Документация
Текст задания
План автоматизации
Отчётные документы по итогам тестирования
Отчётные документы по итогам автоматизации
