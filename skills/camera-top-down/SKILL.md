---
name: "camera-top-down"
description: "Top-down — вид строго сверху с медленным вращением по часовой стрелке и лёгким снижением камеры. Используй при создании коммерческого видео для соцсетей и сайтов (HyperFrames, промты для видеомоделей), когда нужно показать стол, раскладку товаров, еду, рабочее место, карту или сцену с двумя участниками и действием рук."
---

# Top-down (вид сверху с вращением)

Камера смотрит вертикально вниз на стол или поверхность, медленно вращается по часовой стрелке и чуть снижается. Зритель видит всю раскладку как схему, а медленное вращение добавляет напряжение и дороговизну. В центре внимания руки и предметы.

Из исходного кадра берётся только камера, эффект и действие. Локация, время суток, свет, плёнка и персонажи подставляются под задачу ролика.

## Ядро приёма — не менять
- Камера строго над центром поверхности, смотрит прямо вниз, без наклона.
- Медленное вращение по часовой стрелке и небольшое снижение одновременно.
- Все участники и вся поверхность остаются в кадре до конца.
- Одно медленное действие руками в центре (в оригинале — переворот карты).
- Звук: приглушённый гул помещения, звуки предметов, акцент на действии.
- Строки `top-down ONLY` и `No tilt, no cuts` оставлять всегда.

## Что подставлять
Плёнка или look, свет и цветовые акценты, поверхность (стол, прилавок, пол, карта), предметы на ней, участники (референсы Image 1, Image 2) или только руки, действие руками, звуки.

## Шаблон промта (на английском)
```
Shot on [FILM STOCK / LOOK], [LIGHT], [COLOR ACCENTS], cinematic. Image 1 is [SUBJECT A] ([key details]). Image 2 is [SUBJECT B] ([key details]). Keep both faces and outfits exact. [SUBJECTS] sit facing each other at [TABLE / SURFACE] in [LOCATION], [OBJECTS laid out between them]; [SUBJECT] slowly [SMALL HAND ACTION]. Camera movement: top-down ONLY. The camera looks straight down from directly above the [TABLE] and slowly rotates clockwise while descending a little. Framing: [all subjects] and the [TABLE] stay in frame. Audio: [ROOM MURMUR], [OBJECT SOUNDS], [accent on the hand action]. No tilt, no cuts.
```
Вариант без людей: вместо участников напиши `Only hands enter the frame from [side]` и опиши раскладку товаров.

## Исходный пример
```
Shot on Kodak Vision3 500T 35mm film, smoky casino light, green felt, gold accents, cinematic. Image 1 is Ramón (mustache, cream guayabera, gold chain). Image 2 is Dolores (grey hair, glasses). Keep both faces and outfits exact. Ramón and Dolores sit facing each other at a green baccarat table in a Macao casino, cards and stacks of chips between them; Dolores slowly flips one card. Camera movement: top-down ONLY. The camera looks straight down from directly above the table and slowly rotates clockwise while descending a little. Framing: both players and the table stay in frame. Audio: casino murmur, chips clicking, a card flip. No tilt, no cuts.
```

## С HyperFrames
- **Живой кадр.** Сгенерируй клип по шаблону в видеомодели и передай в HyperFrames прямую https-ссылку на mp4. Клип вставляется без звука, поэтому гул, звуки предметов и акцент закажи в промте compose.
- **Без генерации.** Приём легко делается графикой. Возьми фото раскладки сверху или макет интерфейса и опиши в compose: кадр медленно и равномерно поворачивается по часовой стрелке на 10–15 градусов и увеличивается с 1 до 1.1 за всю длину сцены. Изображение бери с запасом по краям, чтобы при повороте не появились пустые углы.

## Советы
- Лица сверху почти не видны: героев делают узнаваемыми одежда, причёска и руки. Укажи это в деталях референса.
- Раскладка должна быть симметричной или иметь явный центр: вращение идёт вокруг него.
- Подходит для еды, распаковки, планирования поездки над картой, набора товаров, рабочего стола.
- Для 9:16 разверни стол длинной стороной по вертикали.