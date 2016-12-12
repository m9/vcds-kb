
### 1. Тест стрелок
* Блок 17 -> Длинное кодирование -> Байт 1 -> Бит 0 (вкл)

### 2. Включение задних габаритов в режиме только ДХО
* Блок 09 -> Закрытая область (31347) -> Адаптация ->
* (6) — Tagfahrlicht — Dauerfahrlicht aktiviert zusaetzlich Standlicht auswählen -> Active

### 3. Отключение оповещения о не пристегнутом ремне
* Блок 17 -> Длинное кодирование -> Байт 0 -> Выбрать отключить оповещение (Бит 2-4)

### 4. Адаптация Hill Start Assistant !НЕ ПРОВЕРЕНО!
* Блок 03 -> Адаптация -> Berganfahrassistent -> Поменять значение на нужное вам

### 5. Отображает скорость вращения вентилятора в автоматическом режиме, на кондиционер
* Блок 08 -> Длинное кодирование -> Байт 11 -> Бит 6 (вкл)

### 6. Сохранение последнего набор сиденья стадии нагрева !НЕ ПРОВЕРЕНО!
* Блок 08 -> Адаптация ->
* Speicherung der Sitzheizungsstufe Fahrer — Aktiv
* Speicherung der Sitzheizungsstufe Beifahrer — Aktiv

### 7. Включение противотуманок при включении функции Coming home, Living home
* Блок 09 -> Закрытая область (31347) -> Адаптация ->
* (04) Comfort-Illumination — Coming Home Leuchten ->
Fog Light

### 8. Отключение ходовых огней в режиме "0" при поднятии ручника
* Блок 09 -> Закрытая область (31347) -> Адаптация ->
* (5) Tagfahrlicht — Dauerfahrlicht bei Handbremse abschalten — Aktiv

### 9. Звуковое сопровождение открытия и закрытия авто штатной сигналкой
* Блок 09 -> Закрытая область (31347) -> Адаптация ->
* (1) Rückmeldungssignale-Akustische Rückmeldung entriegeln auswählen — Aktiv
* (2) Rückmeldungssignale-Akustische Rückmeldung verriegeln auswählen — Aktiv
* (7)-Rückmeldungssignale-Menuesteuerung akustische Rückmeldung — Aktiv
* (8)-Rückmeldungssignale-Akustische Rückmeldung global — Aktiv

### 10. Включение функции складывания боковых зеркал удержанием кнопки закрытия дверей
* Блок 09 -> Закрытая область (31347) -> Адаптация ->
* (22)-Zugangskontrolle2-Funk Spiegelanklappen Modus -> by convenience operation

### 11. Изменение количества мигания поворотника в режиме обгона или перестроения (короткое нажатие на на рычаг поворотника)
* Блок 09 -> Закрытая область (31347) -> Адаптация ->
* (2) Turn signal control-Komfortblinken Blinkzyklen – выставляем нужно количество (5)

### 12. Светодиоды в подсветку номера (не будет выдавать ошибку)
* Блок 09 -> Закрытая область (31347) -> Адаптация ->
* (1)-Leuchte25KZL HA59-Lasttyp 25 (ставим 43)
* (6)-Leuchte25KZL HA59-Dimmwert AB 25 (ставим 127)

### 13. Увеличение интервала срабатывания омывателей фар
* Блок 09 -> Закрытая область (31347) -> Адаптация ->
* 1 канал (Windshield wiper –Anzahl) ставим 15

### 14. Увеличение времени срабатывания омывателей фар
* Блок 09 -> Закрытая область (31347) -> Адаптация ->
* 2 канал (Windshield wiper-SRA) ставим 150

### 15. Увеличение времени обогрева заднего стекла!НЕ ПРОВЕРЕНО!
* Блок 09 -> Закрытая область (31347) -> Адаптация ->
* 3 канал (Window heater) ставим 1200

### 16. Активация режима авторециркуляции печки: !НЕ ПРОВЕРЕНО!
* Блок 08 -> Длинное кодирование -> Байт 4 -> прописать 10

### 17. Брелок работает в зажигании !НЕ ПРОВЕРЕНО!
* Блок 09 -> Закрытая область (31347) -> Адаптация ->
* [LO]_Funk bei Klemme 15 ein — aktiv

### 18. Закрытие окон при дожде
У меня не работает
* Блок 09 -> Закрытая область (31347) -> Адаптация ->
* (15) Access Control 2 — Regenschliessen_ein aus (Rain Closing on / off) — aktiv
* (16) Access Control 2 — Regenschliessen_art (Rain closing Type) set to Permanent
* (28) Access Control 2 — Menuesteuerung Regenschliessen (Menu Control Rain close) – aktiv

### 19. TSC:
* Блок 44 -> Закрытая область (19249) -> Длинное кодирование -> Байт 0 -> Бит 2-3 выбрать with learned value

### 20. Выбор активного профиля вождения
* Блок 44 -> Закрытая область (19249) -> Длинное кодирование -> Байт 0 -> Бит 7 (вкл) Driving Profile Selection active
* Адаптация ->
* Characteristic curve of steering assistance — Dynamic
* Driving Profile switchover — Direct

### 21.Стартовая заставка магнитолы
* Блок 5F -> Длинное кодирование -> 18 байт -> 03
* Варианты:
* 03 — GTI, так же сменится машинка в меню Car
* 07 — R
* 02 — GTD
* 01 — Hybrid

### 21.5 Смена скина магнитолы и приборки
Магнитола
* Блок 5F -> Длинное кодирование -> 17 байт -> 02
Приборка(только MFA Premium)
* Блок 17 -> Адаптация->
* Displaydarstellung — Variante 2

### 22. Активация ESC Sport
ВНИМАНИЕ!
для активации у вас должен быть блок ABS с 30 байтным кодированием, иначе не трогайте
* Блок 03 -> Длинное кодирование -> 29 байт -> прописать
* 05 — даёт менюшки ESC ВКЛ, ASR выкл, ESC выкл.
* 06 или 08 — даёт менюшки ESC ВКЛ, ESC Sport, ESC выкл.
* 09 — даёт менюшки ESC ВКЛ, ASR выкл, ESC Sport
Чтобы, ESC не включалась обратно при скорости выше 100км/ч
* Адаптация ->
* ESP activation depending on speed — поставить activated

### 23. Стробоскопы
* Блок 09 -> Закрытая область (31347) -> Адаптация ->
**НОВЫЙ СПОСОБ**, предпочтительный
* driveng light and parking lightZahl der aktivern Sheinwerfer Auf 2 limitieren — aktiv

**СТАРЫЙ СПОСОБ**
* адаптация
* Leuchte12NL LB45
* Lichtfunktion C 12: Lichthupe generеll
* Dimmwert CD 12: 0
* Dimming Direction CD 12: minimize
далее
* Leuchte13NL RB5
* Lichtfunktion C 12: Lichthupe generеll
* Dimmwert CD 12: 0
* Dimming Direction CD 12: minimize

### 24. ДХО выключаются при ручнике
* Блок 09 -> Закрытая область (31347) -> Адаптация ->
* (5)-Tagfahrlicht-Tagfahrlicht Dauerfahrlicht bei Handbremse abschalten — Aktiv

### 25.Таймер круга.
Блок 17 -> Длинное кодирование -> Байт 01 -> Бит 3(вкл)

### 26. Отключение ДХО через меню
* Блок 09 -> Закрытая область (31347) -> Адаптация ->
* (2)-Daytime running lights-Tagfahrlicht Aktivierung durch BAD oder Bedienfolge möglich — Aktiv

### 27. Отключить старт-стоп, способ через температуру
* Блок 19 -> Адаптация ->
* (1)start/stop Au.Temperaturvorgabe-Minimaltemperatur -> -50 меняем на 50

### 28. Отключить омыватель фар
Блок 09 -> Длинное кодирование -> Адаптация -> Байт 13 -> Бит 3(выкл)

### 29. Просушка дисков
* Блок 03 -> Адаптация ->
* Disk drying -> выбрать нужное

### 30. Настройка порога скорости срабатывания ассистента дальнего света
* Блок A5 -> Адаптация ->
* Aktivierungsgeschwindigkeit für Fernlichtassistent (activation speed for high-beam assistant)
выставляем скорость (по умолчанию 57)

### 31.Режим работы стояночных огней
По умолчанию светится сторона, куда включен поворотник (или только левая, честно не знаю =))
Можно настроить тут
* Блок 09 -> Закрытая область (31347) -> Адаптация ->
* Driving Parking Light — Parklicht ueber LSS aktiviert ->
можно выбрать из списка режимы, я поставил USA, Canada, так горят обе стороны

з.ы. некоторые коды для блоков
* 31347 — 09
* 20103 + 40168 — 03,17
* 14117 = 13
* 27971 = 01
* 19249 = 44

