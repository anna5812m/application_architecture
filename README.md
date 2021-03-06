# Sahana Eden

## Назначение ПО

Sahana Eden - это бесплатная система с открытым исходным кодом для управления операциями в случае бедствий, которая высоко ценится за ее конфигурируемость и настраиваемость. Она предоставляет правительствам, организациям, гражданскому обществу, сообществам и пострадавшим лицам решение для реагирования на стихийное бедствие, когда оно происходит.
В настоящее время последняя разработка Sahana Eden включает в себя множество функций для управления организациями, людьми, проектами, инвентарными запасами и активами, а также для обработки оценочной информации и обеспечения ситуационной осведомленности с помощью карт. Ее цель - заранее спланировать ситуацию, чтобы реакция была быстрой, и предоставить инструмент управления в такой ситуации. 
Sahana Eden высоко ценится различными сообществами, от правительственных и неправительственных организаций, которые ценят настраиваемость, до академических исследователей, которые видят в нем полезную платформу для анализа и изучения программного обеспечения для управления стихийными бедствиями с открытым исходным кодом.

## Заинтересованные лица

- Совет директоров Sahana Eden

Основная команда Sahana Eden (их совет директоров) наблюдает за будущей дорожной картой компании, создавая проблемы и участвуя в обсуждениях для разработки системы.
- Оценщики

Основная команда сама оценивает соответствие стандартам и правовым нормам.
- Коммуникаторы

Члены основной команды регулярно публикуют обновления и разработки Sahana Eden на внешних коммуникационных платформах (их веб-сайт, блог, Twitter и т.д.).
- Разработчики

- Сопровождающие

Общее развитие поддерживается основными разработчиками, все другие задачи обслуживания, такие как исправление ошибок, выполняются участниками. Команда локализации назначает специалиста по сопровождению для каждого языкового перевода, и командами руководят основные члены команды.
- Поставщики

Вспомогательные организации обеспечивают меры по оказанию помощи и не имеют прямого отношения к системе. Поскольку Sahana Eden также является автономной системой, развертывание которой выполняется пользователями, которые ее используют.
- Вспомогательный персонал

Поддержка разработки Sahana Eden осуществляется как внутренними, так и внешними разработчиками через github и группы Google.
- Системные администраторы

Поскольку Sahana Eden развертывается самостоятельно, пользователь становится системным администратором.
- Тестеры

Основная команда занимается исправлением ошибок и сообщением об ошибках. Кроме того, члены сообщества Sahana могут зарегистрироваться в качестве тестировщиков для участия в тестировании ветвей разработки. Trendspotter - один из основных тестеров системы.
- Пользователи

Конечные пользователи представляют большую часть сообщества Sahana Eden. Они варьируются от волонтеров, организаций здравоохранения или государственных организаций. Их больше всего беспокоит функциональность системы.
- Конкуренты

Ushahidi - это организация по реагированию на стихийные бедствия с открытым исходным кодом, которая позволяет любому собирать распределенные данные с помощью SMS, электронной почты или Интернета и визуализировать их на карте или временной шкале. Их цель - создать самый простой способ сбора информации от общественности для использования в кризисных ситуациях.
- Исследователи и ученые

Исследуют и представляют результаты работы системы в журналах. Они также являются неотъемлемой частью улучшения функциональности системы.
- СМИ

Представляют собой однозначные и надежные источники информации и имеют жизненно важное значение для коммуникации системы с людьми и разработчиками, которые заинтересованы в новых задачах и проектах.


## Функции

- Картографирование (Mapping) — контроль за ситуацией и геопространственный анализ.
- Управление запросами (Requests Management) — отслеживание запросов о помощи и сопоставление их с теми, кто способен такую помощь оказать.
- Управление волонтёрами (Volunteer Management) с учётом их навыков, доступности и размещения.
- Реестр пропавших людей (Missing Persons Registry) — учёт и поиск пропавших людей.
- Идентификация жертв стихийных бедствий (Disaster Victim Identification).
- Реестр укрытий (Shelter Registry) — отслеживание размещения, вместимости и распределение пострадавших в укрытия.
- Управление медицинскими учреждениями (Hospital Management System) - медучреждения могут предоставлять информацию о ресурсах и потребностях.
- Реестр организаций (Organization Registry) — “кто, где и чем занимается”. Помогает организациям координировать свою деятельность.
- Система заявок (Ticketing☭) — главный журнал сообщений для обработки входящих отчетов и запросов.
- Сообщения (Messaging) — приём и отправка предупреждений через Email и SMS.
- Библиотека документов (Document Library) — библиотека цифровых ресурсов, таких, как фотографии и офисные документы.
- Интеграция с Ushahidi (Ushahidi Integration) — возможность интеграции данных из Ushahidi.

## Контекстное представление

![](https://github.com/anna5812m/application_architecture/blob/main/ContextDiagram.png)

## Архитектура приложения

![](https://github.com/anna5812m/application_architecture/blob/main/Architecture.png)

## Диаграмма развертывания

![](https://github.com/anna5812m/application_architecture/blob/main/DeploymentView.png)

## Особенности реализации

1) Интернационализация.

Поскольку с этой системой должны взаимодействовать разные люди из разных стран и культур, важно, чтобы система была понятна всем пользователям. Большинство языков обрабатываются с помощью механизма локализации web2py. Он содержит файл для каждого языка, который содержит переводы с английского на нужный язык. Некоторые из этих файлов были созданы с помощью Google Translate.

2) Импорт и экспорт.

Поскольку Sahana Eden позволяет организациям сотрудничать друг с другом, ей приходится импортировать данные из большинства этих организаций. Эти данные могут варьироваться от информации об инвентаризации до данных об определенной области. Для поддержки большого количества различных форматов, используемых для импорта и экспорта данных, они используют шаблоны XSLT.

3) Условные обозначения кода.

Чтобы проверить соглашения кода, они используют несколько инструментов, включая PEP8, PyLint и PyChecker. Поскольку они нацелены на международную доступность, все строки должны быть помечены, чтобы соответствующий язык можно было извлечь из соответствующего файла. Кроме того, все файлы, классы и функции должны иметь строку документации, позволяющую автоматически создавать документацию по API с помощью Epydoc.

4) EdenTest.

EdenTest - это тестовая среда на основе Robot Framework, используемая для автоматического тестирования в Sahana Eden. Файлы, реализующие эти тесты, представляют собой файлы .txt, которые содержат инструкции. Эти функции определены в отдельных файлах, что упрощает их повторное использование.

5) Единичные тесты.

У каждого модуля есть собственный набор тестов, который запускался отдельно. Помимо проверки, эти тесты используются для проверки соответствия дизайна требованиям, упрощения и целенаправленности реализации и упоминания о том, что это может быть отличным источником примеров кода для применения ваших методов API. Настроен сервер непрерывной интеграции, использующий Travis. Всякий раз, когда создается запрос на вытягивание, все модульные тесты запускаются раньше и должны быть успешными, прежде чем его можно будет объединить.

## Литература

1. GitBook - https://delftswa.gitbooks.io/desosa2018/content/eden/chapter.html/
2. Sahana Eden deployments - https://sahanafoundation.org/eden/deployments/
3. Github language files - https://github.com/sahana/eden/tree/master/languages
4. The website of the Sahana foundation. It contains information about who is contributing, guidelines, a blog and also links to other useful resources. - https://sahanafoundation.org/ -
5. A book describing the system - http://archive.flossmanuals.net/_booki/sahana-eden/sahana-eden.pdf
6. The demo of the system was used to get a good overview of the system. - http://demo.sahanafoundation.org/eden/
7. Google Groups for discussions - https://groups.google.com/forum/#!forum/sahana-eden
8. Facebook - https://www.facebook.com/SahanaFOSS/
9. XSLT Templates - http://eden.sahanafoundation.org/wiki/XsltTemplates -
10. Sahana Eden Github repository - https://github.com/sahana/eden
11. Sahana Eden brochure - https://www.slideshare.net/SahanaFOSS/sahana-eden-brochure-10577413
12. Disaster Risk Reduction Project Portal website - http://www.drrprojects.net/drrp/
13. Sahana Eden Wiki - http://eden.sahanafoundation.org/wiki/
14. Sahana Eden coding conventions - http://eden.sahanafoundation.org/wiki/DeveloperGuidelines/CodeConventions
15. SonarQube - https://www.sonarqube.org/
