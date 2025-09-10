# 🚕 Прогнозирование заказов такси (Forecasting Taxi Orders)

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green)
![LightGBM](https://img.shields.io/badge/LightGBM-Gradient%20Boosting-yellow)
![TimeSeries](https://img.shields.io/badge/TimeSeries-Forecasting-red)

Прогнозирование количества заказов такси на следующий час для оптимизации работы службы такси и привлечения водителей в периоды пиковой нагрузки.

## 🎯 О проекте

Проект посвящен разработке модели машинного обучения для прогнозирования спроса на услуги такси. На основе исторических данных о заказах такси в аэропортах строится модель, способная предсказать количество заказов на следующий час с высокой точностью.

**Ключевые особенности:**
- 📈 Анализ временных рядов с выявлением трендов и сезонности
- 🛠️ Создание комплексных признаков (лаги, скользящие статистики)
- 🤖 Сравнение нескольких ML-моделей
- ⚙️ Оптимизация гиперпараметров с временной кросс-валидацией
- 🎯 Достижение целевой метрики RMSE < 48

## 📊 Результаты

**Лучшая модель:** LightGBM Regressor  
**Метрика RMSE на тесте:** 42.17 ✅  
**Целевая метрика:** ≤ 48  

**Параметры лучшей модели:**
```python
LGBMRegressor(
    max_depth=9,
    n_estimators=78, 
    num_leaves=9,
    objective='regression', 
    random_state=42,
    metric='rmse'
)

🛠️ Технологический стек
Python 3.8+ - основной язык разработки

Pandas - обработка и анализ временных рядов

NumPy - математические операции

Scikit-learn - ML модели и preprocessing

LightGBM - градиентный бустинг для временных рядов

Matplotlib/Seaborn - визуализация данных

Statsmodels - анализ временных рядов

Jupyter Notebook - интерактивный анализ

📁 Структура проекта
