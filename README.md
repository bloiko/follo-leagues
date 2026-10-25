# Follo league packs

Пакети ліг для [Follo](https://github.com/bloiko/follo): одна папка на лігу, у ній `league.json` та емблеми.
У додатку: Налаштування → Ліга → код = назва папки (наприклад `volodymyr-district`).

```json
{
  "league": "Назва турніру (над табло)",
  "version": 1,
  "teams": [
    { "id": "club", "name": "Повна назва", "short": "КОРОТКА", "colour": "#RRGGBB", "emblem": "club.png" }
  ],
  "replay": { "transition": "millWhite", "video": "stinger.mov" }
}
```

- `emblem` — PNG з прозорим фоном, до 512 px, поряд із `league.json` (або повне посилання).
- `colour` — колір форми на табло.
- `replay` — типовий перехід на повтор для цієї ліги (`millWhite`, `mill`, `flip`, `wipe`, `zoom`, `fade`, `card`) або `video` — кліп 1–3 с (HEVC з альфою або mp4). Застосовується один раз при завантаженні; оператор може змінити в налаштуваннях.
- Підняв `version` — телефони підтягнуть зміни при наступному запуску.
