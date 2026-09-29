# Инструкция по бесплатному деплою Bridge Page (Сайта-прокладки)

Сайт находится в папке: `bridge_page/` (главный файл: `index.html`).

---

## Вариант 1: Деплой через Vercel CLI (Самый быстрый, 1 минута)

1. Откройте терминал (PowerShell / Command Prompt) в папке `bridge_page`:
   ```bash
   cd "H:\PROEKTY\МОЁ_GPT_ПРОСТРАНСТВО\PROJECT-Pinterest\Pinterest\PROJECT\bridge_page"
   ```
2. Выполните команду (если Vercel CLI не установлен, npx запустит его автоматически):
   ```bash
   npx vercel
   ```
3. Следуйте простым подсказкам в терминале:
   - `Set up and deploy?` — Нажмите `Y`
   - `Which scope do you want to deploy to?` — Выберите ваш аккаунт Vercel
   - `Link to existing project?` — Нажмите `N`
   - `What's your project's name?` — Введите имя (например: `typecraft-fonts` или `canva-aesthetic-fonts`)
   - `In which directory is your code located?` — Оставьте `./` (просто Enter)
4. Через 10–15 секунд вы получите готовый публичный HTTPS URL вида:
   `https://typecraft-fonts.vercel.app`

---

## Вариант 2: Деплой через GitHub + Vercel Dashboard (Рекомендуется для удобства обновлений)

1. Создайте бесплатный публичный или приватный репозиторий на [GitHub](https://github.com/new) (например, `pinterest-bridge-page`).
2. Загрузите файлы из папки `bridge_page/` (файл `index.html`) в репозиторий.
3. Перейдите на [Vercel](https://vercel.com) и нажмите **"Add New..." -> "Project"**.
4. Выберите созданный репозиторий и нажмите **"Deploy"**.
5. Vercel автоматически развернет статический сайт за 10 секунд и выдаст постоянный бесплатный домен с SSL-сертификатом (HTTPS).

---

## Вариант 3: Бесплатный хостинг GitHub Pages (Альтернатива)

1. В репозитории GitHub перейдите в **Settings** -> **Pages**.
2. В секции **Branch** выберите `main` и папку `/ (root)`.
3. Нажмите **Save**.
4. Сайт будет доступен по адресу: `https://<ваш_логин>.github.io/<имя_репозитория>/`

---

## Важный шаг после получения ссылки:
Скопируйте полученный домен (например, `https://typecraft-fonts.vercel.app`) и укажите его в `data/pins_metadata.csv` в колонке `link_url` для всех пинов.
