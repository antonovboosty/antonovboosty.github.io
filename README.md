# Сайт «Алексей Антонов — Антонов Бусти»

Одностраничный сайт-визитка для личного бренда с полной SEO-оптимизацией
под Google и Яндекс. Хостинг — GitHub Pages (бесплатно).

## Файлы

| Файл | Назначение |
|---|---|
| `index.html` | Главная (и единственная) страница |
| `style.css` | Оформление (тёмная тема, адаптив под телефоны) |
| `og-image.png` | Миниатюра 1200×630 для превью в Telegram, VK, соцсетях |
| `favicon.svg`, `favicon-32.png` | Иконка сайта во вкладке браузера |
| `apple-touch-icon.png` | Иконка при добавлении на главный экран iPhone |
| `robots.txt` | Правила для поисковых роботов |
| `sitemap.xml` | Карта сайта для Google и Яндекса |

## Как опубликовать

1. Зайдите на GitHub в репозиторий `antonov-boosti.github.io`
   (если его нет — создайте: **New repository** → имя `antonov-boosti.github.io` → Public → Create).
2. Нажмите **Add file → Upload files**.
3. Перетащите **все файлы из этой папки** (index.html, style.css, картинки, robots.txt, sitemap.xml).
4. Нажмите **Commit changes**.
5. Через 1–2 минуты сайт доступен по адресу:
   **https://antonov-boosti.github.io**

## После публикации — обязательно для продвижения

1. **Яндекс Вебмастер** — https://webmaster.yandex.ru
   - Добавьте сайт, получите код верификации
   - Раскомментируйте в `index.html` строку `<meta name="yandex-verification" ...>` и впишите код
   - Загрузите свой сайт и отправьте sitemap.xml на индексацию
2. **Google Search Console** — https://search.google.com/search-console
   - То же самое: добавьте сайт, впишите код в `meta name="google-site-verification"`
   - Отправьте `sitemap.xml` и запросите индексацию главной страницы
3. Индексация обычно занимает от 2–3 дней до 2–4 недель.

## Что можно (и нужно) менять

- **Тексты в блоке «Обо мне»** — в `index.html` ищите комментарий `TODO`.
  Именно текст страницы сильнее всего влияет на позиции в поиске.
- **Монограмма «АА»** — если есть своё фото, замените в `index.html` блок
  `<div class="avatar">АА</div>` на `<img class="avatar" src="photo.jpg" alt="Алексей Антонов">`
  и добавьте фото в папку.
- **Если измените адрес сайта** (например, купите домен) — замените
  `antonov-boosti.github.io` на новый адрес в этих местах:
  - `index.html`: теги `canonical`, `og:url`, `og:image`, блок JSON-LD
  - `robots.txt`: строка Sitemap
  - `sitemap.xml`: тег `<loc>`
