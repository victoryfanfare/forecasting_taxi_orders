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
- 🎯 Достижение целевой метрики RMSE

## 📁 Структура проекта
- analyst-job-market-analysis/
- ├── 📓 taxi_orders_forecasting.ipynb  # Полное исследование в Jupyter
- ├── 📈 results/                       # Результаты и графики
- └── 📖 README.md                      # Документация

## 📊 Данные

### Источник данных:
- Исторические данные о заказах такси в аэропортах
- Период: март - август 2018 года
- Исходная частота: 10 минут → преобразовано в часовые данные

### Основные поля данных:
- `datetime` - временная метка
- `num_orders` - количество заказов (целевая переменная)

## 🚀 Быстрый старт

```bash
git clone https://github.com/victoryfanfare/forecasting_taxi_orders.git
cd analyst-job-market-analysis
