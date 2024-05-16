# Анализ продуктовых метрик мобильного приложения

## В данном проекте были поставлены следующие задачи:
- написать функцию для подсчета retention;
- при помощи А/B тестирования определить какой набор акционных предложений лучше.
Стек:
Python, Pandas, Seaborn, Scipy

## Применялись следующие подходы:
* когортный анализ
* А/Б тестирование
* bootstrap  
## Для выполнения поставленных задач были предприняты следующие шаги :
- выполнил проверку качества данных (пропущенные значения, количество строк);
- предобработал данные в датафрейме (перевод во временной формат);
- написал функцию, позволяющую сформировать *retention* по заданным параметрам: дата начала и конца для расчета *retention*;
- с помощью библиотеки seaborn визуализировал когортный анализ в виде графика;
- выполнил анализ двух групп, сформированных для проведения А/B тестирования, с помощью статистических тестов на нормальность распределения и статистическую значимость полученных результатов (Тесты Шапиро, Манна-Уитни, а также bootstrap)
- оценил, какие группы метрик необходимо анализировать в случае изменения механики игрового процесса
## Результаты
- по результатам исследования, можно предположить,что система плитования сработала некорректно;
- стоит применять новые функции на всех пользователей кроме випов, если система сплитования сработала корректно
