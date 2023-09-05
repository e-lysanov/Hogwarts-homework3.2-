# Homework3.2
Это домашнее задание, в котором осуществлена работа с базой данных студентов Хогвартса.
Тестировал запросы через Swagger/Postman.
Реализовано:
1. Получение списка студентов определенной возрастной категории
2. Получение факультета по названию или цвету
3. Настройка связи ManyToOne между студентом и факультетом (можно получить студентов факультета и факультет студента)
4. Написание класса Avatar и настройка связи OneToOne между студентом и аватаром
5. Возможность добавления аватара в БД и в директорию одновременно, а так же возможность получить картинку по отдельности как из БД, так и из директории
6. Написаны Mock-тесты и TestRestTemplate-тесты
7. Возможность получения всех студентов/последних пяти/их среднего возраста
8. Возможность постраничного получения списка аватаров
9. В корне проекта написан файл scripts42.sql для создания ограничений
10. Подключена зависимость liquibase-core. Создан файл миграций с двумя changeset`ами с SQL-командами для создания индексов. Настроен файл changelog-master.yml
11. Во все методы сервисов добавлено логирование
12. Настроил конфигурации Application с возможностью запуска приложения на разных портах, реализован метод получения актуального порта
13. Создан эндпоинт, который возвращает отсортированные в алфавитном порядке имена всех студентов в верхнем регистре, чье имя начинается на букву А, эндпоинт, который возвращает средний возраст всех студентов, эндпоинт, который возвращает самое длинное название факультета (посредством Stream API)
14. Создан эндпоинт, который запускает два параллельных потока для вывода имен студентов в консоль, а так же эндпоинт, который запускает два СИНХРОНИЗИРОВАННЫХ параллельных потока для вывода имен студентов в консоль 
