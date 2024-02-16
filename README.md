<!--###### -

### [***`Coдержание`***](#-) :<br>

 - [***Краткое описание проекта***](#Краткое-описание-проекта)
 
 - [***Цель проекта***](#Цель-проекта)
 
 - [***Ключевые задачи***](#Ключевые-задачи)
 
 - [***Ссылка на проект***](https://github.com/IvanoVladimir/karpov_courses/blob/main/Final_project/Mobile_games.ipynb 'Ссылка на проект')

-----> 

### [***`Краткое описание`***](#-)<br>

**Название:** *Mobile games*

**Стэк:**

[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-424242?style=for-the-badge&logo=Jupyter&logoColor=BA7400)](https://jupyter.org/)
[![Python](https://img.shields.io/badge/python-1C648D?style=for-the-badge&logo=python&logoColor=ffdd54)](https://www.python.org/)
[![Datetime](https://img.shields.io/badge/Datetime-1C648D?logo=Datetime&logoColor=ffdd54&style=for-the-badge)](https://docs.python.org/3/library/datetime.html)
[![urllib.parse](https://img.shields.io/badge/urllib.parse-1C648D?logo=urllib.parse&logoColor=ffdd54&style=for-the-badge)](https://docs.python.org/3/library/urllib.parse.html)
[![os](https://img.shields.io/badge/os-1C648D?logo=os&logoColor=ffdd54&style=for-the-badge)](https://docs.python.org/3/library/os.html)
[![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Numpy](https://img.shields.io/badge/Numpy-00232B.svg?style=for-the-badge&logo=Numpy&logoColor=00A9D2)](https://numpy.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-00B1DC?logo=matplotlib&logoColor=white&style=for-the-badge)](https://matplotlib.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-0E174A?logo=seaborn&logoColor=white&style=for-the-badge)](https://seaborn.pydata.org/)
[![Pingouin](https://img.shields.io/badge/Pingouin-000000?logo=Pingouin&logoColor=white&style=for-the-badge)](https://pingouin-stats.org/build/html/index.html)
[![Requests](https://img.shields.io/badge/Requests-2E2E2E?logo=Requests&logoColor=white&style=for-the-badge)](https://requests.readthedocs.io/en/latest/index.html)
[![Scipy](https://img.shields.io/badge/Scipy-00232B?logo=Scipy&logoColor=0052BA&style=for-the-badge)](https://scipy.org/)
[![Stats](https://img.shields.io/badge/Stats-00232B?logo=Stats&logoColor=0052BA&style=for-the-badge)](https://docs.scipy.org/doc/scipy/reference/stats.html)

---

### [***`Цель`***](#-)<br>
 
**Изучив имеющиеся данные мобильного приложения рассчитать показатель *Retention*, определить наилучшее акционное предложение по результатам A/B тестирования и предложить метрики для оценки результатов последнего прошедшего тематического события в игре.**

---

### [***`Этапы выполнения`***](#-)<br>
 
1. Произвёл считывание данных, провёл предварительный анализ и предобработку данных
2. Написал формулу расчёта *Retention*, а также функцию со множеством параметров и пояснения к ним, а также добавил визуализацию
3. По Api получил данные результатов последнего A/B тестирования
4. Проверил не оказались ли пользователи случайно в обеих группах
5. Посмотрел описательную статистику, а также распределения выручки по активным и платящим пользователям
6. Выбрал метрики(*CR, ARPU*) и написал их определение
7. Посчитал Conversion rate в каждой группе и нашёл процентную разницу между ними
8. Выбрал статистический тест(*Хи-квадрат*) и определил есть ли статистичеси значимое различие между группами
9. Посчитал Average revenue per user в каждой группе и нашёл процентную разницу между ними
10. Проверил распределения на нормальность и гомогенность
11. На основании полученных результатов выбрал статистически тест(*Т-теста Стьюдента*)
12. Подвёл итоги по результатам тестов выбранных метрик, сделал выводы
13. Предложил следующие метрики(*ASD, Stickiness, Retention rate, Churn rate, Game Ready API* и т.д)
14. Написал определения и пояснения к ним, а также изложил свои мысли, как поменяются метрики, если усложнить механику прохождения

---

### [***`Результаты`***](#-)<br>

* Написал сложную функцию с описанием и визуализацией для расчёта *Retention* формирующую когорты по множеству параметрам:
  * даты начала и окончания формирования когорт;
  * размеры когорт по(дням, неделям, месяцам, кварталам, годам);
  * временной интервал для расчета(день, неделя, месяц, год) и количество периодов
* По итогам A/B тестирования получил:
  * Конверсию в покупку контрольной группы **выше на ~7.1%**, результат статистически значим.
  * *ARPU* тестовой группы **выше на ~5.3 %**, результат статистически не значим.
  * **Вывод:** считаю, что набор акционных предложений для контрольной группы оказался лучше, хотя и есть некоторые сомнения по поводу корректности проведения A/B теста, а именно системы сплитования(предположение)
* Выбрал метрики для оценки результатов последнего прошедшего тематического события игры и выдвинул свои предположения, как поменяются метрики, если усложнить механику событий так, что при каждой неудачной попытке выполнения уровня
игрок будет откатываться на несколько уровней назад

---

## [***К проекту***](https://github.com/IvanoVladimir/MobileApp/blob/main/Mobile_games.ipynb 'Ссылка на проект') 
<!--## [***К содержанию ->***](#-)-->
<div id="badges" align="center">

<!-- [![GitHub last commit](https://img.shields.io/github/last-commit/IvanoVladimir/E-commerce.svg)](https://github.com/IvanoVladimir/E-commerce) 
[![GitHub commit activity the past week, 4 weeks, year](https://img.shields.io/github/commit-activity/y/IvanoVladimir/E-commerce.svg)](https://github.com/IvanoVladimir/E-commerce)--> 
[![GitHub repo size in bytes](https://img.shields.io/github/repo-size/IvanoVladimir/E-commerce.svg)](https://github.com/IvanoVladimir/E-commerce)
![ViewCount](https://views.whatilearened.today/views/github/IvanoVladimir/E-commerce.svg?cache=remove)
![GitHub top language](https://img.shields.io/github/languages/top/IvanoVladimir/E-commerce.svg?style=flat)

</div>
