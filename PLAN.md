# ПЛАН САЙТА — Beauty by Anna Holod
> Статус: в работе | Дата: 2026-03-17

---

## 🤖 КАК ИСПОЛЬЗОВАТЬ ЭТОТ ФАЙЛ В НОВОЙ СЕССИИ

Если ты — новая сессия Claude Code, прочитай этот файл полностью.
Он содержит всё что нужно: архитектуру, дизайн, SEO-план, тексты и статус работы.

**Рабочая папка проекта:** `/Users/vs/Desktop/HOL/beauty-by-anna-holod-com`

**Что уже сделано:**
- ✅ Папка `images/` укомплектована (21 файл, все в латинице, без кириллицы)
- ✅ PLAN.md написан и утверждён
- ✅ Изображения подобраны и переименованы
- ✅ `style.css` создан (цвета, типографика, все компоненты, адаптив)
- ✅ `script.js` создан (язык EN/RU + hamburger + FAQ accordion + scroll reveal)
- ✅ `index.html` создан (главная, полный SEO-текст, schema.org, все блоки)
- ✅ `about.html` создан (о студии, команда Анна + Екатерина)
- ✅ `contact.html` создан (адрес, карта, кнопки, FAQ запись)
- ✅ `sitemap.xml` создан (все 9 страниц с priority)
- ✅ `robots.txt` создан

**Перед началом работы прочитай:**
1. Раздел **"СЕССИИ"** ниже — найди свою сессию и список задач
2. Раздел **"КРИТИЧЕСКИЕ РЕШЕНИЯ"** — обязательные правила
3. Раздел **"КОМПОНЕНТЫ"** — header и footer одинаковые на всех страницах
4. Раздел **"СХЕМА ЦВЕТОВ"** — все цвета только через CSS-переменные

**НЕ делай в новой сессии:**
- Не читай файлы изображений через Read tool (съедает контекст)
- Не изменяй имена файлов в images/
- Не используй слово "эндосферотерапия" — только "apparatus figure correction"
- Не используй фреймворки, только чистый HTML/CSS/vanilla JS

---

## ⚡ СЕССИИ — РАЗБИВКА РАБОТЫ

### СЕССИЯ 1 — Фундамент (style.css, script.js, index.html, about, contact, sitemap)
**Статус:** ✅ Сессия 1 завершена

**Задачи по порядку:**
1. `style.css` — весь дизайн: переменные, типографика, header, footer, все компоненты, адаптив
2. `script.js` — ~40 строк: переключатель EN/RU + hamburger меню
3. `index.html` — главная страница, 1000–1300 слов EN
4. `about.html` — о студии, 600–800 слов EN
5. `contact.html` — контакты, 350–500 слов EN
6. `sitemap.xml` — все 9 страниц
7. `robots.txt`

**После завершения обнови статус:** ✅ Сессия 1 завершена

---

### СЕССИЯ 2 — Страницы услуг, часть 1
**Статус:** ⬜ не начата (начинать только после ✅ Сессии 1)

**Задачи по порядку:**
1. `manicure.html` — 900–1100 слов EN
2. `massage.html` — 950–1150 слов EN
3. `waxing.html` — 800–1000 слов EN
4. `body.html` — 900–1100 слов EN

**Перед началом:** прочти style.css чтобы знать доступные классы.
Не открывай index.html — он большой, потратит контекст.

**После завершения обнови статус:** ✅ Сессия 2 завершена

---

### СЕССИЯ 3 — Страницы услуг, часть 2 + финальная проверка
**Статус:** ⬜ не начата (начинать только после ✅ Сессии 2)

**Задачи по порядку:**
1. `brows.html` — 750–950 слов EN
2. `hair.html` — 950–1150 слов EN
3. Финальная проверка: запусти `ls -la` в папке проекта, убедись что все 13 файлов созданы
4. Проверь что во всех HTML есть: `<title>`, `<meta description>`, `canonical`, schema.org, OpenGraph

**После завершения обнови статус:** ✅ Сессия 3 завершена — САЙТ ГОТОВ

---

## 📁 ИЗОБРАЖЕНИЯ (уже готовы, не трогать)

```
images/
├── hero.jpg            → главная, hero секция
├── studio-1.jpg        → about, интерьер студии
├── manicure-1.jpg      → маникюр
├── manicure-2.jpg      → маникюр
├── manicure-3.jpg      → маникюр
├── massage-1.jpg       → массаж
├── massage-2.jpg       → массаж
├── massage-3.jpg       → массаж
├── massage-4.jpg       → массаж
├── massage-5.jpg       → массаж
├── hair-1.jpg          → волосы
├── hair-2.jpg          → волосы
├── hair-3.jpg          → волосы
├── waxing-1.jpg        → депиляция/шугаринг
├── waxing-2.jpg        → депиляция/шугаринг
├── waxing-3.jpg        → депиляция/шугаринг
├── body-1.jpg          → обёртывания
├── body-2.jpg          → обёртывания
├── body-3.jpg          → обёртывания
├── body-4.jpg          → коррекция фигуры
└── about-studio.png    → about страница
```

> Фото для brows.html нет — используй `studio-1.jpg` или `about-studio.png` как fallback.

---

---

## 1. СТРУКТУРА ПРОЕКТА

```
beauty-by-anna-holod-com/
├── index.html
├── manicure.html
├── waxing.html
├── massage.html
├── body.html
├── brows.html
├── hair.html
├── about.html
├── contact.html
├── style.css
├── script.js          ← только: язык + hamburger (~40 строк)
├── sitemap.xml
├── robots.txt
├── favicon.ico        ← placeholder
└── images/
    ├── hero.jpg           → использовать: images/massage-1.jpg (пока)
    ├── manicure-1.jpg     ✓ есть
    ├── manicure-2.jpg     ✓ есть
    ├── manicure-3.jpg     ✓ есть
    ├── massage-1.jpg      ✓ есть
    ├── massage-2.jpg      ✓ есть
    ├── massage-3.jpg      ✓ есть
    ├── massage-4.jpg      ✓ есть
    ├── massage-5.jpg      ✓ есть
    ├── hair-1.jpg         ✓ есть
    ├── hair-2.jpg         ✓ есть
    ├── hair-3.jpg         ✓ есть
    ├── about-studio.png   ✓ есть
    ├── waxing-1.jpg       ← нужно скопировать из instagramm/
    ├── body-1.jpg         ← нужно скопировать из instagramm/
    ├── body-2.jpg         ← нужно скопировать из instagramm/
    ├── brows-1.jpg        ← placeholder (фото нет в проекте)
    └── studio-1.jpg       ← использовать: instagramm/интерьер.jpg
```

### Источники изображений из instagramm/фото услуг работ/:
| Файл | Куда копировать | Назначение |
|------|----------------|------------|
| депиляция.jpg | images/waxing-1.jpg | страница депиляции |
| депилция.jpg | images/waxing-2.jpg | страница депиляции (дубль) |
| шугаринг.jpg | images/waxing-3.jpg | страница шугаринга |
| обертывание2.jpg | images/body-1.jpg | страница тела |
| обертывание3.jpg | images/body-2.jpg | страница тела |
| обнртывание.jpg | images/body-3.jpg | страница тела |
| аппаратная коррекция.jpg | images/body-4.jpg | коррекция фигуры |
| интерьер.jpg | images/studio-1.jpg | about, главная |

> ⚠️ Файлы с кириллицей в именах нужно переименовать перед деплоем на GitHub Pages

---

## 2. ТЕХНИЧЕСКИЙ СТЕК

| Параметр | Решение | Причина |
|----------|---------|---------|
| HTML | семантический HTML5 | SEO, доступность |
| CSS | чистый CSS, BEM-нейминг | без фреймворков |
| JS | ~40 строк vanilla | язык + hamburger меню |
| Шрифты | Google Fonts: Cormorant Garamond + Lato | элегантность + читаемость |
| Иконки | inline SVG | скорость, без запросов |
| Изображения | реальные JPG из проекта | конверсия |
| Карта | Google Maps iframe (статичный) | контакты |
| Хостинг | GitHub Pages | по ТЗ |

### Производительность:
- `<link rel="preload">` для hero изображения
- `loading="lazy"` на все остальные `<img>`
- CSS минимизирован, без неиспользуемых правил
- Один CSS-файл (без @import цепочек)
- Шрифты: только нужные начертания (400, 500, 600)

---

## 3. SEO-АРХИТЕКТУРА

### Технические SEO-элементы (каждая страница):
- `<title>` уникальный
- `<meta name="description">` уникальный, 150-160 символов
- `<meta name="robots" content="index, follow">`
- `<link rel="canonical">`
- `<html lang="en">`
- OpenGraph теги (og:title, og:description, og:image, og:url)
- H1 → H2 → H3 строго по иерархии (один H1 на страницу)
- Schema.org JSON-LD (LocalBusiness на всех страницах)
- FAQ Schema на страницах услуг

### Внутренняя перелинковка:
Каждая страница услуги → ссылки на 3 другие услуги (блок "You may also like")

### sitemap.xml:
Все 9 страниц с `<lastmod>` и `<priority>`

### robots.txt:
```
User-agent: *
Allow: /
Sitemap: https://beautybyanna.com/sitemap.xml
```

---

## 4. ЯЗЫКОВОЕ РЕШЕНИЕ

**Реализация**: ~15 строк JS + CSS data-атрибуты

```html
<!-- Шапка -->
<button onclick="switchLang('en')" class="lang-btn">EN</button>
<button onclick="switchLang('ru')" class="lang-btn">RU</button>

<!-- Контент -->
<p data-en="Welcome to our studio" data-ru="Добро пожаловать в студию"></p>
```

```js
function switchLang(lang) {
  localStorage.setItem('lang', lang);
  document.querySelectorAll('[data-en]').forEach(el => {
    el.textContent = el.dataset[lang];
  });
}
```

**Правило**: Весь основной SEO-текст — на английском. Русский — дублирующий слой. Google индексирует английскую версию как основную.

---

## 5. ЦВЕТОВАЯ ГАММА И ДИЗАЙН

```css
:root {
  --color-bg:        #FAF8F5;   /* тёплый белый фон */
  --color-surface:   #F5F0EA;   /* карточки, секции */
  --color-border:    #E8DDD0;   /* разделители */
  --color-text:      #3D3530;   /* основной текст */
  --color-text-muted:#8C7B70;   /* второстепенный */
  --color-accent:    #C9A882;   /* золотисто-бежевый */
  --color-accent-2:  #D4A5A0;   /* нюдово-розовый */
  --color-cta:       #8B5E4A;   /* кнопки CTA */
  --color-cta-hover: #6B4535;   /* hover кнопок */
}
```

**Типографика:**
- Заголовки: `Cormorant Garamond` (элегантность)
- Текст: `Lato` (читаемость)
- H1: 2.5rem mobile → 3.5rem desktop
- Body: 16px / line-height 1.7

---

## 6. ПОСТРАНИЧНЫЙ ПЛАН

---

### index.html — Главная
**Title**: `Beauty Salon in Limassol | Beauty by Anna Holod — Professional Beauty Studio`
**Description**: `Beauty by Anna Holod — professional beauty studio in Limassol. Manicure, massage, waxing, hair, body treatments. Book via Instagram or WhatsApp. Arch. Makarios III, 161.`
**H1**: `Professional Beauty Studio in Limassol`

**Блоки страницы:**
1. **Hero** — фото студии/массажа, H1, подзаголовок, 2 CTA кнопки (Book via Instagram / WhatsApp)
2. **Positioning** — 3–4 предложения о студии, ключи: beauty studio Limassol, beauty services Limassol
3. **Services grid** — 7 карточек с фото и ссылками на страницы услуг
4. **Why choose us** — 6 преимуществ из реальных отзывов (иконки + текст)
5. **Reviews** — 5 реальных Google-отзывов (слайдер или сетка)
6. **Gallery** — сетка 6–9 фото
7. **Video placeholder** — атмосфера студии, ссылка на Instagram
8. **FAQ** — 5 вопросов
9. **CTA section** — запись
10. **Contact mini-block** — адрес, телефон, часы

**Word count цель**: 1000–1300 слов EN

**FAQ вопросы:**
- Where is Beauty by Anna Holod studio located in Limassol?
- Do I need to book an appointment in advance?
- What languages do your specialists speak?
- How many beauty specialists work at the studio?
- What payment methods do you accept?

---

### manicure.html — Маникюр и педикюр
**Title**: `Manicure & Pedicure in Limassol | Nail Salon — Beauty by Anna Holod`
**Description**: `Professional manicure and pedicure in Limassol. Gel polish, hardware pedicure, nail art. Clean tools, lasting results. Book at Beauty by Anna Holod on Makarios III.`
**H1**: `Manicure & Pedicure in Limassol — Professional Nail Care`

**Блоки**: Hero → Intro SEO text → Что включает (gel, classic, hardware pedicure, nail art) → Для кого → Результат → Почему у нас → Gallery (3 фото) → Video placeholder → FAQ → CTA → Mini contact → Другие услуги

**Ключевые смыслы**: гигиена (одноразовые материалы), скорость, долговечность, из отзыва Ксении — "профессионально, быстро и красиво"

**FAQ:**
- How long does gel manicure last?
- Do you use disposable files and tools?
- Can I book manicure and pedicure together in one session?
- What nail polish brands do you use?
- How long does a full manicure + pedicure session take?

**Word count цель**: 900–1100 слов EN

---

### waxing.html — Депиляция и шугаринг
**Title**: `Waxing & Sugaring in Limassol | Hair Removal — Beauty by Anna Holod`
**Description**: `Smooth skin all year round. Professional waxing and sugaring in Limassol at Beauty by Anna Holod. Gentle hair removal for face and body. Book now on Makarios III.`
**H1**: `Waxing & Sugaring in Limassol — Smooth Skin All Year Round`

**Уникальный угол**: Кипр = жара круглый год → депиляция актуальна 365 дней. Мягкость шугаринга для чувствительной кожи.

**FAQ:**
- What is the difference between waxing and sugaring?
- How long does hair removal last?
- Can I sunbathe after waxing in Limassol?
- Is sugaring suitable for sensitive skin?
- How often should I book hair removal sessions?

**Word count цель**: 800–1000 слов EN

---

### massage.html — Массаж
**Title**: `Massage in Limassol | Anti-Cellulite & Lymphatic Drainage — Beauty by Anna Holod`
**Description**: `Professional massage in Limassol: relaxation, anti-cellulite, lymphatic drainage. Certified specialist Anna Holod. Visible results from first session. Book now.`
**H1**: `Professional Massage in Limassol — Relaxation, Recovery & Body Care`

**Ключевые смыслы**: Анна Холод — сертифицированный специалист, владелица, сама проводит сеансы. Из отзыва Аллы: "Анна спасала мою спину от боли". Конкретные виды: relaxation, anti-cellulite, lymphatic drainage.

**FAQ:**
- What types of massage do you offer in Limassol?
- How many sessions do I need to see visible results?
- Is anti-cellulite massage painful?
- Can I combine massage with body wraps?
- Who performs the massage — a certified specialist?

**Word count цель**: 950–1150 слов EN

---

### body.html — Обёртывания и коррекция фигуры
**Title**: `Body Wraps & Figure Correction in Limassol | Body Treatments — Beauty by Anna Holod`
**Description**: `Body wraps, body treatments and figure correction in Limassol. Reduce swelling, improve skin tone, visible results from first session. Beauty by Anna Holod, Makarios III.`
**H1**: `Body Wraps & Figure Correction in Limassol`

**Ключевые смыслы**: Из отзыва Ольги Чик — конкретные результаты: "ушли отёки, влезла в старые джинсы, кожа стала упругой". Из отзыва Алёны: "вода ушла за первый сеанс". Аппаратная коррекция фигуры (НЕ эндосферотерапия — запрещено).

**FAQ:**
- How many body wrap sessions do I need for results?
- What is body wrap and how does it work?
- What is apparatus figure correction?
- Are body treatments suitable during summer in Cyprus?
- Can I combine body wraps with massage?

**Word count цель**: 900–1100 слов EN

---

### brows.html — Оформление бровей
**Title**: `Eyebrow Shaping & Styling in Limassol | Brow Correction — Beauty by Anna Holod`
**Description**: `Professional eyebrow shaping and brow correction in Limassol. Natural-looking results, brow tinting, precise styling. Book at Beauty by Anna Holod on Makarios III.`
**H1**: `Eyebrow Shaping & Styling in Limassol — Natural, Defined Brows`

**Уникальный угол**: брови без татуажа — только уход, коррекция, натуральный результат. "Правильные брови меняют лицо".

**FAQ:**
- How often should I get brow correction?
- Do you offer brow tinting at the studio?
- What is the difference between wax and thread brow shaping?
- How long does eyebrow shaping take?
- Can you reshape overgrown brows?

**Word count цель**: 750–950 слов EN

---

### hair.html — Волосы
**Title**: `Hair Salon in Limassol | Haircut, Coloring & Styling — Beauty by Anna Holod`
**Description**: `Professional hair salon in Limassol. Haircuts, balayage, highlights, hair coloring and styling. Specialist Ekaterina. Book at Beauty by Anna Holod on Makarios III.`
**H1**: `Hair Salon in Limassol — Cuts, Coloring & Expert Styling`

**Ключевые смыслы**: специалист Екатерина, из отзыва Натальи Шугриной — "наконец нашла грамотного мастера-колориста на Кипре". Из отзыва Анны Золкиной — "учитывают пожелания, даже когда торопишься". Акцент: балаяж, мелирование, восстановление повреждённых волос.

**FAQ:**
- Do you do balayage and highlights in Limassol?
- How long does hair coloring take?
- Can you fix a bad color from another salon?
- Do I need a consultation before hair coloring?
- What hair care products do you use?

**Word count цель**: 950–1150 слов EN

---

### about.html — О студии
**Title**: `About Beauty by Anna Holod | Beauty Studio in Limassol — Our Team & Values`
**Description**: `Beauty by Anna Holod — a professional beauty studio in Limassol with a team of specialists. Learn about our team, values and approach. Arch. Makarios III, 161.`
**H1**: `About Beauty by Anna Holod — Beauty Studio in Limassol`

**Структура текста:**
- История студии и концепция
- Команда: Анна Холод (основательница, массаж, тело), Екатерина (волосы, колорист)
- Ценности: чистота, профессионализм, результат, атмосфера
- Расположение и удобство (Макариос — центральная улица)
- CTA блок

**Word count цель**: 600–800 слов EN

---

### contact.html — Контакты
**Title**: `Contact Beauty by Anna Holod | Book Appointment in Limassol`
**Description**: `Contact Beauty by Anna Holod beauty studio in Limassol. Call, WhatsApp or book via Instagram. Address: Arch. Makarios III Ave 161, Limassol, Cyprus.`
**H1**: `Contact Us — Book Your Appointment at Beauty by Anna Holod`

**Блоки:**
- Адрес + схема проезда (Google Maps iframe)
- Часы работы (placeholder)
- Телефон + WhatsApp + Instagram (крупные кнопки)
- Мини-FAQ про запись

**Word count цель**: 350–500 слов EN

---

## 7. КОМПОНЕНТЫ (повторяются на всех страницах)

### Header (одинаковый на всех страницах):
```
[Логотип — текст: Beauty by Anna Holod]    [Телефон]  [EN | RU]  [☰]
НАВИГАЦИЯ: Home | Manicure | Waxing | Massage | Body | Brows | Hair | About | Contact
```
- Sticky header (прилипает при скролле)
- Hamburger меню на mobile

### Footer (одинаковый на всех страницах):
```
Beauty by Anna Holod
Arch. Makarios III Ave 161, Limassol, Cyprus
📞 +357 XXX XXX XXX
📱 WhatsApp: +357 XXX XXX XXX
📷 Instagram: @beauty_by_anna_holod
🕐 Mon–Sat: [HOURS] | Sun: [HOURS]
---
© 2024 Beauty by Anna Holod. All rights reserved.
```

### CTA блок (каждая страница):
```
Ready to book?
[📞 Call Now]  [💬 WhatsApp]  [📷 Book via Instagram]
```

### Mini contact блок (каждая страница услуг):
```
📍 Arch. Makarios III Ave 161, Limassol
📞 +357 XXX XXX XXX
```

---

## 8. SCHEMA.ORG (JSON-LD на каждой странице)

```json
{
  "@context": "https://schema.org",
  "@type": "BeautySalon",
  "name": "Beauty by Anna Holod",
  "url": "https://beautybyanna.com",
  "telephone": "+357XXXXXXXXX",
  "address": {
    "@type": "PostalAddress",
    "streetAddress": "Arch. Makarios III Avenue 161",
    "addressLocality": "Limassol",
    "addressCountry": "CY",
    "postalCode": "3090"
  },
  "geo": {
    "@type": "GeoCoordinates",
    "latitude": "34.6751",
    "longitude": "33.0441"
  },
  "sameAs": ["https://www.instagram.com/beauty_by_anna_holod/"],
  "openingHours": ["Mo-Sa 09:00-20:00"],
  "priceRange": "€€",
  "image": "https://beautybyanna.com/images/studio-1.jpg",
  "areaServed": "Limassol, Cyprus"
}
```

### FAQ Schema (страницы услуг):
```json
{
  "@type": "FAQPage",
  "mainEntity": [...]
}
```

---

## 9. ПЕРЕЧЕНЬ ФАЙЛОВ ДЛЯ СОЗДАНИЯ

| # | Файл | Сессия | Статус |
|---|------|--------|--------|
| 1 | style.css | 1 | ✅ готов |
| 2 | script.js | 1 | ✅ готов |
| 3 | index.html | 1 | ✅ готов |
| 4 | about.html | 1 | ✅ готов |
| 5 | contact.html | 1 | ✅ готов |
| 6 | sitemap.xml | 1 | ✅ готов |
| 7 | robots.txt | 1 | ✅ готов |
| 8 | manicure.html | 2 | ⬜ не начат |
| 9 | massage.html | 2 | ⬜ не начат |
| 10 | waxing.html | 2 | ⬜ не начат |
| 11 | body.html | 2 | ⬜ не начат |
| 12 | brows.html | 3 | ⬜ не начат |
| 13 | hair.html | 3 | ⬜ не начат |

---

## 10. КРИТИЧЕСКИЕ РЕШЕНИЯ (зафиксированы)

| Вопрос | Решение |
|--------|---------|
| Язык SEO | EN основной, RU дублирующий слой через data-атрибуты |
| Реальные фото | Использовать из `/images/` и `/instagramm/` |
| HEIC файлы | Не использовать (нет браузерной поддержки) |
| Видео | Placeholder-блоки со ссылкой на Instagram вместо пустых iframe |
| "Эндосферотерапия" | Заменить на "apparatus figure correction" |
| Имена файлов | Переименовать все кириллические имена перед деплоем |
| JS объём | Максимум ~40 строк, только язык + hamburger |
| Hero фото | images/massage-1.jpg или studio-1.jpg (интерьер) |

---

## 11. ПРОМТ ДЛЯ ЗАПУСКА КАЖДОЙ СЕССИИ

Скопируй нужный блок и вставь в новую сессию Claude Code.

---

### 🟢 Промт для Сессии 1

```
Рабочая папка: /Users/vs/Desktop/HOL/beauty-by-anna-holod-com

Прочитай файл PLAN.md — он содержит всю архитектуру, дизайн и SEO-план сайта.

Твоя задача — Сессия 1 из раздела "СЕССИИ":
1. style.css
2. script.js
3. index.html
4. about.html
5. contact.html
6. sitemap.xml
7. robots.txt

Строго следуй разделам: ЦВЕТОВАЯ ГАММА, КОМПОНЕНТЫ, SCHEMA.ORG, SEO-АРХИТЕКТУРА.
Не читай файлы изображений через Read tool.
После создания каждого файла обнови статус в таблице раздела 9 в PLAN.md: ⬜ → ✅
После завершения всех 7 файлов обнови статус Сессии 1 в PLAN.md на: ✅ Сессия 1 завершена
```

---

### 🟡 Промт для Сессии 2

```
Рабочая папка: /Users/vs/Desktop/HOL/beauty-by-anna-holod-com

Прочитай файл PLAN.md — он содержит всю архитектуру, дизайн и SEO-план сайта.
Затем прочитай style.css чтобы знать доступные классы (но не читай HTML файлы — они большие).

Твоя задача — Сессия 2 из раздела "СЕССИИ":
1. manicure.html
2. massage.html
3. waxing.html
4. body.html

Для каждой страницы строго следуй её разделу в PLAN.md:
Title, Description, H1, блоки, FAQ вопросы, ключевые смыслы, word count.
Структура каждой страницы: Hero → SEO intro → Что включает → Для кого → Результат → Почему у нас → Gallery → Video placeholder → FAQ → CTA → Mini contact → Другие услуги.
Не читай файлы изображений через Read tool.
После создания каждого файла обнови статус в таблице раздела 9 в PLAN.md: ⬜ → ✅
После завершения всех 4 файлов обнови статус Сессии 2 в PLAN.md на: ✅ Сессия 2 завершена
```

---

### 🔴 Промт для Сессии 3

```
Рабочая папка: /Users/vs/Desktop/HOL/beauty-by-anna-holod-com

Прочитай файл PLAN.md — он содержит всю архитектуру, дизайн и SEO-план сайта.
Затем прочитай style.css чтобы знать доступные классы (но не читай другие HTML файлы).

Твоя задача — Сессия 3 из раздела "СЕССИИ":
1. brows.html
2. hair.html
3. Финальная проверка: ls -la в корне проекта — убедись что все 13 файлов созданы
4. Проверь что во всех HTML-файлах есть: <title>, <meta description>, canonical, schema.org JSON-LD, OpenGraph теги

Для каждой страницы строго следуй её разделу в PLAN.md.
Не читай файлы изображений через Read tool.
После создания каждого файла обнови статус в таблице раздела 9 в PLAN.md: ⬜ → ✅
После завершения обнови статус Сессии 3 в PLAN.md на: ✅ Сессия 3 завершена — САЙТ ГОТОВ
```

---

*Документ обновляется по мере разработки.*
