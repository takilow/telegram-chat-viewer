# Telegram Chat Viewer — Tauri project

## Требования
- Node.js + npm
- Rust + Cargo (https://www.rust-lang.org/tools/install)
- Tauri CLI ставится через npm (см. ниже), доп. системные зависимости для Windows: Microsoft C++ Build Tools + WebView2 (обычно уже есть в Windows 10/11)

## Сборка
```
npm install
npm run tauri build
```
Готовый `.exe`/`.msi`/`.nsis` появится в `src-tauri/target/release/bundle/`.

## Разработка (запуск без сборки инсталлятора)
```
npm install
npm run dev
```

## Структура
- `src/index.html` — сам вьювер (это тот же файл, что и отдельный telegram_chat_viewer.html)
- `src-tauri/` — код Rust-обёртки и конфиг Tauri
- `src-tauri/icons/` — иконки приложения (сгенерированы из твоего лого)

Если обновишь `telegram_chat_viewer.html`, просто скопируй его поверх `src/index.html` перед сборкой.
