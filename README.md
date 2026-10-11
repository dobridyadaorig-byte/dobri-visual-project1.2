# Dobri Visual (Fabric, MC 1.21.11) — клиентский мод
Меню: Right Shift (меняется в Settings → Keybinds). ЛКМ по модулю — вкл/выкл, ПКМ — настройки (ползунки).
Конфиг: `config/dobri_visual/config.json` (автосохранение, при повреждении файл копируется в .bak и берутся значения по умолчанию).
## Сборка
GitHub: залей проект вместе с `.github`, вкладка Actions -> build -> артефакт `dobri-visual-jar`.
Локально: Java 21 + Gradle 8.14+, `gradle build` -> `build/libs/`. Версии в `gradle.properties` сверь с https://fabricmc.net/develop/
## Модули
Combat Visuals: Auto Armor (пустые слоты, shift-клик), Custom Crosshair. Render: NoRender (частицы: дождевые брызги, порталы, дым, огонь, взрывы, пепел).
World: Color Filter (+яркость), Fog Haze (экранная дымка). HUD: FPS, Coordinates, Direction, Clock, Session Timer, Speed, CPS, Keystrokes, Armor HUD (масштаб, прозрачность, HUD Editor).
Movement: Freelook (удержание клавиши, по умолчанию Left Alt). Cosmetics: Hat (Top Hat, Crown, Wizard Hat, Cat Ears, Halo) и Wings (Angel, Demon, Butterfly) — 3D-модели на игроке, плюс Jump Circle, Particles, Aura, Trail, Orbits. Всё локально, видно только тебе.
Settings: 10 тем (в т.ч. Liquid Glass), HUD Editor, Keybinds (защита от конфликтов, сброс), Reset Config.
## Ограничения
Не реализовано: настоящие небо/туман (нужны миксины рендера, не проверенные для 1.21.11), скрытие дождя/снега и портального оверлея, свой цветовой пикер/HEX, поиск по модулям, Target HUD, TNT Timer, звуки критов, Potion HUD, экспорт/импорт профилей в GUI (методы есть в Config).
Проект не компилировался и не запускался в среде разработки (нет доступа к сети).
