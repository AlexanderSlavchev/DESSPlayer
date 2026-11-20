# DESSPlayer

Личен онлайн аудио плеър на Десислава. Песните се стриймват директно от Google Drive папка,
така че нова песен, качена в папката, се появява в плеъра автоматично.

## Настройка (еднократно)

1. **Google API ключ** – https://console.cloud.google.com → нов проект → *APIs & Services* →
   *Library* → включи **Google Drive API** → *Credentials* → *Create credentials* → *API key*.
2. Ограничи ключа: *Application restrictions* → **Websites** →
   `https://alexanderslavchev.github.io/*`; *API restrictions* → само **Google Drive API**.
3. Постави ключа в `config.js` (`apiKey`).
4. Папката в Drive трябва да е споделена „Всеки с линка – Читател“.
5. GitHub → *Settings* → *Pages* → *Deploy from a branch* → `main` / `/ (root)`.

Адрес: https://alexanderslavchev.github.io/DESSPlayer/

Без API ключ плеърът чете `songs.json` – списък от `{ "title": "...", "id": "<Drive file ID>" }`.
