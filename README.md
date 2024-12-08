Лабораторные работы по курсу "Методы, средства и технологии мультимедиа"
Студент: Русаков Александр Владиславович
Группа: М8О-410Б-21

Выполненные лабораторные работы №1-5 находятся в файле [multimedia.ipynb](https://github.com/mx4alex/Multimedia/blob/main/multimedia.ipynb)

Были получены следующие результаты при использовании метрик Accuracy для задачи классификации и R2-score для задачи регрессии на тестовых наборах данных:

| Алгоритм            | Задача            | Бейзлайн           | Улучшенный бейзлайн | Самостоятельная имплементация алгоритма |
|---------------------|-------------------|--------------------|---------------------|--------------------------------------|
| KNN                 | Классификация     | 0.884259           | 0.928241            | 0.872832                             |
|                     | Регрессия         | 0.589127           | 0.591984            | 0.595362                             |
| Линейные модели     | Классификация     | 0.662037           | 0.682870            | 0.812138                             |
|                     | Регрессия         | 0.502250           | **0.864627**        | 0.864627                             |
| Решающее дерево     | Классификация     | 0.967593           | 0.967593            | 0.959537                             |
|                     | Регрессия         | 0.711365           | 0.619319            | 0.724721                             |
| Случайный лес       | Классификация     | 0.951389           | 0.951389            | 0.973988                             |
|                     | Регрессия         | 0.792813           | 0.818482            | 0.773095                             |
| Градиентный бустинг | Классификация     | 0.969907           | **0.990741**        | 0.852601                             |
|                     | Регрессия         | 0.696458           | 0.782312            | 0.782331                             |

Остальные данные с другими метриками представлены в файле [multimedia.ipynb](https://github.com/mx4alex/Multimedia/blob/main/multimedia.ipynb).

Вывод: улучшение бейзлайна позволило значительно повысить точность почти всех моделей, при этом наилучшие показатели для задачи классификации выявлены у градиентного бустинга, а для задачи регрессии - у линейных моделей. Также было получено, что для некоторых моделей самостоятельная имплементация алгоритма показывала лучшие результаты по сравнению с моделями из sklearn.
