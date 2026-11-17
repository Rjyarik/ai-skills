---
name: "camera-rack-focus"
description: "Rack focus — перевод фокуса с предмета на переднем плане на героя в глубине кадра при полностью неподвижной камере. Используй при создании коммерческого видео для соцсетей и сайтов (HyperFrames, промты для видеомоделей), когда нужно связать продукт и человека, показать реакцию на товар или перевести внимание с детали на главное."
---

# Rack focus (перевод фокуса)

Камера не двигается совсем. В резкости предмет на переднем плане, герой сзади размыт. Затем фокус переезжает на героя, он даёт маленькую реакцию, а предмет уходит в размытие. Так в одном кадре связываются продукт и человек: товар и его покупатель, блюдо и гость, гаджет и владелец.

Из исходного кадра берётся только камера, эффект и действие. Локация, время суток, свет, плёнка и персонажи подставляются под задачу ролика.

## Ядро приёма — не менять
- Камера полностью неподвижна: меняется только фокус.
- Длинный объектив (85mm) и очень малая глубина резкости.
- Передний план: один предмет в резкости, занимает одну сторону кадра.
- Задний план: герой не в фокусе.
- На второй секунде фокус переходит на героя; он делает микрореакцию в камеру (поднимает бровь, улыбается, кивает).
- Звук тихий и детальный: тиканье, лёгкое шипение, комнатный тон.
- Строки `rack focus ONLY` и `No dolly, no zoom, no cuts` оставлять всегда.

## Что подставлять
Look плёнки, свет, предмет или продукт на переднем плане, сторона кадра, герой (с референсом Image 1), место и поза героя, микрореакция, тихие звуки.

## Шаблон промта (на английском)
```
Shot on [FILM LOOK], [LIGHT], 85mm lens, very shallow depth of field, cinematic. Image 1 is [SUBJECT]: keep [exact face and clothing]. Foreground: [OBJECT / PRODUCT], in sharp focus, filling the [left / right] of frame. Background: [SUBJECT] [pose and place], out of focus. Camera movement: rack focus ONLY. The camera is completely still; at second 2 focus shifts from [OBJECT] to [SUBJECT], who [MICRO REACTION] at the camera. [OBJECT] goes soft. Audio: [QUIET ROOM TONE], [faint detail sound]. No dolly, no zoom, no cuts.
```
Обратный вариант для рекламного финала на продукте: начать в фокусе на герое и перевести фокус на продукт: `focus shifts from [SUBJECT] to [PRODUCT]. [SUBJECT] goes soft.`

## Исходный пример
```
Shot on Kodak Portra 400 look, warm tungsten kitchen light at night, 85mm lens, very shallow depth of field, cinematic. Image 1 is Dolores: keep her exact face, grey hair, glasses and clothing. Foreground: a fork holding one golden croquette, in sharp focus, filling the left of frame. Background: Dolores sitting at the kitchen table, out of focus. Camera movement: rack focus ONLY. The camera is completely still; at second 2 focus shifts from the croquette to Dolores, who slowly raises one eyebrow at the camera. The croquette goes soft. Audio: kitchen clock ticking, faint sizzle. No dolly, no zoom, no cuts.
```

## С HyperFrames
- **Живой кадр.** Сгенерируй клип по шаблону в видеомодели и передай в HyperFrames прямую https-ссылку на mp4. Клип вставляется без звука, поэтому тихие звуки закажи в промте compose. Титр ставь на свободной стороне кадра, напротив предмета.
- **Без генерации.** Приём хорошо воспроизводится графикой. Нужны два слоя: предмет на переднем плане (PNG без фона) и фон с героем. В compose опиши: первые 2 с передний слой резкий, задний размыт примерно на 12–16 px; затем за 0.6–0.8 с размытие меняется местами; оба слоя увеличиваются на 1–2 процента, имитируя «дыхание» объектива.

## Советы
- Предмет и герой должны стоять на разных сторонах кадра, иначе перевод фокуса не читается.
- Реакцию героя держи маленькой: в этом приёме работает сдержанность.
- Для карточек товаров и рекламы еды используй обратный вариант с финалом на продукте.
- Для 9:16 предмет ставь внизу кадра, героя выше и глубже.