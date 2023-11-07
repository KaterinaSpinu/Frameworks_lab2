# Frameworks_lab2
Контрольные вопросы: 

1.	Что представляет собой `Service Layer` (Слой сервисов) в архитектуре Model-View-Controller (MVC) веб-приложений, и какую роль он играет в разделении бизнес-логики?

Service Layer (Слой сервисов) в архитектуре Model-View-Controller (MVC) веб-приложений представляет собой слой, который отвечает за обработку бизнес-логики приложения. Его цель - разделить бизнес-логику от представления (View) и уровня доступа к данным (Model). Слой сервисов содержит сервисы, которые предоставляют высокоуровневый интерфейс для выполнения операций приложения, таких как создание, редактирование, удаление и получение данных. Сервисы инкапсулируют логику, что упрощает поддержку, улучшает тестируемость и соблюдение принципов SOLID.

2.	Объясните понятия аутентификации и авторизации в веб-разработке. Как они связаны и почему они важны для безопасности приложений?

Аутентификация - это процесс проверки подлинности пользователя. Это процесс, при котором приложение удостоверяет, что пользователь действительно тот, за кого себя выдаёт, чаще всего путем проверки логина и пароля.
Авторизация — это процесс установления того, какие действия или ресурсы пользователь имеет право выполнять или получать доступ. Она определяет, какие ресурсы доступны для конкретного пользователя, и основана на его ролях или правах.
Аутентификация и авторизация важны для безопасности приложений, так как они позволяют предотвратить несанкционированный доступ к данным и функциональности приложения, а также защищают конфиденциальность пользовательских данных.

3.	Как, в выбранном Вами фреймворке, можно реализовать авторизацию пользователей и ограничение доступа к определенным маршрутам или действиям на основе их ролей?
В Symfony, авторизацию пользователей и ограничение доступа к маршрутам или действиям можно реализовать с использованием Symfony Security Bundle. Для этого необходимо: 
1)	Настроить аутентификацию, определив, как пользователи будут аутентифицироваться (например, через логин и пароль).
2)	Создать систему ролей и ролевой иерархии для определения прав доступа пользователей.
3)	Применить аннотации @IsGranted к методам контроллеров или использовать конфигурацию маршрутов для ограничения доступа на основе ролей.
4.	В чем заключается разница между юнит-тестированием, интеграционным тестированием?

Юнит-тестирование — это тип тестирования, который проверяет отдельные компоненты (или "юниты") приложения на корректное выполнение их функций. Он изолирует компонент, который тестируется, от остальных частей приложения. Цель - проверить, что каждый компонент работает правильно в изоляции.
Интеграционное тестирование — это тип тестирования, который проверяет взаимодействие между различными компонентами или модулями приложения. Он оценивает, как эти компоненты взаимодействуют друг с другом и проверяет, что они работают вместе правильно. Цель - проверить, что компоненты интегрируются правильно и взаимодействуют корректно.
