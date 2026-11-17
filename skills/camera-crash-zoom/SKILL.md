---
name: "camera-crash-zoom"
description: "Crash zoom — резкий наезд зумом с общего плана на сверхкрупный за долю секунды. Используй при создании коммерческого видео для соцсетей и сайтов (HyperFrames, промты для видеомоделей), когда кадру нужен акцент, панчлайн, реакция героя или резкий показ ключевой детали продукта."
---

# Crash zoom (резкий наезд зумом)

Камера стоит неподвижно, короткая пауза, затем объектив за долю секунды «влетает» с общего плана на сверхкрупный одной детали. Работает как восклицательный знак: реакция героя, панчлайн, цена, логотип, ключевая деталь продукта.

Из исходного кадра берётся только камера, эффект и действие. Локация, время суток, свет, плёнка и персонажи подставляются под задачу ролика.

## Ядро приёма — не менять
- Камера зафиксирована на месте: работает только зум. Без тележки, панорам и склеек.
- Спокойная пауза около 2 секунд на общем плане, затем зум за долю секунды.
- Цель зума — одна конкретная деталь (глаза, логотип, экран, кнопка, этикетка).
- Лёгкая тряска в момент «приземления», потом удержание резкого крупного плана.
- Звук: жёсткий whoosh точно на зуме.
- Строки `crash zoom ONLY` и `No dolly, no pan, no cuts` оставлять всегда: они удерживают модель от лишних движений.

## Что подставлять
Плёнка или look, время суток и свет, локация, герой или продукт (с референсом Image 1), статичная поза до зума, деталь-цель, фоновый звук.

## Шаблон промта (на английском)
```
Shot on [FILM STOCK / LOOK], [TIME OF DAY], [LIGHT], [GRAIN], cinematic. Image 1 is [SUBJECT]: keep [exact face / product details]. [SUBJECT] [stands still / holds a pose] in [LOCATION], [small static action], staring ahead. Camera movement: crash zoom ONLY. The camera stays locked in place; at second 2 the lens zooms violently in a fraction of a second from a wide shot to an extreme close-up of [TARGET DETAIL], with a tiny shake on landing. End: hold on [TARGET DETAIL], sharp. Audio: [AMBIENCE], a hard whoosh on the zoom. No dolly, no pan, no cuts.
```

## Исходный пример
```
Shot on Kodak Vision3 500T 35mm film, night, sodium streetlight, heavy grain, cinematic. Image 1 is Ramón: keep his exact face, thick mustache, slicked-back hair, cream guayabera, gold chain and tattooed forearms. Ramón stands in a rain-soaked Mexico City alley, cigarette in his mouth, staring ahead. Camera movement: crash zoom ONLY. The camera stays locked in place; at second 2 the lens zooms violently in a fraction of a second from a wide shot to an extreme close-up of his eyes, with a tiny shake on landing. End: hold on his eyes, sharp. Audio: rain, distant traffic, a hard whoosh on the zoom. No dolly, no pan, no cuts.
```

## С HyperFrames
- **Живой кадр (люди, локации, фотореализм).** Сгенерируй клип по шаблону в видеомодели (image-to-video с референсом) и передай в HyperFrames прямую https-ссылку на mp4. Клип вставляется без звука, поэтому whoosh и фон закажи отдельно в промте compose, привязав whoosh к моменту зума.
- **Без генерации (фото продукта, скриншот, графика).** Опиши в compose виртуальную камеру: статичный общий план 2 с, затем масштаб с 1 до 4–6 за 0.15–0.25 с с жёстким ускорением и радиальным размытием, 2–3 кадра микротряски на остановке, удержание 1–2 с, whoosh на зуме. Исходник нужен в высоком разрешении, иначе крупный план будет мыльным.

## Советы
- Один crash zoom на клип: второй обесценивает первый.
- Деталь-цель должна быть видна уже на общем плане и стоять близко к центру кадра.
- Сразу после зума хорошо ставить титр, цену или склейку на следующий кадр.
- Для 9:16 держи героя и деталь-цель в центральной трети кадра.