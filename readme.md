RESTfull сервис.
Реализовать предпросмотр/просмотр, добавление и редактирование компаний-рекламодателей (advertisers) и рекламных кампаний, проводимых этими рекламодателями (campaigns)

Страницы:
1. Список рекламодателей. Необходимо наличие фильтрации по критериям, сортировки, постраничного просмотра (Pagination).
2. Предпросмотр, детальный просмотр характеристик рекламодателя/кампании (разные DTO).
3. Для пользователя добавление/редактирование рекламодателя, кампании.
4. Детальное редактирование кампании должно включать ссылку на картинку/видео, целевые страны, языки, группы пользователей по возрасту, геолокация итд.
   Необходимо наличие валидации вводимых данных. Ответ api должен содержать информацию почему реквест не валиден.
   Примечания:
   Удаление объектов сделать через soft delete (пометить флагом) и на клиента вытягивать все не удаленные.
   Написать unit тесты для сервисов с использованием какого-либо Mock фреймворка, например Mockito.
   Исходные/тестовые данные необходимо задать в виде миграций Flyway.

Технологии:

Java 8+, Spring Boot, Spring MVC (REST), Swagger, Spring Data\Spring JDBC, Spring Security, PostgreSQL
, Flyway\LiquidBase, Gradle\Maven.
Следовать принципам SOLID
Архитектура с разделением по слоям - Controller, Service, Repository и д.т. Общие вещи не дублировать, а делать через наследование от базовых классов (по возможности использовать generics).
Авторизация и 2 вида пользователей: администратор и простой пользователь.
Админ видит все компании/реклам и т.д. и всех пользователей