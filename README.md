# H&M Personalized Fashion Recommendations - Pet Project

[![Python](https://img.shields.io/badge/Python-3.7+-blue.svg)](https://www.python.org/downloads/)
[![pandas](https://img.shields.io/badge/pandas-1.0+-green.svg)](https://pandas.pydata.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-0.23+-orange.svg)](https://scikit-learn.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

![image](https://github.com/user-attachments/assets/85952c79-040d-410e-9770-5c1ef590f777)


## Project Overview

This pet project is about developing a product recommendation system for H&M as part of Kaggle's "H&M Personalized Fashion Recommendations" competition. The goal of the project is to create a model that will recommend personally selected items from the H&amp;M catalog to customers based on historical transaction data as well as product and customer metadata.

**Task:**

Develop a recommendation system that predicts the top 12 products that a customer is likely to purchase in the future. The quality of recommendations is evaluated using the Mean Average Precision @ 12 (MAP@12) metric.

**Data used:**

The project uses data provided by H&M on Kaggle:

- `transactions_train.csv`: Shopper transaction history.
- `articles.csv`: Metadata about items (description, type, group, color, etc.).
- `customers.csv`: Metadata about customers (age, gender, membership status, etc.).
- `sample_submission.csv`: Sample submission file.

**Methods and models:**

The project includes the following steps:

1. **Exploratory Data Analysis (EDA)**:  Visualization and analysis of data to understand structure, distributions, and trends.
2. **Baseline Models (Baselines)**: Implementing simple recommendation models to compare and estimate the complexity of a task:
    - Recommendations based on recent purchases in a month.
    - Recommendations based on jointly purchased items.
3. **Alternating Least Squares (ALS) Collaborative Filtering Model**:  Using the ALS model to build personalized recommendations based on a matrix of user-good interactions.
    - Finding optimal hyperparameters (number of latent factors).
    - Evaluation of the model performance on a validation sample.
    - Generation of recommendations for submission.

**How to start the project:**

1. **Data Download:** You need to go to the competition page on Kaggle, download the data. “H&amp;M Personalized Fashion Recommendations” ([https://www.kaggle.com/competitions/h-and-m-personalized-fashion-recommendations/data](https://www.kaggle.com/competitions/h-and-m-personalized-fashion-recommendations/overview)). Place the downloaded CSV files in the project folder.
2. **Installing the libraries:** The Python libraries need to be installed. This can be done using pip, for example:
 
 pip install -r requirements.txt\
3. **Run files in Jupyter** Open the project file via JupyterLab or Jupyterhub and sequentially run the cells.\
4. **Change file paths** In the **Loading dataset** section of the notebook, change the **base_path** permenon to the actual path to the data downloaded from Kaggle in csv format.

## Обзор проекта

Этот pet-проект посвящен разработке системы товарных рекомендаций для H&M в рамках соревнования Kaggle "H&M Personalized Fashion Recommendations". Цель проекта - создать модель, которая будет рекомендовать покупателям персонально подобранные товары из каталога H&M, основываясь на исторических данных о транзакциях, а также метаданных о товарах и клиентах.

**Задача:**

Разработать рекомендательную систему, которая предсказывает топ-12 товаров, которые покупатель, вероятно, приобретет в будущем. Оценка качества рекомендаций производится с помощью метрики Mean Average Precision @ 12 (MAP@12).

**Использованные данные:**

Проект использует данные, предоставленные H&M на Kaggle:

- `transactions_train.csv`: История транзакций покупателей.
- `articles.csv`: Метаданные о товарах (описание, тип, группа, цвет и т.д.).
- `customers.csv`: Метаданные о клиентах (возраст, пол, статус членства в клубе и т.д.).
- `sample_submission.csv`: Пример файла submission.

**Методы и модели:**

Проект включает следующие этапы:

1. **Исследовательский анализ данных (EDA)**:  Визуализация и анализ данных для понимания структуры, распределений и трендов.
2. **Базовые модели (Baselines)**: Реализация простых рекомендательных моделей для сравнения и оценки сложности задачи:
    - Рекомендации на основе последних покупок за месяц.
    - Рекомендации на основе совместно покупаемых товаров.
3. **Модель коллаборативной фильтрации ALS (Alternating Least Squares)**:  Использование модели ALS для построения персональных рекомендаций на основе матрицы взаимодействий "пользователь-товар".
    - Поиск оптимальных гиперпараметров (количество латентных факторов).
    - Оценка производительности модели на валидационной выборке.
    - Генерация рекомендаций для submission.


**Как запустить проект:**

1. **Загрузка данных:** Необходимо зайти не страницу соревнования на Kaggle, скачать данные. "H&M Personalized Fashion Recommendations" ([https://www.kaggle.com/competitions/h-and-m-personalized-fashion-recommendations/data](https://www.kaggle.com/competitions/h-and-m-personalized-fashion-recommendations/overview)). Поместите скачанные CSV-файлы в папку с проектом.
2. **Установка библиотек:** Необходимо установить библиотеки Python. Это можно сделать, например при помощи pip: \
   pip install -r requirements.txt
3. **Запустить файлы в Jupyter** Открой файл проекта через JupyterLab или Jupyterhub и последовательной запускайте ячейки.
4. **Изменение путей к файлам** В секции тетрадки **Loading dataset** поменяйте пеерменную **base_path** на актуальный путь к данным, скачанным из Kaggle, в формате csv.
