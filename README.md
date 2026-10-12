# Artastasia — бесплатный сайт-видеоархив

## Файлы
- `index.html` — главная страница, поиск, сортировка и встроенный YouTube-плеер.
- `config.js` — место для YouTube Data API key.

## Подключение полного каталога видео
1. Открой https://console.cloud.google.com/ и создай проект.
2. В APIs & Services → Library включи **YouTube Data API v3**.
3. В APIs & Services → Credentials создай **API key**.
4. Вставь ключ в `config.js` вместо `PASTE_YOUR_YOUTUBE_DATA_API_KEY_HERE`.
5. После публикации обязательно ограничь ключ: Websites / HTTP referrers — добавь адрес GitHub Pages; API restrictions — разреши только YouTube Data API v3.

Ключ в статическом сайте виден посетителям, поэтому обязательно ограничь его доменом и API. Не отправляй ключ в чат.

## Публикация на GitHub Pages
1. В репозитории нажми **Add file → Upload files**.
2. Загрузи `index.html` и `config.js` (можно также `README.md`).
3. Нажми **Commit changes**.
4. Открой **Settings → Pages**.
5. В **Build and deployment** выбери **Deploy from a branch**, ветка `main`, папка `/(root)`, нажми **Save**.
6. Подожди появления адреса сайта в разделе Pages.

Каталог после подключения API будет загружать публичные видео канала `@artastasia`, включая старые публикации; новые появятся при следующем посещении/обновлении сайта. Приватные видео не показываются. Видео остаются на YouTube.
