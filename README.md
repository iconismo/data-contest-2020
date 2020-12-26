# DataContest 2020, задача №5 "Определение основных принципов анализа и типологизации финансовых моделей деятельности ВУЗов"

## Постановка задачи
Проект выполнялся в рамках конкурса DataContest https://data-contest.ru. 

Цель - на основании анализа планов финансово-хозяйственной деятельности и финансовой отчетности проанализировать и типологизировать финансовые модели деятельности организаций высшего образования.

Подробнее https://github.com/Corporate-Accelerator-GenerationS/DataContest/issues/5

## Источники данных
- Реестр организаций, осуществляющих образовательную деятельность по аккредитованным образовательным программам http://obrnadzor.gov.ru/ru/opendata/7701537808-RAOO/
- Официальный сайт для размещения информации о государственных (муниципальных) учреждениях https://bus.gov.ru

## Основные этапы
1. Загрузка данных
2. Очистка данных
3. Вычисление корреляции финансовых показателей
4. Анализ аномальных значений
5. Масштабирование данных
6. Кластерный анализ
7. Интерпретация результатов

## Структура проекта
В соответствии с http://drivendata.github.io/cookiecutter-data-science/
├── LICENSE
├── Makefile           <- Makefile with commands like `make data` or `make train`
├── README.md          <- The top-level README for developers using this project.
├── data
│   ├── external       <- Data from third party sources.
│   ├── interim        <- Intermediate data that has been transformed.
│   ├── processed      <- The final, canonical data sets for modeling.
│   └── raw            <- The original, immutable data dump.
│
├── docs               <- A default Sphinx project; see sphinx-doc.org for details
│
├── models             <- Trained and serialized models, model predictions, or model summaries
│
├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
│                         the creator's initials, and a short `-` delimited description, e.g.
│                         `1.0-jqp-initial-data-exploration`.
│
├── references         <- Data dictionaries, manuals, and all other explanatory materials.
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures        <- Generated graphics and figures to be used in reporting
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
│
├── setup.py           <- Make this project pip installable with `pip install -e`
├── src                <- Source code for use in this project.
│   ├── __init__.py    <- Makes src a Python module
│   │
│   ├── data           <- Scripts to download or generate data
│   │   └── make_dataset.py
│   │
│   ├── features       <- Scripts to turn raw data into features for modeling
│   │   └── build_features.py
│   │
│   ├── models         <- Scripts to train models and then use trained models to make
│   │   │                 predictions
│   │   ├── predict_model.py
│   │   └── train_model.py
│   │
│   └── visualization  <- Scripts to create exploratory and results oriented visualizations
│       └── visualize.py
│
└── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io
