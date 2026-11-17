---
name: "camera-dolly-zoom"
description: "Dolly zoom (эффект вертиго) — камера отъезжает, объектив наезжает, герой остаётся того же размера, а фон меняет масштаб. Используй при создании коммерческого видео для соцсетей и сайтов (HyperFrames, промты для видеомоделей), когда нужно показать момент осознания, боль клиента, шок или внезапное решение."
---

# Dolly zoom (эффект вертиго)

Камера едет назад, а объектив одновременно наезжает зумом. Лицо героя остаётся того же размера, а пространство за ним «плывёт». Зритель физически чувствует внутренний сдвиг героя: «о нет», «вот оно что», «мне это нужно».

Из исходного кадра берётся только камера, эффект и действие. Локация, время суток, свет, плёнка и персонажи подставляются под задачу ролика.

## Ядро приёма — не менять
- Два движения сразу: тележка назад и зум вперёд. Размер героя в кадре постоянный.
- Герой стоит неподвижно; меняется только эмоция на лице (глаза расширяются, медленная улыбка).
- Скорость медленная и постоянная, без рывков.
- Нужен глубокий фон с линиями перспективы: проход, коридор, улица, ряды полок.
- Звук: низкий тянущийся тон плюс тихий фон локации.
- Строки `dolly zoom ONLY (vertigo effect)` и `No pan, no cuts` оставлять всегда.

## Что подставлять
Плёнка или look, свет, герой (с референсом Image 1), глубокая локация, триггер осознания (пустая полка, экран, вывеска, ценник), смена эмоции, фоновый звук.

## Шаблон промта (на английском)
```
Shot on [FILM STOCK / LOOK], [LIGHT], [GRAIN], cinematic. Image 1 is [SUBJECT]: keep [exact face and clothing]. [SUBJECT] stands still in the middle of [LONG DEEP LOCATION: aisle, corridor, street], in front of [TRIGGER OBJECT], realising [WHAT], [EMOTION SHIFT: eyes widening / slow smile]. Camera movement: dolly zoom ONLY (vertigo effect). The camera dollies backward while the lens zooms in, so [SUBJECT]'s face stays the same size while the [BACKGROUND] behind stretches away. Speed: slow and constant. Audio: low droning tone, [AMBIENCE]. No pan, no cuts.
```
Зеркальный вариант для позитивного «вау»: `The camera dollies forward while the lens zooms out` — фон раскрывается вширь.

## Исходный пример
```
Shot on Kodak Vision3 250D 35mm film, flat fluorescent supermarket light, fine grain, cinematic. Image 1 is Dolores: keep her exact face, grey hair, glasses and clothing. Dolores stands still in the middle of a long supermarket frozen-food aisle in front of an empty shelf with a sign that reads AGOTADO, realising the croquettes are gone, eyes widening. Camera movement: dolly zoom ONLY (vertigo effect). The camera dollies backward while the lens zooms in, so her face stays the same size while the aisle behind her stretches away. Speed: slow and constant. Audio: low droning tone, fridge hum. No pan, no cuts.
```

## С HyperFrames
- **Живой кадр.** Сгенерируй клип по шаблону в видеомодели и передай в HyperFrames прямую https-ссылку на mp4. Клип вставляется без звука, поэтому низкий тон и фон закажи в промте compose.
- **Без генерации.** Нужны два слоя: вырезанный герой (PNG без фона) и отдельный фон. В compose опиши: герой неподвижен и не меняет размер, фон медленно и равномерно меняет масштаб с 1 до 1.3–1.5 от центра за всю длину кадра, лёгкое затемнение краёв. Из одной склеенной картинки эффект не получится.

## Советы
- Приём сильный: одного раза на ролик достаточно.
- Хорошо ставится в начало ролика как «проблема клиента», следом идёт решение.
- Надпись-триггер в кадре (вывеска, ценник) делай короткой: модели ошибаются в длинном тексте.
- Для 9:16 лицо держи в верхней трети, перспектива уходит за спину по центру.