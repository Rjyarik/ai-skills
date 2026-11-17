---
name: "camera-handheld"
description: "Handheld — ручная камера, оператор бежит следом за героем с живой тряской и рывками кадра, документальный реализм. Используй при создании коммерческого видео для соцсетей и сайтов (HyperFrames, промты для видеомоделей), когда нужна энергия, спешка, погоня, эффект присутствия или ощущение настоящей съёмки без постановки."
---

# Handheld (ручная камера следом за героем)

Оператор бежит прямо за героем: кадр трясётся, дышит, герой то и дело уходит к краю, камера его догоняет. Ощущение, что всё происходит по-настоящему и прямо сейчас. Приём для спешки, погони, закулисья, роликов в стиле репортажа.

Из исходного кадра берётся только камера, эффект и действие. Локация, время суток, свет, плёнка и персонажи подставляются под задачу ролика.

## Ядро приёма — не менять
- Камера в руках оператора, который бежит сразу за героем.
- Органичная тряска, «дыхание» кадра, мелкие рывки при перекадровке; оператор с трудом удерживает героя в кадре.
- Герой быстро движется через людное место, преодолевает препятствия, оглядывается через плечо.
- Документальный look: 16mm, жёсткий естественный свет, сильное зерно.
- Звук: шаги, голоса толпы, тяжёлое дыхание.
- Строки `handheld ONLY` и `No zoom, no cuts` оставлять всегда.

## Что подставлять
Плёнка (лучше 16mm или «documentary»), свет, герой (с референсом Image 1), людная локация, препятствия и что герой задевает, куда он спешит, звуки среды.

## Шаблон промта (на английском)
```
Shot on [FILM STOCK] 16mm film, [HARSH NATURAL LIGHT], documentary realism, heavy grain. Image 1 is [SUBJECT]: keep [exact face and clothing]. [SUBJECT] runs fast through [CROWDED LOCATION], [OBSTACLE ACTIONS: shoving past ..., knocking over ...], glancing back over the shoulder. Camera movement: handheld ONLY. An operator runs right behind [SUBJECT] with organic shake, breathing, small reframing bumps, fighting to keep [SUBJECT] in frame. Audio: footsteps, [CROWD SOUNDS], heavy breathing. No zoom, no cuts.
```
Спокойный вариант для интервью и закулисья: замени бег на `walks through` и тряску на `subtle handheld sway and breathing, gentle reframing`.

## Исходный пример
```
Shot on Kodak Vision3 500T 16mm film, harsh midday sun, documentary realism, heavy grain. Image 1 is Ramón: keep his exact face, mustache, slicked hair, cream guayabera and gold chain. Ramón runs fast through a crowded street market, shoving past stalls, knocking over a crate of oranges, glancing back over his shoulder. Camera movement: handheld ONLY. An operator runs right behind him with organic shake, breathing, small reframing bumps, fighting to keep him in frame. Audio: footsteps, shouting vendors, heavy breathing. No zoom, no cuts.
```

## С HyperFrames
- **Живой кадр.** Сгенерируй клип по шаблону в видеомодели и передай в HyperFrames прямую https-ссылку на mp4. Клип вставляется без звука, поэтому шаги, толпу и дыхание закажи в промте compose.
- **Оформление в HyperFrames.** Титры поверх трясущегося клипа держи неподвижными и крупными: контраст статичного текста и живого кадра хорошо читается. Субтитры ставь на плашке.
- **Без генерации.** Ручную камеру можно добавить к статичному кадру или графике: в compose опиши лёгкое плавающее смещение кадра на 6–10 px и поворот до 0.3 градуса с медленным «дыханием», кадр чуть увеличен, чтобы не было видно краёв. Тряска задаётся фиксированными ключевыми кадрами, а не случайными числами: рендер должен быть одинаковым при каждом запуске.

## Советы
- Препятствия конкретизируй (ящик, стулья, вешалка с одеждой): они дают кадру события.
- Взгляд через плечо создаёт историю: за героем кто-то или что-то гонится (дедлайн, распродажа, уходящий автобус).
- Для 9:16 приём идеален: съёмка со спины естественно ложится в вертикаль.
- Не сочетай с другими движениями камеры в одном клипе.