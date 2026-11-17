---
name: "camera-fpv-drone"
description: "FPV drone — один непрерывный пролёт дрона — пике сверху, полёт низко над поверхностью и резкий выход на героя. Используй при создании коммерческого видео для соцсетей и сайтов (HyperFrames, промты для видеомоделей), когда нужен динамичный показ места — путешествия, отели, недвижимость, рестораны, события."
---

# FPV drone (пролёт дрона одним кадром)

Дрон пикирует сверху, проносится вдоль рельефа и резко выходит к герою, который приветствует камеру. За несколько секунд зритель получает всё место целиком и эмоцию в финале. Лучший приём для путешествий, отелей, недвижимости и событий.

Из исходного кадра берётся только камера, эффект и действие. Локация, время суток, свет, плёнка и персонажи подставляются под задачу ролика.

## Ядро приёма — не менять
- Один непрерывный кадр, без склеек.
- Маршрут из четырёх точек: высоко над локацией, пике вниз вдоль вертикали, бреющий полёт над поверхностью, резкий подъём к герою.
- Быстрые плавные виражи с наклоном горизонта.
- Финал: крупный план героя, который делает жест в камеру (поднимает бокал, показывает продукт, машет).
- Звук: шум ветра, звук поверхности, акцент на финальном жесте.
- Строки `FPV drone shot ONLY` и `One continuous shot, no cuts` оставлять всегда.

## Что подставлять
Плёнка или look, время суток и свет, общий вид локации, вертикальный элемент (скала, фасад, водопад), поверхность (море, улица, бассейн, виноградник), точка прибытия (терраса, вход, палуба), герой (с референсом Image 1), жест в камеру, звуки.

## Шаблон промта (на английском)
```
Shot on [FILM STOCK / LOOK], [TIME OF DAY], [LIGHT], cinematic. Image 1 is [SUBJECT]: keep [exact face and clothing]. Camera movement: FPV drone shot ONLY. The drone dives fast from above [WIDE LOCATION], plunges down [VERTICAL FEATURE], skims low over [SURFACE], then pulls up sharply onto [DESTINATION] where [SUBJECT], [detail], [GREETING ACTION to the camera]. Fast, fluid banking turns. End: close on [SUBJECT] [smiling / PRODUCT in focus]. Audio: rushing wind, [SURFACE SOUND], [accent sound of the final action]. One continuous shot, no cuts.
```

## Исходный пример
```
Shot on Kodak Vision3 250D 35mm film, golden hour, warm sun flares, cinematic. Image 1 is Dolores: keep her exact face, grey hair, glasses and clothing. Camera movement: FPV drone shot ONLY. The drone dives fast from above a white Mediterranean village on a cliff, plunges down the cliff face, skims low over the sea, then pulls up sharply onto a terrace where Dolores, wearing sunglasses, raises a glass of vermouth to the camera. Fast, fluid banking turns. End: close on Dolores smiling. Audio: rushing wind, waves, a glass clink. One continuous shot, no cuts.
```

## С HyperFrames
- **Живой кадр.** Этот приём почти всегда требует сгенерированного клипа. Сгенерируй его по шаблону в видеомодели и передай в HyperFrames прямую https-ссылку на mp4. Клип вставляется без звука, поэтому ветер, поверхность и финальный акцент закажи в промте compose. Титр или призыв к действию ставь на финальном крупном плане.
- **Без генерации.** Опиши в compose пролёт по большой карте или коллажу: быстрый непрерывный проезд от общего вида к точке назначения с увеличением масштаба, лёгким наклоном кадра на поворотах и размытием движения, остановка на карточке места или продукта. Хорошо работает для маршрута путешествия.

## Советы
- Маршрут описывай глаголами движения по порядку (dives, plunges, skims, pulls up): модель идёт по ним как по точкам.
- Больше четырёх точек маршрута за один клип не уместить: кадр развалится.
- Жест в камеру в финале обязателен: без него пролёт остаётся просто красивым видом.
- Для 9:16 выбирай маршруты с вертикалью (скала, башня, фасад): пике читается сильнее.