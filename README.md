# MSK_for-Autodesk-Civil-3D
Сборник русских систем координат для AutoCAD Civil 3D (ок. 366 определений + вспомогательные файлы)
Файлы размещать в директории C:\Users\USER_NAME\AppData\Local\Autodesk\User Geospatial Coordinate Systems
Подробная информация по пакету содержится тут https://inj9.gitbook.io/msk-for-civil-3d/

Изменения:
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
