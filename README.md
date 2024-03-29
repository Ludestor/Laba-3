# Проект "Автоматическое обнаружение и анализ объектов на космических изображениях"
## Описание проекта
Этот проект посвящен разработке архитектуры нейронной сети для автоматического обнаружения и анализа объектов на космических изображениях. Мы используем данные о мультиспектральных изображениях городских областей, а также соответствующие метки, показывающие наличие или отсутствие застроенных территорий.

## Как использовать код
Загрузите необходимые библиотеки и установите зависимости, если это необходимо (используйте "!pip install" для установки библиотек).


Укажите путь к файлам с данными о мультиспектральных изображениях и метками.


## Описание кода
Мы используем TensorFlow и Keras для создания и обучения модели нейронной сети.


Данные о мультиспектральных изображениях и соответствующих метках загружаются с использованием библиотеки pyrsgis.


Мультиспектральные изображения предварительно обрабатываются, а метки очищаются от NoData значений.


Данные разделяются на обучающий и тестовый наборы.


Модель состоит из нескольких слоев, включая полносвязанные слои и слои активации.


Модель обучается на обучающем наборе с использованием оптимизатора Adam и категориальной кросс-энтропии в качестве функции потерь.


После обучения модель применяется к тестовому набору, и вывод сравнивается с фактическими метками.


Дополнительно, модель используется для предсказания на новых данных, и результат сохраняется в формате GeoTIFF.


## Результаты
Выводится матрица ошибок (confusion matrix) и вычисляются метрики точности (precision) и полноты (recall) для тестового набора.

Предсказания модели визуализируются на обработанных и необработанных космических изображениях.

## Важные моменты
Убедитесь, что у вас установлены все необходимые библиотеки и зависимости.


Запустите код последовательно, следуя инструкциям в ноутбуке. [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1nB22eElQYAp0pF3SWReZjVPSMHXk-9If?hl=ru#scrollTo=YG8JzyAaXi9P)


## Пример визуализации

![image](https://github.com/Ludestor/Laba-3/assets/119999440/6a820d7e-797a-482c-9bd8-83f385c060a3)



![image](https://github.com/Ludestor/Laba-3/assets/119999440/ca0f97ed-05b2-4e66-9cd6-d9ff8e87f496)
