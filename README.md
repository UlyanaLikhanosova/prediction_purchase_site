# Предсказание совершения покупки пользователем во время его сессии на сайте некоторого интернет-магазина

ML-модель, которая прогнозирует купит ли что-то клиент на сайте интернет-магазина, чтобы компания магазина могла внести исправления в сайт для повышения конверсии.

В качестве метода был использован RandomForestClassifier с подбором гиперпараметров, а также метод кластеризации KMeans с PCA для добавления новых признаков

Пример работы модели:

![Пример работы модели](https://github.com/UlyanaLikhanosova/prediction_purchase_site/blob/main/Results.JPG)


Данная работа была выполнена индивидуально.

## Содержание

- [Технологии](#технологии)

- [Инструкция](#инструкция)

- [Структура проекта](#структура-проекта)

- [Результаты](#результаты)

- [Контакты](#контакты)

## Технологии

- Python 3.13.5

- Библиотеки:

```python

pandas, numpy, scikit-learn, xgboost, matplotlib, seaborn 

```

- Данные: 12330 записей (Administrative, Administrative_Duration, Informational, ExitRates и др.)
## Инструкция

```

1. Клонируйте репозиторий:

```

git clone https://github.com/UlyanaLikhanosova/prediction_purchase_site.git

cd prediction_purchase_site

```

2. Установите зависимости:

```

pip install -r requirements.txt

```

3. Запустите Jupyter Notebook:

```

jupyter notebook notebooks/prediction_purchase_site.ipynb



## Структура проекта

```

prediction_purchase_site/

├── data/ # Исходные данные

│ └── online_shoppers_intention.csv

├── notebooks/ # Анализ и моделирование

│ └── prediction_purchase_site.ipynb

└── README.md # Этот файл

└── .gitignore

└── requirements.txt

└── Results.JPG

```

## Результаты

**Метрики модели RandomForestClassifier для клиентов, совершивших покупку:**

1. Precision 0.63 
2. F1-score 0.67 
3. Accuracy 0.89 
4. Recall 0.71

**Важные признаки**
1. PageValues
2. PCA_1
3. PCA_5
4. ExitRates
5. ProductRelated_Duration

Ключевые инсайты:

- Те кого заинтересовали товары, персональные предложения магазина и кто в целом внимательно изучает сайт с целью знакомства с магазином чаще покупают на сайте;

- Те кто просматривают страницы важные для конверсии, а также на них заканчивают, чаще совершают покупки.

## Контакты

Авторы: [Лиханосова Ульяна]

Email: likhanosova@yandex.ru
