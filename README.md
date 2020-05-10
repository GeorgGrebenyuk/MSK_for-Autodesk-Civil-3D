# MSK_for-Autodesk-Civil-3D
Сборник русских систем координат для AutoCAD Civil 3D (ок. 366 определений + вспомогательные файлы)
Файлы размещать в директории C:\Users\USER_NAME\AppData\Local\Autodesk\User Geospatial Coordinate Systems
Подробная информация по пакету содержится тут https://inj9.gitbook.io/msk-for-civil-3d/

Изменения:
13:05_08.05.2020
- убраны датумы и связанные с ними определения для ПЗ-90.11 (не нужны для работы программы)
- убраны преобразование USK-2000 to ITRS и датум USK-2000-1
- добавлены датумы для СК-42: EPSG:1254, EPSG:1267, уточнено что текуший датум "SK42_to_WGS84_GOST_32453-2017" равен формулировке EPSG:5044
- добавлены датумы для СК-95: EPSG:1281, уточнено что текуший датум "SK95_to_WGS84_GOST_32453-2017" равен формулировке EPSG:5043
- для СК-1963 принят датум EPSG:1267 (переход от СК-42 к WGS-84 образца 2001 года)
- для СК-63 добавлена зона U в числе 11 определений СК

19:50_29.04.2020
- скорректировано геодезическое преобразование SK-1963_to_WGS84 (неверное значение попраки для угла поворота по оси Z)
- изменен датум для СК-1964 г. Санкт-Петербург с СК-42 на СК-1963

0:17_25.04.2020
- переопределен датум для МСК-02 и МСК-50 с СК-42 на СК-95

4:00_23.03.2020
- добавлена примерная городская СК для г. Пермь и методические указания по настройке систем координат с аффинновыми преобразованиями

5:15_05.03.2020
- исправлена зона Х СК-1963 (неправильно было задано неверное северное смещение)
- добавлена категория "Ukraine Coordinate Systems"
- в состав систем координат для Украины внесены системы координат на основе СК-1963 - Зоны 1-6 с параметрами проекций, отличными от СК-1963, Зоны Х
- внесена система координат УСК-2000 с подзонами (4-7) и геодезическое трансформация от него до WGS-84, ETRS89 и ITRF2005 (фактически, также WGS-84) - эти параметры требуеют проверки на работоспособность
- в качестве датума для СК-1963 выбрана формулировка 	EPSG:1267 (https://epsg.io/1267); может быть уточнена пользователями

15:37_23.02.2020:
- исправлены осевые меридианы зоны L6_SK-1963
- добавлена городская система координат г. Екатеринбург "Russia-Town_EKB_var1" (System of Ekaterinburg)
- удалены географические системы координат из прежнего CK (Russia-SK42.LL), так как не несут никакой нагрузки
- удалены пути преобразования геодезических данных SK-42_to_WGS-84 по причине неработоспособности и в прцинипе излишества подстроиться под понимание Сивилом методики преобразования координат. Способ "SK42_to_WGS84_GOST_32453-2017" полностью рабочий и законный

5:11_19.02.2020:
- добавлены параметры перехода по ГОСТ 32453-2017 (двойная трансформация - преобразование от СК-42 (95) до WGS-84 через промежуточную трансформацию в ПЗ-90.11 пока не получается настроить чтобы было прямо по всем нормам из-за ошибок Civil 3D).
- уточнен состав зон 1963_W6
- исправлены рамки захвата карты для Республики Якутия (была избыточная площадь, и функция Геопозиционирования не работала)
- для Чукотского АО, двух последних зон карта исправлена на показ части справа от 180-меридиана, также для них добавлен отрицательный осевой меридиан (в силу условностей Civil 3D) - требуется тест чертежей в МСК для этих 2-ух зон
