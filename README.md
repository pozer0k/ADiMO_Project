# Image Classification

Этот проект демонстрирует процесс создания модели классификации изображений на основе PyTorch, начиная с обработки данных, базового обучения модели и заканчивая использованием метода transfer learning.

## Структура проекта

### 📂 Данные
Изображения разделены на три класса: `Happy`, `Sad`, `Angry`.  
Данные расположены в директории `ADiMO_Project/дб/`.

### 📜 Содержание
1. **Импорт библиотек и данных**  
   - Используются библиотеки: `numpy`, `pandas`, `torch`, `torchvision` и др.
   - Данные считываются с помощью библиотеки `pathlib` и создается датафрейм с путями и метками.  

2. **EDA (Exploratory Data Analysis)**  
   - Исследование распределения классов.  
   - Визуализация изображений и их размеров.  

3. **Подготовка данных**  
   - Данные разделяются на обучающую и валидационную выборки.  
   - Используются трансформации изображений с помощью `torchvision.transforms`.  

4. **Создание модели**  
   - Реализована базовая сверточная сеть `ConvNet`.  
   - Используется метод transfer learning с моделью `EfficientNet-B0`.  

5. **Обучение модели**  
   - Определены функции `train_step` и `test_step` для обучения и валидации.  
   - Модель обучается на GPU (при наличии).  

6. **Оценка модели**  
   - Используется метрика точности (`torchmetrics.Accuracy`) для оценки производительности модели.  

## Установка и запуск

### Требования
- Python 3.7+
- Установленные зависимости:

pip install numpy pandas torch torchvision torchmetrics matplotlib seaborn plotly


### Запуск
1. Скачайте данные и расположите их в структуре, описанной выше.
2. Запустите ноутбук Jupyter или Google Colab.
3. Запустите файл все части кода в BotEmote.ipynb
4. Используйте бота в Telegram
https://t.me/BotEmote_bot

## Возможные улучшения
1. Добавить больше данных для обучения, особенно для классов с меньшим количеством изображений.  
2. Применить другие методы аугментации данных.  
3. Исследовать более сложные архитектуры сетей, такие как ResNet, DenseNet и т. д.  


## Авторы
Разработано для студенческого проекта по изучению классификации изображений.  
Хайрудинов Никита МКИС32
Тельп Владсилва МКИС32
Жаданов Антно МКИС32
