Задача 2:
-
• физические сервера=> Windows-системы для использования бухгалтерским отделом;
ПДН - информация конфиденциального характера и для защиты данных в соответствии с классом защиты выгодно будет использовать физический сервер. 

• виртуализация уровня ОС=> Системы, выполняющие высокопроизводительные расчёты на GPU ; Высоконагруженная база данных MySql, критичная к отказу (если есть быстрое выделенное хранилище в противном случае физические сервера); Различные web-приложения.

• Паравиртуализация=> виртуализация уровня ОС=> Системы, выполняющие высокопроизводительные расчёты на GPU; Высоконагруженная база данных MySql, критичная к отказу (если есть быстрое выделенное хранилище в противном случае физические сервера); Различные web-приложения.
Виртуализация уровня ОС или паравиртуализация выбор будет отличатся наличием специалистов. Виртуализация — это экономически выгодно и надежно (резервное копирование и восстановление).

Задача 3:
-
1) 100 виртуальных машин на базе Linux и Windows, общие задачи, нет особых требований. Преимущественно Windows based-инфраструктура, требуется реализация программных балансировщиков нагрузки, репликации данных и автоматизированного механизма создания резервных копий.  
Kubernetes -  открытое программное обеспечение для оркестровки контейнеризированных приложений — автоматизации их развёртывания, масштабирования и координации в условиях кластера. Поддерживает основные технологии контейнеризации, включая Docker, rkt, также возможна поддержка технологий аппаратной виртуализации[7].
ESXi VMware используется для создания гипервизоров, предназначенных для запуска нескольких связанных общей сетью автономных операционных систем на одном хосте. Есть возможность подключения гипервизоров ESXi к удаленным хранилищам для организации полноценных виртуальных машин с целью защиты контейнеризации. Также предусмотрена функция создания кластеров, составляемых минимум из 2 гипервизоров. Кластеризация дает возможность создания и удаления виртуальных машин, а также разделения аппаратных мощностей.

2) Требуется наиболее производительное бесплатное open source-решение для виртуализации небольшой (20-30 серверов) инфраструктуры на базе Linux и Windows виртуальных машин.
Xen позволяет нескольким виртуальным машинам (ВМ) одновременно работать на одной физической машине, совместно используя ее аппаратные ресурсы. Каждая ВМ работает независимо и может запускать различные операционные системы, что делает Xen гибким и мощным решением для управления ресурсами сервера.

3) Необходимо бесплатное, максимально совместимое и производительное решение для виртуализации Windows-инфраструктуры.
Hyper-V — нативная (встроенная в ОС) платформа для аппаратной виртуализации, разработанная компанией Microsoft на основе Virtual PC, продукта дочерней компании Apple Connectix.

4) Необходимо рабочее окружение для тестирования программного продукта на нескольких дистрибутивах Linux.
VirtualBox — это программа, которая позволяет на одном компьютере запускать одновременно несколько операционных систем. Среди этих операционных систем могут быть Linux, Windows, Mac и другие.

Задача 4:
-
Опишите возможные проблемы и недостатки гетерогенной среды виртуализации (использования нескольких систем управления виртуализацией одновременно) и что необходимо сделать для минимизации этих рисков и проблем. Если бы у вас был выбор, создавали бы вы гетерогенную среду или нет?
Гетерогенная виртуальная среда — это виртуальная среда, в которой параллельно эксплуатируются несколько виртуальных платформ в рамках виртуальной среды одного предприятия. Недостатки использования таких сред – это наличие специалистов, затраты на обучение и взаимозаменяемость. Наличие регламентов по обслуживанию, резервному копированию и т.д. для данных систем. Желательно перейти на одну систему. Если не возможно отказаться, то разделить по задачам. Если была аттестация ГИС на данных системах, то придётся использовать те виртуальные платформы на которых они аттестовывались.
