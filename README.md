# OTUS_SA :sunglasses:
## :bowtie: Система управления видеоконтентом для наружной рекламы :bowtie:
- [Бизнес требования](#busines)
- [Определение предметной области](#predmet)
- [Определение требований](#treb)
- [Пользовательские истории](#us)
- [Информационная модель приложения](#imodel)
- [Проектирование структуры приложения](#proekt)
- [Примеры прототипов интерфейсов](#prototype)
- [Разработка API для управления воспроизведением](#api)
- [Acceptance Criteria для MVP](#ac)

<a name="busines"><h3>Бизнес требования к приложению</h3></a>
#### Цели проекта:
- **Увеличение прибыли и доходности:** Одной из основных целей автоматизированного показа рекламы может быть увеличение прибыли за счет дополнительного источника дохода, который представляет рекламный контент.
- **Повышение эффективности маркетинга:** Автоматизация позволяет более гибко управлять рекламными кампаниями, выбирать подходящее время и контекст для показа рекламы, что повышает ее эффективность и результативность.
- **Создание дополнительной ценности для партнеров и поставщиков:** Возможность показа рекламы в предприятиях общепита может привлечь дополнительных партнеров и поставщиков, заинтересованных в продвижении своих продуктов и услуг в этом сегменте рынка.
- **Сокращение затрат на персонал и ресурсы:** Автоматизация показа рекламы позволяет сократить затраты на персонал, так как не требуется постоянное управление и контроль над рекламными процессами.
- **Увеличение осведомленности о продукции и акциях:** Показ рекламы помогает повысить осведомленность клиентов о новинках, акциях и специальных предложениях, что может стимулировать повышение продаж и увеличение лояльности клиентов.
- **Адаптация рекламных роликов под аудиторию:** Автоматизация может позволить адаптировать рекламные ролики под конкретную аудиторию, учитывая её предпочтения и поведение.
- **Экономия времени и ресурсов:** Автоматизация позволяет сократить время и ресурсы, затрачиваемые на управление и контроль за процессом показа рекламы.
#### Критерии успеха
- MVP должен быть выпущен через шесть месяцев со старта разработки
- Выход на самоокупаемость приложения должен быть осуществлен в течение трех лет
- В течение года после выпуска MVP все 134 экрана должны перейти на данную систему
- Ожидаемое снижение транспортных расходов на 40% и сокращение штата обслуживающего персонала как минимум на треть.
#### Процессы которые требуют автоматизации:
* Возможность автоматически загружать контент на устройство.
* Возможность формирования плейлистов (управлять очерёдностью воспроизведения).
* Возможность удалённого просмотра проигрываемого контента.
* Возможность удалённого доступа к устройству.
* Ежемесячная аналитика проигрываемых видео с привязкой к экрану.
* Фильтрация по различным компаниям.
* Возможность вести статистику.

#### Бизнес требования:
|*№*|*Тема*|*Требование*|*Тип*|
| :- | :- | :- | :- |
||*Цель данного проекта*|*Получить приложение для автоматизации трансляции контента на экраны*|*Бизнес*|
||*Цель данного проекта*|*Предоставить конкурентноспособное приложение на рынке онлайн услуг*|*Бизнес*|
||*Как понять что проект успешен?*|*Окупаемость за 3 года*|*Бизнес*|
||*Как понять что проект успешен?*|*134 экранов работающих в приложении с функционалом MVP*|*Бизнес*|
||*Каков бюджет на разработку* |*Разработка MVP 3 млн*|*Бизнес*|
||*Каков срок разработки MVP*|*6 месяцев*|*Бизнес*|
||*Бюджет на поддержку* |*200 тыс. в месяц*|*Бизнес*|
||*Анализ конкурентов*|*Анализ конкурентов показал, отсутствие подобных сервисов с большим охватом разных рынков.*|*Бизнес*|

<a name="predmet"><h3>Определение предметной области</h3></a>
Наша компания занимается наружной рекламой, а также рекламой в кафе спорт залах и других местах проведения досуга граждан с использованием ЖК панелей с транслируемыми на них рекламными роликами. 
#### Текущие проблемные места:
* В заведениях партнёрах нет стандартизированной системы проигрывания роликов.
* Зачастую отсутствует возможность удалённого управления устройствами.
* Зачастую отсутствует возможность загрузки новых роликов в устройство.
* Отсутствует централизованная система мониторинга состояния устройств.
* Отсутствует возможность контролировать какой ролик играет в данный момент.
* Большие простои в виду отсутствие квалифицированного персонала на местах.
* Штат техников не справляется с парком устройств.
* Отсутствие документирования всех обслуживаемых объектов, что затрудняет их обслуживание и доставку контента.
#### Решение данных проблем:
* Стандартизированные устройства для проигрывания контента.
* Централизованная система управления устройствами.
* Централизованная система получения контента и формирования плейлистов.
* Система мониторинга состояния проигрывателей контента.
* Мониторинг проигрываемого контента.
* Удалённый доступ на все устройства.
* Система, объединяющая все устройства в единую сеть и позволяющая контент менеджерам и специалистам технического отдела выполнять свои функции максимально продуктивно.
* Гибкость системы, позволяющая оперативно добавлять в систему новые устройства, вне зависимости от инфраструктуры заказчика.
#### Предпосылки проекта и его необходимость:
* Клиент оплачивает трансляцию своего рекламного ролика в 10 заведениях по городу. Контент менеджер не может оперативно загрузить и начать транслировать ролики так как отсутствует возможность удалённо загрузить ролики и требуется ехать и загружать ролики вручную. Клиент заезжает в заведение и не видит своего рекламного ролика в плейлисте, соответственно начинаются разбирательства, которые ведут к убыткам и репутационным потерям.
* Сотрудник технической поддержки выезжает по заявке по «нерабочей приставке». В результате по приезду выяснилось, что не был включен телевизор, его включение является обязанностью персонала заведения. Следовательно специалист технической поддержки, не имея возможности удалённо проверить состояние устройства потратил время на проезд до заведения.
* Так же невозможно вести статистику о том сколько часов проигрывался тот или иной ролик на скольких экранах. Вся статистика ведётся в Excel или записывается на бумажке.

<a name="treb"><h3>Определение требований к системе</h3></a>
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

<a name="us"><h3>Пользовательские истории</h3></a>
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

<a name="imodel"><h3>Информационная модель приложения</h3></a>
#### Проектирование диаграммы классов
#### Основные сущности в системе управления проигрыванием видеоконтента включают:
- *Видеоролики* - файлы которые могут быть воспроизведены на рекламных панелях.
- *Рекламные панели* - они являются местом, где видеоролики воспроизводятся.
- *Пользователи* - они являются теми, кто управляет видеороликами и рекламными панелями, например, администраторы или операторы.
- *Плейлисты* - они определяют порядок воспроизведения роликов  на рекламных панелях, они формируются пользователями.
- *Настройки* - они включают параметры, такие как разрешение, частота кадров, сетевые настройки, настройки удалённого доступа.

#### На основе этих сущностей, мы можем спроектировать следующую диаграмму классов:

- *Класс Video:*
  Видеоролики имеют свойства, такие как название, длительность, размер и формат.
  Каждый видеоролик связан с одним или несколькими плейлистами.
  Видео могут иметь разные настройки.
- *Класс Panel:*
  Рекламные панели имеют свойства, такие как местоположение, размеры и разрешение. 
  Каждая рекламная панель может быть связана с одним или несколькими видеороликами.
  Рекламная панель имеет плейлисты, которые определяют время воспроизведения каждого связанного видеоролика.
  У каждой рекламной панели есть настройки, которые определяют ее параметры воспроизведения.
- *Класс User:*
  Пользователи имеют роли, такие как администраторы или операторы, и имеют соответствующие привилегии.
  Администраторы имеют доступ к управлению настройками, рекламными панелями и событиями.
  Операторы имеют доступ только к управлению списками воспроизведения.
- *Класс Playlist:*
  Плейлист имеют свойства, такие как дата начала, дата окончания и продолжительность, состав треков.
  Каждый плейлист связан  видеороликами и одной или несколькими рекламными панелями (в зависимости от того, сколько рекламных панелей воспроизводят этот плейлист).
- *Класс Setting:*
  Настройки имеют свойства, связанные с различными параметрами воспроизведения, такими как разрешение и частота кадров.
  Настройки связаны с рекламными панелями.
#### Диаграмма классов
![image5](https://github.com/AlexSterlev/OTUS_SA_2024/blob/main/Class-Diag.png)
<a name="proekt"><h3>Проектирование структуры приложения</h3></a>
#### Алгоритм добавления устройства в систему:
![image1](https://github.com/AlexSterlev/OTUS_SA_2024/blob/main/add_device.png)
#### Контекст-диаграмма (System context):
![image2](https://github.com/AlexSterlev/OTUS_SA_2024/blob/main/DiagComponent.png)
#### Компонент-диаграмма (Component):
![image3](https://github.com/AlexSterlev/OTUS_SA_2024/blob/main/DiagComponent2.png)
#### Разработка базы данных для функционирования сервиса:
![image4](https://github.com/AlexSterlev/OTUS_SA_2024/blob/main/BD_diag.jpg)
#### Описание таблиц Базы Данных:
- *Employees* – Таблица хранящая данные сотрудников.
- *Account* – Таблица хранящая данные для авторизации.
- *Responsible* – Таблица отвечающая за распределение устройств между пользователями линковачная таблица.
- *Devicegroup* – Информация о членствах устройств в группах.
- *Devicelist* – Информация об устройстве.
- *Rolelist* – Хранят информацию о ролях пользователей. 
- *Roleslinkposition* – линковочная между должностями и ролями.
- *Applications* – Описание  приложений. 
- *Rolelinkapplication* - приложения доступные для роли пользователя.
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
- Далее мы перешли в приложение управление плейлистами, в таблице аккаунта у нас хранится id сотрудника, по нему получаем список ему присвоенных устройств, а так же адреса и атрибуты устройств для дальнейшего отображения в личном кабинете.
```SQL
select DeviceGroup.GroupName, DeviceList.DeviceName, DeviceList.IPAddress, DeviceList.OtherText
  from account
	   inner join Responsible on Responsible.idemployee = account.idemployee
	   inner join DeviceGroup on DeviceGroup.IdGroupDevice = Responsible.IdGroupDevice
	   inner join DeviceList on DeviceList.IdDevice = Responsible.IdDevice
 where account.idaccount = 3
   and Responsible.IsDeleted = 0
 order by DeviceGroup.IdGroupDevice, DeviceList.IdDevice
```
<a name="prototype"><h3>Примеры прототипов интерфейсов</h3></a>
#### Окно авторизации пользователя:
![image5](https://github.com/AlexSterlev/OTUS_SA_2024/blob/main/Login.jpg)
#### Набор инструментов пользователей предоставляемый в зависимости от роли:
![image6](https://github.com/AlexSterlev/OTUS_SA_2024/blob/main/Apps.jpg)
#### Интерфейс управления плейлистами:
![image7](https://github.com/AlexSterlev/OTUS_SA_2024/blob/main/Management_playlist.jpg)
#### Интерфейс формирования плейлистов для дальнейшей загрузки на устройство или группу устройств:
![image8](https://github.com/AlexSterlev/OTUS_SA_2024/blob/main/Create_Playlist.jpg)
#### Интерфейс контент менеджера:
![image9](https://github.com/AlexSterlev/OTUS_SA_2024/blob/main/interface_manager.jpg)
#### Интерфейс специалиста технической потдержки:
![image10](https://github.com/AlexSterlev/OTUS_SA_2024/blob/main/Interface_it.jpg)

<a name="api"><h3>Разработка API для управления воспроизведением</h3></a>

* POST/playback/play - Начать воспроизведение
* POST/playback/pause - Приостоновить воспроизведение
* POST/playback/stop - Остановить вомпроизведение
* POST/playback/skip - Пропустить трек
* GET/playback/status - Статус воспроизведения
* POST/playback/playlist/add - Добавить плейлист
* POST/playback/playlist/remove - Удалить плейлист
* GET/playback/playlist - Запрос плейлиста

```YAML
openapi: 3.0.0
info:
  title: Media Player Control API
  version: '3.2'
  description: REST API for controlling playback of a media player and API authorization.
servers:
  # Added by API Auto Mocking Plugin
  - description: SwaggerHub API Auto Mocking
    url: https://virtserver.swaggerhub.com/SAN4EZSTERLEV/playback-control/3.2
  - url: https://api.example.com/v3
    description: Production server
  - url: https://api.staging.example.com/v3
    description: Staging server
components:
  securitySchemes:
    apiKey:
      type: apiKey
      in: header
      name: Authorization
paths:
  /playback/play:
    post:
      summary: Start playback
      security:
        - apiKey: []
      responses:
        '200':
          description: Playback started successfully
  /playback/pause:
    post:
      summary: Pause playback
      security:
        - apiKey: []
      responses:
        '200':
          description: Playback paused successfully
  /playback/stop:
    post:
      summary: Stop playback
      security:
        - apiKey: []
      responses:
        '200':
          description: Playback stopped successfully
  /playback/skip:
    post:
      summary: Skip to the next track
      security:
        - apiKey: []
      responses:
        '200':
          description: Track skipped successfully
  /playback/status:
    get:
      summary: Get the current playback status
      security:
        - apiKey: []
      responses:
        '200':
          description: Current playback status retrieved successfully
  /playback/playlist/add:
    post:
      summary: Add  playlist
      security:
        - apiKey: []
      requestBody:
        required: true
        content:
          application/json:
            schema:
              type: object
              properties:
                file_path:
                  type: string
      responses:
        '200':
          description: playlist added  successfully
  /playback/playlist/remove:
    post:
      summary: Remove playlist file  
      security:
        - apiKey: []
      requestBody:
        required: true
        content:
          application/json:
            schema:
              type: object
              properties:
                file_path:
                  type: string
      responses:
        '200':
          description: playlist removed successfully
  /playback/playlist:
    get:
      summary: Retrieve the current playlist
      security:
        - apiKey: []
      responses:
        '200':
          description: Current playlist retrieved successfully
```

<a name="ac"><h3>Acceptance Criteria для MVP</h3></a>

#### US001 Я как контент-менеджер хочу авторизоваться в системе что бы управлять и отслеживать проигрываемый контент.
%%- Пользователь должен иметь возможность ввести свои учетные данные (логин и пароль) на странице входа в систему.
- Система должна проверить введенные учетные данные и авторизовать пользователя, если они корректны.
- Пользователь должен быть авторизован только в случае, если его учетные данные совпадают с данными, хранящимися в базе данных системы.
- В случае некорректного ввода учетных данных, система должна выдать сообщение об ошибке и предложить пользователю повторно ввести данные.
- После успешной авторизации, пользователь должен иметь доступ к интерфейсу управления и отслеживания проигрываемого контента.
- Система должна обеспечивать безопасность данных и защиту от несанкционированного доступа к учетным данным других пользователей.
- Пользователь должен иметь возможность выйти из системы (разлогиниться), чтобы завершить текущую сессию работы с контентом.
- Система должна предоставлять механизм для отслеживания активности пользователя в системе, например, время последней активности или количество сеансов авторизации.
- В случае возникновения технических проблем или сбоев, система должна обеспечивать безопасное завершение текущей сессии пользователя и предотвращать потерю данных.
- Пользователь должен иметь возможность запросить восстановление доступа к своему аккаунту в случае утери или забытого пароля, с помощью механизма восстановления пароля по электронной почте.%%
#### US003 Я как контент менеджер хочу иметь возможность централизованно загружать плейлисты и видео в терминалы, для того что бы тратить меньше времени.
- Пользователь должен иметь доступ к интерфейсу управления контентом, где есть опция загрузки плейлистов и видео.
- Пользователь должен иметь возможность выбрать плейлист или видео файлы с локального компьютера или из облачного хранилища.
- Система должна поддерживать различные форматы видео файлов (например, MP4, AVI, MKV и т.д.) и плейлистов (например, M3U8).
- После выбора файлов пользователь должен иметь возможность указать терминалы, на которые нужно загрузить контент.
- Система должна обеспечивать возможность выбора нескольких терминалов для одновременной загрузки контента на несколько устройств.
- Пользователь должен получить уведомление о статусе загрузки каждого файла на каждый выбранный терминал, включая успешную загрузку, ошибки или проблемы с соединением.
- Система должна обеспечивать возможность отслеживания прогресса загрузки каждого файла на каждый выбранный терминал, включая оценочное время окончания загрузки.
- В случае возникновения ошибок или проблем в процессе загрузки, система должна предоставить информацию об ошибке и предложить возможные пути решения.
- Пользователь должен иметь возможность просматривать и редактировать загруженные плейлисты и видео файлы, а также удалять их при необходимости.
- Система должна обеспечивать безопасное хранение загруженных файлов и контроль доступа к ним для предотвращения несанкционированного доступа или удаления.
#### US006 Я как контент менеджер хочу иметь возможность просматривать в реальном времени видео которое воспроизводится на устройстве, для того что бы понимать корректность воспроизводимого контента.
- Пользователь должен иметь доступ к интерфейсу управления контентом, где есть опция просмотра видео в реальном времени.
- Пользователь должен иметь возможность выбрать устройство, на котором он хочет просматривать видео.
- Система должна обеспечивать установление соединения с выбранным устройством и передачу видео с него на интерфейс пользователя.
- Пользователь должен получить возможность просматривать видео в реальном времени без задержек или прерываний.
- Пользователь должен иметь возможность управлять воспроизведением видео (пауза, воспроизведение, перемотка) с интерфейса управления.
- Система должна предоставлять возможность отслеживать качество воспроизведения видео, включая разрешение, частоту кадров и качество звука.
- В случае возникновения проблем с воспроизведением видео (например, низкое качество, задержки, артефакты), система должна предоставить информацию об ошибке и возможные пути решения.
- Пользователь должен иметь возможность в реальном времени оценивать корректность воспроизводимого контента и принимать соответствующие меры по его исправлению или улучшению.
- Система должна обеспечивать безопасное и надежное соединение с устройством, чтобы предотвратить несанкционированный доступ к просматриваемому контенту или возможные угрозы безопасности данных.
#### US014 Я как техник хочу иметь возможность после настройки добавлять новые устройства в систему, чтобы после установки они появлялись в приложении для удалённого управления и контроля.
- Пользователь должен иметь доступ к интерфейсу управления устройствами, где есть опция добавления новых устройств в систему.
- Пользователь должен иметь возможность ввести информацию о новом устройстве, такую как его имя, описание, тип, серийный номер и другие параметры.
- Система должна проверять введенные пользователем данные на корректность и целостность.
- Пользователь должен иметь возможность сохранить информацию о новом устройстве в базе данных системы.
- После сохранения информации о новом устройстве, система должна обновить список устройств в приложении для удаленного управления и контроля, чтобы новое устройство было доступно для управления.
- Пользователь должен иметь возможность удалить или изменить информацию о добавленном устройстве в случае необходимости.
- При добавлении нового устройства в систему, система должна автоматически настроить его для подключения к сети и обеспечить его готовность к удаленному управлению.
- Пользователь должен получить уведомление об успешном добавлении нового устройства в систему и его готовности к удаленному управлению и контролю.
- Система должна обеспечивать защиту данных о новых устройствах и предотвращать несанкционированный доступ к ним или их настройкам.
#### US015 Я как техник хочу иметь возможность при добавлении устройства закрепить ответственного специалиста тех поддержки и контент-менеджера. Для полноценного внедрения его в инфраструктуру.
- Пользователь должен иметь доступ к интерфейсу управления устройствами, где есть опция добавления новых устройств в систему.
- При добавлении нового устройства, пользователь должен иметь возможность выбрать ответственного специалиста технической поддержки из списка существующих пользователей в системе.
- Пользователь также должен иметь возможность выбрать контент-менеджера из списка существующих пользователей в системе.
- Система должна проверять выбранных пользователей на доступность и корректность.
- После выбора ответственных специалистов, информация об устройстве должна содержать данные об ответственных специалистах технической поддержки и контент-менеджере.
- Информация об ответственных специалистах должна быть доступна для просмотра и редактирования через интерфейс управления устройствами.
- Система должна обеспечить возможность уведомления ответственных специалистов о назначении им устройства с указанием соответствующих деталей.
- Пользователь должен иметь возможность изменить ответственных специалистов для устройства в случае необходимости.
- Система должна обеспечить безопасность данных об ответственных специалистах и предотвращать несанкционированный доступ к ним или их изменение.
- Пользователь должен получить уведомление об успешном назначении ответственных специалистов для устройства.
#### US016 Я как техник хочу иметь возможность при добавлении устройства в систему вносить данные об устройстве, для того что бы контент менеджер и специалисты технической поддержки могли их идентифицировать.
- Пользователь должен иметь доступ к интерфейсу управления устройствами, где есть опция добавления новых устройств в систему.
- При добавлении нового устройства, пользователь должен иметь возможность вводить следующие данные:
- Название устройства, Описание устройства, включая модель, серийный номер, характеристики и другую информацию, необходимую для его идентификации.
- Местоположение устройства (например, адрес, помещение или зона).
- Технические характеристики устройства, если они применимы (например, IP-адрес, MAC-адрес, версия ПО и т.д.).
- Система должна проверять введенные пользователем данные на корректность и целостность.
- Пользователь должен иметь возможность сохранить информацию о новом устройстве в базе данных системы.
- После сохранения информации о новом устройстве, эта информация должна быть доступна для контент менеджера и специалистов технической поддержки.
- Контент менеджер и специалисты технической поддержки должны иметь возможность просматривать и обновлять данные об устройствах через соответствующий интерфейс в системе.
- В случае необходимости изменения данных об устройстве, пользователь должен иметь возможность вносить соответствующие изменения через интерфейс управления устройствами.
- Система должна обеспечивать безопасность данных об устройствах и предотвращать несанкционированный доступ к ним или их настройкам.


