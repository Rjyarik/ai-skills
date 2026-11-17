---
name: "camera-crane-down"
description: "Crane down — камера плавно опускается с высоты над локацией до уровня глаз и открывает героя или продукт. Используй при создании коммерческого видео для соцсетей и сайтов (HyperFrames, промты для видеомоделей), когда нужен открывающий кадр, ввод в локацию, атмосферное начало ролика с выходом на героя."
---

# Crane down (опускание крана)

Кадр начинается высоко над локацией, камера плавно спускается до уровня глаз и находит героя. Сначала зритель получает место и атмосферу, потом человека или продукт. Классическое начало ролика.

Из исходного кадра берётся только камера, эффект и действие. Локация, время суток, свет, плёнка и персонажи подставляются под задачу ролика.

## Ядро приёма — не менять
- Старт сверху: крыши, вывески, кроны деревьев, толпа, фасад.
- Плавный вертикальный спуск до уровня глаз, без панорам и зума.
- Герой появляется в кадре по ходу спуска, а не виден с самого начала.
- Финал: средний план и одно маленькое действие героя с акцентом света и звука (в оригинале — огонь зажигалки на лице).
- Строки `crane down ONLY` и `No pan, no zoom, no cuts` оставлять всегда.

## Что подставлять
Плёнка или look, эпоха, время суток, погода и свет, верхний вид локации, герой или продукт (с референсом Image 1), поза и опора героя, финальное действие, фоновый звук и звуковой акцент.

## Шаблон промта (на английском)
```
Shot on [FILM STOCK / LOOK], [ERA / PLACE] at [TIME OF DAY], [WEATHER], [LIGHT AND COLOR ACCENTS], [GRAIN], cinematic. Image 1 is [SUBJECT]: keep [exact face / product details]. Camera movement: crane down ONLY. The shot starts high above [ESTABLISHING VIEW: rooftops, signs, treetops, crowd] and descends smoothly to eye level, revealing [SUBJECT] [pose and place: leaning on / standing at ...] under [LIGHT SOURCE]. End: medium shot as [SUBJECT] [SMALL FINAL ACTION], [light detail on the face or product]. Audio: [AMBIENCE], [one sharp accent sound for the final action]. No pan, no zoom, no cuts.
```

## Исходный пример
```
Shot on Kodak Vision3 500T 35mm film, 1970s Mexico City at night, rain, red and green neon signs, heavy grain, cinematic. Image 1 is Ramón: keep his exact face, mustache, slicked hair, cream guayabera and gold chain. Camera movement: crane down ONLY. The shot starts high above wet rooftops and neon signs and descends smoothly to eye level, revealing Ramón leaning on a red 1970s Ford sedan under a streetlight. End: medium shot as he lights a cigarette, the flame on his face. Audio: rain, buzzing neon, a lighter click. No pan, no zoom, no cuts.
```

## С HyperFrames
- **Живой кадр.** Сгенерируй клип по шаблону в видеомодели и передай в HyperFrames прямую https-ссылку на mp4. Клип вставляется без звука, поэтому фон и финальный звуковой акцент закажи в промте compose. Титр или логотип ставь на финальном среднем плане.
- **Без генерации.** Опиши в compose вертикальный проезд по высокой композиции: кадр начинается в верхней части (небо, вывески, заголовок), камера едет вниз с плавным замедлением и останавливается на герое или продукте; передние слои двигаются быстрее задних (параллакс). Подходит для длинного вертикального изображения или лендинга.

## Советы
- Финальное действие заменяй на уместное для бренда: герой поднимает чашку, открывает ноутбук, включает экран телефона, поворачивает ключ.
- Чем контрастнее верх и низ (холодное небо и тёплый свет у героя), тем сильнее эффект.
- Для 9:16 приём особенно хорош: вертикальный кадр усиливает ощущение высоты.
- Клип 6–10 секунд: спуск занимает большую часть, финальное действие 1–2 секунды.