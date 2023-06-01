# 3D Модели смартфона и Заярдного устройства
## Программы
- **Blender 3.5.1**
## Актуальность
В наше время встретить **DeepFake** не такая большая редкость, и чтобы автоматизировать процесс их выявления и обезопасить себя ведется разработка нейронной сети, способной это сделать
## Теория
Для обучения нейронной сети аудиозаписи из датасета конвертируются в ***mel-спектрограмму***:
![mel_spec](https://miro.medium.com/max/1400/1*zX-rizZKXXg7Ju-entot9g.png)
Она представляет собой график зависимости времени частоты и громкости аудиозаписи, но отличается от обычной спектрограммы тем, что все параметры логарифмически преобразованы в диапазон частот, которые может услышать человек
## Обучение
Для обучения была использована технология ***transfer learning***. В качестве базовой модели взята **ResNet50**. Для получения лучшего результата использовался Баесовский алгоритм оптимизации с помощью которого были получены оптимальные гиперпараметры
## Метрики
Наибольшая достигнутая точность на тестовом наборе данных ~80%
## Пример спектрограммы сгенерированной для обучения нейронной сети
![spec1](https://sun9-74.userapi.com/impf/qu6fFigr2Kbvun37TfyrNtXqAX1DCn-EffSfKw/OoS7F52nAY0.jpg?size=224x224&quality=95&sign=e42c2d19ebb3c33a30ac820d7e7de243&type=album)
![spec2](https://sun9-85.userapi.com/impf/tX5u8i1j-8K_MPBmmOPJN9pA3ts8bN852xTBLA/8sx7r5IMoaA.jpg?size=350x350&quality=95&sign=04a3a17c0226e3a5d87b434b40dac8ee&type=album)
## Если вы хотите изучить/улучшить модель
- датасет находится в репозитории, папка - **'dataset'**
- все возможные варианты кода для переноса обучения в папке - **'scripts'**
- готовые веса, показавшие наилучшую точность на тестовой выборке в папке - **'models'**
## Контакты
- VK : [Матвей Раизнов](https://vk.com/maveyuma)
- [Telegram](https://t.me/barulitka)
- mail : chikernut213@gmai.com
