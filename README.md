# Real Estate Exploratory Data Analysis
Elbrus Bootcamp | Phase-0 | Team project


## 🦸‍♂️Команда
1. [Антон Яблоков](https://github.com/AntNikYab)
2. [Вика Иванова](https://github.com/Vikaska031)
3. [Салман Чакаев](https://github.com/veidlink)
4. [Гриша Ржищев](https://github.com/Rzhischev)

## 🎯 Задача
Подготовить датасет для машинного обучения

## 📐 Ключевая метрика
Средняя абсолютная ошибка в процентах (MAPE). 
Улучшить значение MAPE с 50% до 30% и менее.

## 📚 Библиотеки 

```typescript

import re
import requests
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt

from geopy.exc import GeocoderTimedOut
from geopy.distance import geodesic
from geopy.geocoders import Nominatim

from tqdm import tqdm

from sklearn.preprocessing import OneHotEncoder
from sklearn.preprocessing import StandardScaler
```
	price

## 🧠 Выводы

После проведения очистки и преобразования данных исходного датасета было решено проанализировать корреляцию каждого из параметров с переменной ['Стоимость']. 
В результате были выбраны следующие параметры:

|feature|price_corr|
|---|---|
|eiling_height|	0.299|
|count_room|	0.582|
|area|	0.785|
|toilet_join_count|	0.393|
|shower_bath|	0.353|
|conditioner| 0.242|
|dishwasher| 0.354|
|parking_underground|	0.257|
|repair_designers| 0.288|
|repair_renovation_repair|	0.238|
|windows_courtyard_and_street_side_windows|	0.202|
|district_garden_ring|	0.465|
|district_mkad|	0.234|

В папке release ver 3.0 доступен полный файл корреляция.ipynb
