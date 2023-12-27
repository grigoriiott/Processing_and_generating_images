# Processing_and_generating_images

Обработка и генерация изображений
Отт Григорий Владимирович
Задача: Множественная классификация
Датасет: CIFAR-10

Feature extractor:
![image](https://github.com/grigoriiott/Processing_and_generating_images/assets/92350053/28d070a5-1320-486b-8567-e0321408f3f9)

# Обучение на полном датасете с предобученным feature extractor:

![image](https://github.com/grigoriiott/Processing_and_generating_images/assets/92350053/87a7463e-2ab8-493f-9f59-4a59609dd0bb)

Метрики:

![image](https://github.com/grigoriiott/Processing_and_generating_images/assets/92350053/2701fa02-a24d-403f-b2e7-c10c52cd4737)

Заключение: Модель обучилась на несколько эпох быстрее при этом сохоранив значения метрик из hw_1 и даже превзойдя их (незначительно).

# Обучение на 50% датасете с предобученным feature extractor: 

![image](https://github.com/grigoriiott/Processing_and_generating_images/assets/92350053/5301e6a1-9ffe-42e6-bc23-9e3bd450ac29)

Метрики:

![image](https://github.com/grigoriiott/Processing_and_generating_images/assets/92350053/b9fe8415-8615-4b79-983d-d134291ab967)

Заключение: Метрики при обучении на 50% датасета снизились незначительно в сравнении с полным набором данных. При этом для обучения потребовалось большее количество эпох, что логично из-за меньшего размера датасета (каждая эпоха содержит меньше итераций, т.к. батч сайз остался неизменным). Но стоит отметить, что обучение заняло меньшее количество времени (2,5 мин) в сравнении с первым экспериментом.

# Обучение на 10% датасете с предобученным feature extractor: 

![image](https://github.com/grigoriiott/Processing_and_generating_images/assets/92350053/63054a82-2ede-481b-8d0d-444458bc8447)

Метрики:

![image](https://github.com/grigoriiott/Processing_and_generating_images/assets/92350053/31d8c111-1c06-4dd9-a0fa-df686db34dcb)

Заключение: В случае с использованием всего 10 процентов данных, значения метрик упали. При этом время обучения (1 мин 42 с) значительно меньше, чем при обучении на полном датасете.

# Вывод
Стоит отметить, что при использовании предобучения feature extractor удалось достичь схожих метрик с моделью из hw_1. При этом обучение заняло меньшее количество времени, что может быть существенно при решении более сложных задач.

Примеры работы модели из эксперимента 2:

![image](https://github.com/grigoriiott/Processing_and_generating_images/assets/92350053/d6bcaba3-226b-49c8-89c9-32ca5154ba93)
