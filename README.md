# MSK_for-Autodesk-Civil-3D
Сборник русских систем координат для AutoCAD Civil 3D
Файлы размещать в директории C:\Users\USER_NAME\AppData\Local\Autodesk\User Geospatial Coordinate Systems
Подробная информация по пакету содержится тут https://inj9.gitbook.io/msk-for-civil-3d/

Изменения:
5:11_19.02.2020:
- добавлены параметры перехода по ГОСТ 32453-2017 (двойная трансформация - преобразование от СК-42 (95) до WGS-84 через промежуточную трансформацию в ПЗ-90.11 пока не получается настроить чтобы было прямо по всем нормам из-за ошибок Civil 3D).
- уточнен состав зон 1963_W6
- исправлены рамки захвата карты для Республики Якутия (была избыточная площадь, и функция Геопозиционирования не работала)
- для Чукотского АО, двух последних зон карта исправлена на показ части справа от 180-меридиана, также для них добавлена отрицательный осевой меридиан (в силу условностей Civil 3D) - требуется тест чертежей в МСК для этих 2-ух зон
