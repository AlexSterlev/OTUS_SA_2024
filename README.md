# OTUS_SA_2024
## Система управления видеоконтентом для наружной рекламы
### Определение предметной области
Наша компания занимается наружной рекламой, а также рекламой в кафе спорт залах и других местах проведения досуга граждан с использованием ЖК панелей с транслируемыми на них рекламными роликами. 
#### Текущие проблемные места:
* В заведениях партнёрах нет стандартизированной системы проигрывания роликов.
* Зачастую отсутствует возможность удалённого управления устройствами
* Зачастую отсутствует возможность загрузки новых роликов в устройство
* Отсутствует централизованная система мониторинга состояния устройств
* Отсутствует возможность контролировать какой ролик играет в данный момент
* Большие простои в виду отсутствие квалифицированного персонала на местах
* Штат техников не справляется с парком устройств
* Отсутствие документирования всех обслуживаемых объектов, что затрудняет их обслуживание и доставку контента
#### Решение данных проблем:
* Стандартизированные устройства для проигрывания контента.
* Централизованная система управления устройствами.
* Централизованная система получения контента и формирования плейлистов
* Система мониторинга состояния проигрывателей контента
* Мониторинг проигрываемого контента
* Удалённый доступ на все устройства
* Система, объединяющая все устройства в единую сеть и позволяющая контент менеджерам и специалистам технического отдела выполнять свои функции максимально продуктивно.
* Гибкость системы, позволяющая оперативно добавлять в систему новые устройства, вне зависимости от инфраструктуры заказчика.
#### Предпосылки проекта и его необходимость:
* Клиент оплачивает трансляцию своего рекламного ролика в 10 заведениях по городу. Контент менеджер не может оперативно загрузить и начать транслировать ролики так как отсутствует возможность удалённо загрузить ролики и требуется ехать и загружать ролики вручную. Клиент заезжает в заведение и не видит своего рекламного ролика в плейлисте, соответственно начинаются разбирательства, которые ведут к убыткам и репутационным потерям.
* Сотрудник технической поддержки выезжает по заявке по «нерабочей приставке». В результате по приезду выяснилось, что не был включен телевизор, его включение является обязанностью персонала заведения. Следовательно специалист технической поддержки, не имея возможности удалённо проверить состояние устройства потратил время на проезд до заведения.
* Так же невозможно вести статистику о том сколько часов проигрывался тот или иной ролик на скольких экранах. Вся статистика ведётся в Excel или записывается на бумажке.
#### Требования к функциональности проекта:
* Возможность автоматически загружать контент на устройство
* Возможность формирования плейлистов (управлять очерёдностью воспроизведения)
* Возможность удалённого просмотра проигрываемого контента
* Возможность удалённого доступа к устройству
* Ежемесячная аналитика проигрываемых видео с привязкой к экрану
* Фильтрация по различным компаниям
* Возможность вести статистику
#### Цели проекта:
- **Увеличение прибыли и доходности:** Одной из основных целей автоматизированного показа рекламы может быть увеличение прибыли за счет дополнительного источника дохода, который представляет рекламный контент.
- **Повышение эффективности маркетинга:** Автоматизация позволяет более гибко управлять рекламными кампаниями, выбирать подходящее время и контекст для показа рекламы, что повышает ее эффективность и результативность.
- **Создание дополнительной ценности для партнеров и поставщиков:** Возможность показа рекламы в предприятиях общепита может привлечь дополнительных партнеров и поставщиков, заинтересованных в продвижении своих продуктов и услуг в этом сегменте рынка.
- **Сокращение затрат на персонал и ресурсы:** Автоматизация показа рекламы позволяет сократить затраты на персонал, так как не требуется постоянное управление и контроль над рекламными процессами.
- **Увеличение осведомленности о продукции и акциях:** Показ рекламы помогает повысить осведомленность клиентов о новинках, акциях и специальных предложениях, что может стимулировать повышение продаж и увеличение лояльности клиентов.
- **Адаптация рекламных роликов под аудиторию:** Автоматизация может позволить адаптировать рекламные ролики под конкретную аудиторию, учитывая её предпочтения и поведение.
- **Экономия времени и ресурсов:** Автоматизация позволяет сократить время и ресурсы, затрачиваемые на управление и контроль за процессом показа рекламы.
### Определение требований
#### Нефункциональные требования:
<table><tr><th valign="top"><i>№</i></th><th valign="top"><i>Тема</i></th><th valign="top"><i>Требование</i></th><th valign="top"><i>Тип</i></th></tr>
<tr><td rowspan="3" valign="top">1</td><td rowspan="3" valign="top"><i>Технологический стек</i></td><td valign="top"><i>Разработка backend на Python,</i></td><td valign="top"><i>Нефункциональное</i></td></tr>
<tr><td valign="top"><i>Разработка front-end NODE, NEXT/React</i></td><td valign="top"><i>Нефункциональное</i></td></tr>
<tr><td valign="top"><i>Связь между клиентом и сервером WireGuard</i> </td><td valign="top"><i>Нефункциональное</i></td></tr>
<tr><td rowspan="4" valign="top">2</td><td rowspan="4" valign="top"><i>Безопасность</i></td><td valign="top"><i>Клиент должен взаимодействовать с сервером посредством протокола SSL</i></td><td valign="top"><i>Нефункциональное</i></td></tr>
<tr><td valign="top"><i>Требуется двухфакторная аутентификация</i></td><td valign="top"><i>Нефункциональное</i></td></tr>
<tr><td valign="top"><i>Отслеживание активности пользователя, при бездействии закрывать сессию с сохранением данных.</i></td><td valign="top"><i>Нефункциональное</i></td></tr>
<tr><td valign="top"><i>Требуется шифровать межсервисный трафик</i></td><td valign="top"><i>Нефункциональное</i></td></tr>
<tr><td valign="top">3</td><td rowspan="2" valign="top"><i>Совместимость</i></td><td valign="top"><p><i>Web-приложение должно поддерживать как мобильную версию для смартфонов, так и версию браузеров на ПК (Safari, Google Chrome, Яндекс Браузер, Mozila Firefox, Microsoft Edge, IE 11)</i></p><p></p></td><td valign="top"><i>Нефункциональное</i></td></tr>
<tr><td valign="top">4</td><td valign="top"><p><i>Приложение должно обеспечивать передачу данных с использованием шифрования</i></p><p></p></td><td valign="top"><i>Нефункциональное</i></td></tr>
<tr><td valign="top">5</td><td rowspan="2" valign="top"><i>Масштабируемость</i></td><td valign="top"><i>Решение должно поддерживать ежегодный рост на 30% новых терминалов</i></td><td valign="top"><i>Нефункциональное</i></td></tr>
<tr><td valign="top">6</td><td valign="top"><p><i>Решение должно поддерживать ежегодный рост на 25% от предыдущего количества транзакций.</i></p><p></p></td><td valign="top"><i>Нефункциональное</i></td></tr>
<tr><td valign="top">7</td><td valign="top"><i>Поддерживаемость:</i></td><td valign="top"><i>Обязательное логирование поведения приложения, авторизация пользователей, контроль учётных записей.</i></td><td valign="top"><i>Нефункциональное</i></td></tr>
<tr><td valign="top">8</td><td valign="top"><i>Требования к модульности приложения:</i></td><td valign="top"><i>Инфраструктура, поддерживающая сервис должна состоять из следующих модулей: БД, сервер приложений, клиентский веб интерфейс.</i></td><td valign="top"><i>Нефункциональное</i></td></tr>
<tr><td valign="top">9</td><td rowspan="2" valign="top"><i>Производительность:</i></td><td valign="top"><i>Хранилище данных рассчитывается на 4гб на одно устройство</i></td><td valign="top"><i>Нефункциональное</i></td></tr>
<tr><td valign="top">10</td><td valign="top"><i>Пиковое значение 200 подключённых устройств одновременно</i></td><td valign="top"><i>Нефункциональное</i></td></tr>
<tr><td valign="top">11</td><td rowspan="2" valign="top"><i>Доступность:</i></td><td valign="top"><p><i>Сервис должен быть доступен 95% времени с территории РФ.</i></p><p></p></td><td valign="top"><i>Нефункциональное</i></td></tr>
<tr><td valign="top">12</td><td valign="top"><i>Режим работы 24/7</i></td><td valign="top"><i>Нефункциональное</i></td></tr>
</table>

#### MVP:
<table><tr><th valign="top"><i>№</i></th><th valign="top"><i>Тема</i></th><th valign="top"><i>Требование</i></th><th valign="top"><i>Тип</i></th></tr>
<tr><td rowspan="6" valign="top"></td><td rowspan="6" valign="top"><i>Функционал MVP</i></td><td valign="top"><i>Регистрация пользователей в системе</i></td><td valign="top"><i>Функциональное</i></td></tr>
<tr><td valign="top"><i>Разграничение доступа к устройствам</i></td><td valign="top"><i>Функциональное</i></td></tr>
<tr><td valign="top"><i>Загрузка данных в устройства</i></td><td valign="top"><i>Функциональное</i></td></tr>
<tr><td valign="top"><i>Удалённое управление устройством</i></td><td valign="top"><i>Функциональное</i></td></tr>
<tr><td valign="top"><i>Удалённое управление воспроизведением</i></td><td valign="top"><i>Функциональное</i></td></tr>
<tr><td valign="top"><i>Добавление устройств в систему</i></td><td valign="top"><i>Функциональное</i></td></tr>
<tr><td valign="top"></td><td valign="top"><i>Планируемый охват аудитории (MVP)</i></td><td valign="top"><i>Все менеджеры компании в течении полугода перейдут на данную систему</i></td><td valign="top"><i>Бизнес</i></td></tr>
<tr><td rowspan="4" valign="top"></td><td rowspan="4" valign="top"></td><td valign="top"><i>1 года окупаемость.</i></td><td valign="top"><i>Бизнес</i></td></tr>
<tr><td valign="top"><i>Через год планируем продавать доступ к сервису  и аренду устройств по франшизе</i></td><td valign="top"><i>Бизнес</i></td></tr>
<tr><td valign="top"><i>За 6 месяца (MVP) требуется уменьшить штат и транспортные расходы  вдвое.</i></td><td valign="top"><i>Бизнес</i></td></tr>
<tr><td valign="top"></td><td valign="top"></td></tr>
</table>

#### Бизнес требования:
|*№*|*Тема*|*Требование*|*Тип*|
| :- | :- | :- | :- |
||*Цель данного проекта*|*Получить приложение для автоматизации трансляции контента на экраны*|*Бизнес*|
||*Цель данного проекта*|*Предоставить конкурентноспособное приложение на рынке онлайн услуг*|*Бизнес*|
||*Как понять что проект успешен?*|*Окупаемость за 1год*|*Бизнес*|
||*Как понять что проект успешен?*|*134 экранов работающих в приложении с функционалом MVP*|*Бизнес*|
||*Каков бюджет на разработку* |*Разработка MVP 3 млн*|*Бизнес*|
||*Каков срок разработки MVP*|*3 месяца*|*Бизнес*|
||*Бюджет на поддержку* |*200 тыс. в месяц*|*Бизнес*|
||*Анализ конкурентов*|*Анализ конкурентов показал, отсутствие подобных сервисов с большим охватом разных рынков.*|*Бизнес*|

#### Пользовательские истории:
|US001|Я как контент-менеджер хочу авторизоваться в системе что бы управлять и отслеживать проигрываемый контент|must|контент-менеджер|mvp|На сайте сервиса отображается форма, регистрации. В базе данных после регистрации появилась учётная запись пользователя.|
| :- | :- | :- | :- | :- | :- |
|US002|Я как специалист технической поддержки хочу авторизоваться в системе, чтобы иметь удалённый доступ к терминалам устройств, для решения проблем технического характера. |must|специалист технической поддержки||На сайте сервиса после регистрации, при выборе доступного устройства отображается кнопка SSH, при нажатии на неё мы получаем доступ к консоли устройства.|
|US003|Я как контент менеджер хочу иметь возможность централизованно загружать плейлисты и видео в терминалы, для того что бы тратить меньше времени|must|контент-менеджер|mvp|На сайте сервиса после регистрации, при выборе доступных устройств по средствам чекбокса, появляется кнопка загрузить данные|
|US004|Я как контент менеджер хочу иметь возможность группировать терминалы по различным признакам, что бы загружать один плейлист для группы терминалов|should|контент-менеджер||На сайте сервиса после регистрации, при выборе доступных устройств по средствам чекбокса, появляется кнопка группировать|
|US005|Я как контент менеджер хочу иметь возможность просматривать плейлист который в данный момент проигрывает терминал, для осуществления контроля за контентом|should|контент-менеджер||На сайте сервиса после регистрации, при выборе доступного устройства отображается кнопка «Плейлист»|
|US006|Я как контент менеджер хочу иметь возможность просматривать в реальном времени видео которое воспроизводится на устройстве, для того что бы понимать корректность воспроизводимого контента|should|контент-менеджер|mvp|На сайте сервиса после регистрации, при выборе доступного устройства отображается кнопка «Играет сейчас»|
|US007|Я как контент менеджер хочу иметь возможность просматривать список видеофайлов загруженных на устройство, что бы контролировать целостность загруженного контента на устройство|should|контент-менеджер||На сайте сервиса после регистрации, при выборе доступного устройства отображается кнопка  «файлы»|
|US008|Я как специалист технической поддержки хочу видеть статус устройства в сети, онлайн/оффлайн, чтобы понимать находится устройство в сети или требуется выезд|should|специалист технической поддержки||На сайте сервиса после регистрации, на против каждого доступного устройства горит пиктограмма со статусом красного/зелёного в зависимости от статуса.|
|US009|Я как специалист технической поддержки хочу иметь доступ к параметрам устройства (утилизация процессора и оперативной памяти, загрузка сети, свободное место на диске, температура), для проведения диагностических мероприятий|should|специалист технической поддержки||На сайте сервиса после регистрации, при выборе доступного устройства отображается кнопка  «Ресурсы»|
|US010|Я как специалист технической поддержки хочу иметь доступ к просмотру лог файлов через web интерфейс, для проведения диагностических мероприятий|should|специалист технической поддержки||На сайте сервиса после регистрации, при выборе доступного устройства отображается кнопка  «Логи»|
|US011|Я как специалист технической поддержки хочу иметь возможность выгружать логи в файл, чтобы отправлять диагностическую информацию другим специалистам|should|специалист технической поддержки||На сайте сервиса после регистрации, при выборе доступного устройства отображается кнопка  «Логи», при нажатии на неё мы получаем доступ к просмотру лог файла, в правом верхнем углу окна имеется кнопка «закгрузить лог файл» при нажатии на которую лог файл загружается на локальный компьютер|
|US012|Я как специалист технической поддержки хочу иметь возможность просматривать информацию о местоположении устройства, чтобы в случае невозможности решить проблему удалённо, направить технического специалиста.|should|специалист технической поддержки||На сайте сервиса после регистрации, при выборе доступного устройства отображается кнопка  «Детали», при нажатии которой к отображается местоположение на карте заведения где стоит устройство. |
|US013|Я как контент менеджер хочу иметь возможность формировать плейлисты, чтобы видеофайлы проигрывались в нужном мне порядке|should|контент-менеджер||На сайте сервиса после регистрации, доступно вкладка «сформировать плейлист».|
|US014|Я как техник хочу иметь возможность после настройки добавлять новые устройства в систему, чтобы после установки они появлялись в приложении для удалённого управления и контроля.|must|техник|mvp|На сайте сервиса после регистрации, доступно вкладка «Добавить устройство».|
|US015|Я как техник хочу иметь возможность при добавлении устройства закрепить ответственного специалиста тех поддержки и контент-менеджера. Для полноценного внедрения его в инфраструктуру. ||техник|mvp|После добавления устройства, доступна кнопка «передать устройство»|
|US016|Я как техник хочу иметь возможность при добавлении устройства в систему вносить данные об устройстве, для того что бы контент менеджер и специалисты технической поддержки могли их идентифицировать|must|техник|mvp|После добавления устройства, при нажатии кнопки доступна кнопка «Детали»|
|US017|Я как контент менеджер хочу иметь возможность просматривать статистику, для получения  аналитических данных.|should|контент-менеджер||На сайте сервиса после регистрации, доступна вкладка статистика.|

### Проектирование структуры приложения
#### Алгоритм добавления устройства в систему:
![image1](https://github.com/AlexSterlev/OTUS_SA_2024/blob/main/add_device.png)
#### Контекст-диаграмма (System context):
![image2](https://github.com/AlexSterlev/OTUS_SA_2024/blob/main/DiagComponent.png)
#### Компонент-диаграмма (Component):
![image3](https://github.com/AlexSterlev/OTUS_SA_2024/blob/main/DiagComponent2.png)
#### Разработка базы данных для функционирования сервиса:
![image4](https://github.com/AlexSterlev/OTUS_SA_2024/blob/main/BD_diag.jpg)
#### Описание таблиц Базы Данных
#### Примеры работы запросов Базы данных:
- Например из сервиса приходит запрос с логином и паролем. по такому запросу, мы можем получить данные сотрудника, который авторизовался. Так же мы получим его *accountId*, который уже в другие запросы сможем передавать.
```SQL
select employees.description, position.description, account.idaccount
  from employees
       inner join account on account.idemployee = employees.idemployee
	   inner join position on position.idposition = employees.idposition
 where employees.DateBeginWork <= now()
   and (employees.DateEndWork >= now() or employees.DateEndWork is null)
   and account.password = md5('vozduhonelove')
   and account.login = 'vozdushniyca'
```
- После успешной авторизации, мы получаем список приложений доступные этому аккаунту, по аккаунту получаем данные сотрудника, его должность; По должности получаем список ролей, по ролям получаем список доступных для роли приложений.
```SQL
select Applications.Description
  from account
  	   inner join employees on employees.idemployee = account.idemployee
       inner join RolesLinkPosition on RolesLinkPosition.idposition = employees.idposition
	   inner join RolesLinkApplications on RolesLinkApplications.IdRoles = RolesLinkPosition.IdRoles
	   inner join Applications on Applications.IdApplications = RolesLinkApplications.IdApplications
 where account.idaccount = 3
   and employees.DateBeginWork <= now() 
   and (employees.DateEndWork >= now() or employees.DateEndWork is null)
   and RolesLinkPosition.IsDeleted = 0
order by Applications.IdApplications
```
