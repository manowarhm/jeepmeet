# jeepmeet
jeepmeet project

Структура данных "Мероприятие"

1. № п\п 
1 - counter 
2 - только натуральные числа > 0, c шагом +1
3 - числовой, (number)
4 - нет
------------------------
2. Название мероприятия
1 - event
2 - строковая переменная с ограничением, допустим, 300 символов
3 - строка, (string)
4 - есть 
------------------------
3. Вид соревнования (спринт \ триал \ ралли \ ориентирование)
1 - view_competition
2 - не может быть числом (натуральным \ дробным)
3 - массив (array) или если брать TS, то можно использовать кортеж. Хотя лучше массив
4 - есть 
------------------------
4. Место проведения (область, район, город\поселок)
1 - location
2 - только текстовые значения, не может быть числом
3 - массив (array)
4 - location_region
   - location_region_area
   - location_region_area_town
Лучше создать отдельные таблицы связанные с этой, по типу: 
  - (область (location_region)
  - (район (location_region_area)
  - (город\поселок (location_region_area_town)
------------------------
5. Время проведения
1 - date
2 - не может быть, числом, строкой, контроль формата даты 
3 - если присутствует такой тип, то: время (date), а так числовой (number)
4 - есть 
------------------------
6. Координаты
1 - coordinates 
2 - не может быть строкой, запись в строгой форме в зависимости от выбора системы координат (или) формат записи: градусы, минуты, секунды формата hddd.mm.mmm - числовой.
3 - числовой
4 - есть
------------------------
7. Категории для участия (ATV, Standart, TP-0, TP-1, TP-2, TP-3, Proto)
1 - categories 
2 - не может быть числом
3 - массив (array)
4 - есть 
------------------------
8. Ограничения 
1 - restrictions
2 - не может быть числом
3 - текстовый (string)
4 - есть (отдельная таблица с ограничениями)
------------------------
9. Стоимость взноса за участие
1 - how_much
2 - не может быть строкой
3 - числовой (number)
4 - нет
------------------------

1) Имя
2) Ограничения
3) Тип данных
4) Связь с другими

