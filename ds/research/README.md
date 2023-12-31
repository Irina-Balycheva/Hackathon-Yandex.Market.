# Разработка алгоритма сервиса упаковщика для Яндекс Маркета

## Объект исследования
В качестве исходных данных предоставленны исторические сведения о заказах, товарах и выбранной упаковке.

## Задача проекта
Необходимо придумать способ подсказывать пользователю информацию о выборе упаковочного материала, а также разработать интерфейс для упаковщика.

## Выводы

В основу алгоритма рекомендации упаковки разработана модель LGBMClassifier со следующими параметрами:
   - objective: 'multiclass';
   - num_class:17;
   - metric': 'multi_logloss';
   - num_leaves': 50;
   - learning_rate': 0.1;
   - n_estimators': 500;
   - class_weight': 'balanced';
   - max_depth: 14.

Достигнута лучшая метрика при тестировании для класса упаковки MYB recall = 0.52. 
