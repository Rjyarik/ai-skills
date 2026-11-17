---
name: "camera-low-angle-tracking"
description: "Low-angle tracking — камера на уровне колен едет назад перед героями, которые идут на неё в замедлении, пока за спиной происходит большое событие. Используй при создании коммерческого видео для соцсетей и сайтов (HyperFrames, промты для видеомоделей), когда нужен эпичный проход героя или команды, запуск, анонс, ощущение силы."
---

# Low-angle tracking (проход героев с нижней точки)

Камера низко, на уровне колен, и отъезжает назад ровно со скоростью героев. Они идут прямо на зрителя в замедлении, а за спиной происходит что-то огромное, на что они не оборачиваются. Нижняя точка делает героев крупнее и сильнее. Кадр для запуска, анонса, команды, основателя.

Из исходного кадра берётся только камера, эффект и действие. Локация, время суток, свет, плёнка и персонажи подставляются под задачу ролика.

## Ядро приёма — не менять
- Камера на высоте колен, смотрит вверх на героев.
- Камера едет назад перед героями точно с их скоростью: их размер в кадре не меняется.
- Герои идут на камеру рядом друг с другом, по центру кадра, в замедлении.
- За спиной большое событие; герои не оглядываются. Это и есть эффект.
- Свет от события освещает героев сзади.
- Звук: низкий удар события плюс гул замедления.
- Строки `low-angle tracking ONLY` и `No zoom, no cuts` оставлять всегда.

## Что подставлять
Плёнка или look, время суток, один или несколько героев (референсы Image 1, Image 2), пустая улица, коридор или взлётная полоса, событие за спиной, источник света от события, звуки.

Событие не обязано быть взрывом. Для бренда подойдут: фейерверк, залп конфетти, вспыхивающая вывеска или витрина, гигантский экран, волна, взлетающий самолёт, толпа, которая срывается с места.

## Шаблон промта (на английском)
```
Shot on [FILM STOCK / LOOK], [TIME OF DAY], [LIGHT FROM THE EVENT], [GRAIN], epic action cinema. Image 1 is [SUBJECT A] ([key details]). Image 2 is [SUBJECT B] ([key details]). Keep both faces and outfits exact. [SUBJECTS] walk side by side toward the camera down [EMPTY STREET / CORRIDOR / RUNWAY] in slow motion while [BIG BACKGROUND EVENT] behind them. They never look back. Camera movement: low-angle tracking ONLY. The camera is at knee height, moving backward in front of them at exactly their walking speed, keeping [both / the subject] centered. Audio: [EVENT SOUND], [DETAIL SOUND], slow-motion rumble. No zoom, no cuts.
```

## Исходный пример
```
Shot on Kodak Vision3 500T 35mm film, night, orange fire light, heavy grain, epic action cinema. Image 1 is Ramón (mustache, cream guayabera, gold chain). Image 2 is Dolores (grey hair, glasses). Keep both faces and outfits exact. Ramón and Dolores walk side by side toward the camera down an empty street in slow motion while a car explodes behind them in a huge fireball. They never look back. Camera movement: low-angle tracking ONLY. The camera is at knee height, moving backward in front of them at exactly their walking speed, keeping both centered. Audio: deep explosion boom, debris, slow-motion rumble. No zoom, no cuts.
```

## С HyperFrames
- **Живой кадр.** Этот приём требует сгенерированного клипа. Сгенерируй его по шаблону в видеомодели и передай в HyperFrames прямую https-ссылку на mp4. Клип вставляется без звука, поэтому удар события и гул закажи в промте compose, привязав удар к моменту события.
- **Оформление в HyperFrames.** Центр кадра оставь героям. Крупный титр или название продукта ставь в верхней трети, появление титра синхронизируй с событием за спиной.
- **Без генерации.** Полноценной замены нет. Ближайший графический вариант: вырезанные герои неподвижны по центру, фон за ними медленно уменьшается и уходит вдаль, сзади вспышка света. Используй только если клип сгенерировать нельзя.

## Советы
- Один герой тоже работает: убери Image 2 и замени `both` на `the subject`.
- Событие должно быть сзади и по центру, иначе герои его перекрывают неудачно.
- В 9:16 двое героев помещаются плечом к плечу; для троих и больше нужен 16:9.
- Хороший финальный кадр ролика перед логотипом.