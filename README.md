# Лабораторная работа №3: Работа с базой данных

## Выполнил: Королев Федор ИСП-221с  
**Язык программирования:** Java  

---

## Описание  
Приложение представляет собой Android-приложение с двумя активностями, работающее с базой данных SQLite.  

### Активность 1 (activity_main.xml)  
Содержит три кнопки для взаимодействия с таблицей **«Одногруппники»**:  
1. **Показать одногруппников**  
   - Открывает вторую активность, где отображаются все записи таблицы.  
2. **Добавить запись**  
   - Добавляет новую запись.  
3. **Обновить последнюю запись**  
   - Обновляет данные в последней записи таблицы, заменяя ФИО на «Иванов Иван Иванович».  

### Активность 2 (activity_student_list)  
Отображает данные из таблицы **«Одногруппники»** в табличном формате:  
- **ID** — уникальный идентификатор записи.  
- **Фамилия** — фамилия студента.  
- **Имя** — имя студента.  
- **Отчество** — отчество студента.  
- **Время добавления записи** — дата и время создания записи в формате `yyyy-MM-dd HH:mm:ss`.  

---

## Задания  

### Задание 1  
На первом экране реализованы следующие функции:  
1. **Создание базы данных:**  
   - При первом запуске создается база данных, если она отсутствует.  
   - Создается таблица **«Одногруппники»** с полями:  
     - `ID`  
     - `ФИО`  
     - `Время добавления записи`.  
   - Удаляются все существующие записи.  
   - В таблицу добавляются 5 начальных записей.  
2. **Добавление записи:**  
   - При нажатии на кнопку **«Добавить запись»** добавляется новая строка с фиктивными данными.  
3. **Обновление последней записи:**  
   - При нажатии на кнопку **«Обновить последнюю запись»** обновляется последняя строка, заменяя ФИО на «Иванов Иван Иванович».  
4. **Просмотр записей:**  
   - При нажатии на кнопку **«Показать записи»** открывается второй экран, где выводятся данные из таблицы.  

---

## Пример использования  
1. Запустите приложение.  
2. Нажмите на кнопку **«Показать одногруппников»**, чтобы просмотреть записи.  
3. Добавьте новую запись, нажав **«Добавить запись»**.  
4. Обновите последнюю запись, выбрав **«Обновить последнюю запись»**.  
