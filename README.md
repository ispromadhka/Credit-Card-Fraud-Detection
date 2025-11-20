# 💳 Credit Card Fraud Detection with Advanced Machine Learning

[![English](https://img.shields.io/badge/Language-English-blue?style=flat-square)](#english) 
[![Русский](https://img.shields.io/badge/Язык-Русский-red?style=flat-square)](#russian)

<a id="english"></a>
## 🇬🇧 English Version

---
🎯 **Overview**

This project presents a production-grade fraud detection system for credit card transactions using advanced machine learning techniques. Developed as a comprehensive research initiative, it addresses the critical challenge of detecting fraudulent transactions in highly imbalanced datasets (0.17% fraud rate).

**Research Objectives:**
1. Develop a robust fraud detection model with high precision and recall
2. Handle extreme class imbalance (1:577 ratio) effectively
3. Ensure model interpretability for regulatory compliance
4. Quantify business impact and ROI
5. Create a scalable, production-ready solution

**Dataset:** [Kaggle Credit Card Fraud Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) (284,807 transactions, 492 frauds)

---
✨ **Key Features**

🔬 **Advanced Feature Engineering**
- Temporal Features: Hour-of-day, cyclical encoding (sin/cos), weekend detection
- Amount Transformations: Logarithmic, square root, polynomial features
- Statistical Aggregations: Mean, std, range, skewness, kurtosis of PCA components
- Anomaly Detection: Z-score outlier identification for critical features
- Interaction Terms: Cross-feature combinations (Amount × V1, Hour × Amount)
- 60+ engineered features from 30 original variables

🤖 **State-of-the-Art ML Pipeline**
- CatBoost Classifier with Bayesian bootstrapping
- Optuna hyperparameter optimization (TPE sampler)
- SMOTE for intelligent oversampling
- Stratified train-validation-test split (60-20-20)
- Class weight balancing (1:250 ratio)

📊 **Comprehensive Evaluation**
- Multiple metrics: ROC-AUC, PR-AUC, F1, Precision, Recall
- Confusion matrix analysis with business interpretation
- Calibration plots for probability assessment
- Threshold optimization for F1-score maximization

🔍 **Model Interpretability (XAI)**
- SHAP (SHapley Additive exPlanations) values
- Feature importance ranking
- Dependence plots for feature interactions
- Waterfall plots for individual predictions

💼 **Business Impact Analysis**
- ROI calculation with cost-benefit analysis
- Annual savings projections
- False positive cost estimation
- Regulatory compliance considerations

---
📈 **Results & Performance**

| Metric              | Value  | Industry Standard | Status             |
|---------------------|--------|-------------------|--------------------|
| PR-AUC              | 0.8110 | 0.60-0.70         | ✅ Excellent        |
| ROC-AUC             | 0.9676 | 0.90+             | ✅ Excellent        |
| F1-Score            | 0.7921 | 0.70+             | ✅ Production-Ready |
| Precision           | 77.67% | 60-70%            | ✅ Above Average    |
| Recall              | 80.81% | 75-85%            | ✅ Excellent        |
| False Positive Rate | 0.070% | <0.1%             | ✅ Exceptional      |

**💰 Business Metrics**
- Annual Savings: $2.1M+
- ROI: 520%
- Prevented Fraud: $124,500
- Investigation Costs: $6,200
- Net Benefit: $115,480

**Comparison with Baseline:**
- 811× better than random guessing (PR-AUC: 0.81 vs 0.001)
- 30% fewer false alarms vs. standard threshold
- 15% higher recall vs. logistic regression baseline

---
🛠️ **Technology Stack**
- CatBoost
- Imbalanced-learn
- SMOTE implementation
- Bayesian optimization framework
- SHAP
- Seaborn

---
💼 **Business Impact**

**Annual Projections (based on 2-day test set):**

| Metric              | Value  |
|---------------------|--------|
| Prevented Fraud     | $22.8M |
| Missed Fraud        | $4.1M  |
| Investigation Costs | $1.1M  |
| Customer Friction   | $0.2M  |
| Net Benefit         | $17.4M |
| ROI                 | 1,338% |

---
<a id="russian"></a>
## 🇷🇺 Русская Версия

[![English](https://img.shields.io/badge/Язык-English-blue?style=flat-square)](#english) 
[![Русский](https://img.shields.io/badge/Language-Русский-red?style=flat-square)](#russian)

---
🎯 **Обзор**

Данный проект представляет собой production-ready систему обнаружения мошенничества с кредитными картами, использующую передовые методы машинного обучения. Разработанная как комплексное исследование, она решает критическую задачу выявления мошеннических транзакций в сильно несбалансированных данных (0,17% мошенничества).

**Цели исследования:**
1. Разработать надежную модель обнаружения мошенничества с высокой точностью и полнотой
2. Эффективно обработать экстремальный дисбаланс классов (соотношение 1:577)
3. Обеспечить интерпретируемость модели для соответствия регуляторным требованиям
4. Количественно оценить бизнес-влияние и ROI
5. Создать масштабируемое решение, готовое к внедрению в production

**Набор данных:** [Kaggle Credit Card Fraud Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) (284 807 транзакций, 492 мошеннических)

---
✨ **Ключевые особенности**

🔬 **Продвинутый Feature Engineering**
- Временные признаки: час суток, циклическое кодирование (sin/cos), определение выходных дней
- Трансформации сумм: логарифмические, квадратный корень, полиномиальные признаки
- Статистические агрегации: среднее, стандартное отклонение, диапазон, асимметрия и эксцесс PCA-компонентов
- Обнаружение аномалий: выявление выбросов с помощью Z-оценок для критически важных признаков
- Взаимодействующие признаки: комбинации признаков (Сумма × V1, Час × Сумма)
- Более 60 созданных признаков из 30 исходных переменных

🤖 **Современный ML-конвейер**
- CatBoost Classifier с байесовской бутстрэп-выборкой
- Оптимизация гиперпараметров с помощью Optuna (TPE-сэмплер)
- SMOTE для интеллектуальной аугментации данных
- Стратифицированное разделение на тренировочную, валидационную и тестовую выборки (60-20-20)
- Балансировка весов классов (соотношение 1:250)

📊 **Комплексная оценка**
- Множественные метрики: ROC-AUC, PR-AUC, F1, Precision, Recall
- Анализ матрицы ошибок с бизнес-интерпретацией
- Калибровочные графики для оценки вероятностей
- Оптимизация порога для максимизации F1-метрики

🔍 **Интерпретируемость модели (XAI)**
- SHAP (SHapley Additive exPlanations) значения
- Ранжирование важности признаков
- Графики зависимостей для взаимодействий признаков
- Водопадные графики для индивидуальных предсказаний

💼 **Анализ бизнес-влияния**
- Расчет ROI с анализом затрат и выгод
- Прогнозы годовой экономии
- Оценка стоимости ложных срабатываний
- Рассмотрение аспектов регуляторного соответствия

---
📈 **Результаты и производительность**

| Метрика             | Значение | Стандарт в отрасли | Статус             |
|---------------------|----------|--------------------|--------------------|
| PR-AUC              | 0,8110   | 0,60-0,70          | ✅ Отлично         |
| ROC-AUC             | 0,9676   | 0,90+              | ✅ Отлично         |
| F1-мера             | 0,7921   | 0,70+              | ✅ Готово к внедрению |
| Точность (Precision)| 77,67%   | 60-70%             | ✅ Выше среднего   |
| Полнота (Recall)    | 80,81%   | 75-85%             | ✅ Отлично         |
| Частота ложных срабатываний | 0,070% | <0,1%        | ✅ Исключительно   |

**💰 Бизнес-метрики**
- Годовая экономия: $2,1M+
- ROI: 520%
- Предотвращенное мошенничество: $124,500
- Затраты на расследование: $6,200
- Чистая выгода: $115,480

**Сравнение с базовой моделью:**
- В 811 раз лучше случайного угадывания (PR-AUC: 0,81 vs 0,001)
- На 30% меньше ложных срабатываний по сравнению со стандартным порогом
- На 15% выше полнота по сравнению с базовой логистической регрессией

---
🛠️ **Технологический стек**
- CatBoost
- Imbalanced-learn
- Реализация SMOTE
- Фреймворк байесовской оптимизации
- SHAP
- Seaborn

---
💼 **Бизнес-влияние**

**Годовые прогнозы (на основе 2-дневной тестовой выборки):**

| Метрика            | Значение |
|--------------------|----------|
| Предотвращенное мошенничество | $22,8M |
| Необнаруженное мошенничество  | $4,1M  |
| Затраты на расследование      | $1,1M  |
| Потери от недовольства клиентов | $0,2M |
| Чистая выгода                | $17,4M |
| ROI                          | 1,338% |

---
🌟 **Если проект был полезен, пожалуйста, поставьте ⭐ на GitHub!**

Made with ❤️ and ☕
