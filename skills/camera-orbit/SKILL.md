---
name: "camera-orbit"
description: "Orbit — плавный облёт камеры вокруг героя или продукта по дуге, объект в центре, фон вращается за ним. Используй при создании коммерческого видео для соцсетей и сайтов (HyperFrames, промты для видеомоделей), когда нужен hero shot, представление основателя, эксперта или продукта, ощущение уверенности и масштаба."
---

# Orbit (облёт вокруг героя)

Камера плавно обходит героя по дуге, он остаётся в центре кадра, а фон проворачивается за спиной. Это «знакомьтесь»: кадр делает из человека или продукта главного героя и показывает мир вокруг него.

Из исходного кадра берётся только камера, эффект и действие. Локация, время суток, свет, плёнка и персонажи подставляются под задачу ролика.

## Ядро приёма — не менять
- Камера движется по окружности вокруг объекта; объект всё время в центре.
- Высота камеры — уровень груди, скорость ровная и постоянная.
- Герой почти неподвижен: спокойная уверенная поза, максимум лёгкое движение (ветер в одежде, поворот головы).
- Фон должен читаться и красиво проворачиваться: панорама города, море, цех, зал.
- Строки `orbit ONLY` и `No zoom, no cuts` оставлять всегда.

## Что подставлять
Плёнка или look, время суток и свет, герой или продукт (с референсом Image 1), предмет в руках, локация с широким фоном, угол дуги (90, 180 или 360 градусов), направление, фоновый звук.

## Шаблон промта (на английском)
```
Shot on [FILM STOCK / LOOK], [TIME OF DAY], [LIGHT], [GRAIN], cinematic. Image 1 is [SUBJECT]: keep [exact face / product details]. [SUBJECT] stands [in LOCATION with a wide readable background], [holding OBJECT / posing], calm and confident. Camera movement: orbit ONLY. The camera circles [180] degrees around [SUBJECT] at chest height, keeping [SUBJECT] centered, while the [BACKGROUND] rotates behind. Speed: smooth constant motion. Audio: [AMBIENCE]. No zoom, no cuts.
```

## Исходный пример
```
Shot on Kodak Vision3 500T 35mm film, blue hour, city lights, light grain, cinematic. Image 1 is the man: keep his exact face, shaved head, clear glasses, beard and black T-shirt. He stands on a windy rooftop above a glowing modern skyline, holding a cinema camera at his side, calm and confident. Camera movement: orbit ONLY. The camera circles 180 degrees around him at chest height, keeping him centered, while the skyline rotates behind him. Speed: smooth constant motion. Audio: wind, distant city. No zoom, no cuts.
```

## С HyperFrames
- **Живой кадр.** Сгенерируй клип по шаблону в видеомодели и передай в HyperFrames прямую https-ссылку на mp4. Клип вставляется без звука, поэтому фон и музыку закажи в промте compose. Поверх удобно ставить имя, должность или название продукта.
- **Без генерации.** Настоящий облёт из одной фотографии не сделать. Для графики опиши в compose 3D-эквивалент: карточка продукта, телефон или макет медленно поворачивается по оси Y на 30–40 градусов с постоянной скоростью, фон плавно сдвигается в противоположную сторону (параллакс), объект остаётся в центре.

## Советы
- 180 градусов хватает для клипа 5–8 секунд; 360 просит больше времени и чаще ломает лицо.
- Если модель искажает лицо на обороте, сократи дугу до 90–120 градусов.
- Для продукта: поставь его на подиум или стол, свет сзади даёт красивый контур на повороте.
- Для 9:16 выбирай высокий фон (небоскрёбы, скалы, стеллажи), чтобы вращение читалось в узком кадре.