# U-net classification

## Статус проекта: завершён

## Описание проекта

Реализовать U-Net в файле model.py для задачи семантической сегментации: 0 - не автомобиль, 1 - автомобиль

## Навыки и инструменты

- **tensorboard**
- **torch**
- **tqdm**
- **carvana_dataset**
- **seaborn**


## Цель исследования

Нужно реализовать U-Net в файле model.py для задачи семантической сегментации: 0 - не автомобиль, 1 - автомобиль. Модель должна принимать четырёхмерные тензоры картинок (нулевая размерность — батч) и предсказывать трёхмерные тензоры (нулевая размерность — батч) из логарифмов вероятностей (логитов) каждого пикселя в бернуллиевской модели. В качестве функции ошибки при обучении используется бинарная кросс-энтропия в реализации с логитами — torch.nn.BCEWithLogitsLoss(). Переход от логитов к маске осуществляется посредством отсечения по порогу: logits > 0.
