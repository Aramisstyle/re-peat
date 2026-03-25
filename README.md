# Re-Peat.store

## In-Store Conversion + Local SEO Architecture

Re-Peat е статичен маркетинг сайт за second hand и outlet мода в София, изграден с ясна бизнес цел: **реални посещения в обектите**, а не онлайн checkout.

Платформата е оптимизирана за:

- локално откриване в търсачки
- бърз mobile UX
- директна конверсия към физически локации
- вторичен социален канал чрез Facebook

## Core positioning

- **Primary conversion:** посещение в магазин
- **Secondary conversion:** контакт/ангажиране през Facebook
- **Support conversion:** директно обаждане чрез `tel:` линк

## Technical architecture

- Статичен multi-page сайт: начало, за нас, блог индекс и самостоятелни статии
- Inline critical CSS/JS за бърз first render и минимален overhead
- Zero external dependencies: без framework-и, CDN библиотеки и third-party JS пакети
- Custom SVG icon rendering през vanilla JavaScript
- WebP-first media strategy с fallback логика за по-стари браузъри

## SEO architecture

- Local intent копирайт с фокус върху физически посещения в София
- Пълни метаданни: `title`, `description`, `canonical`, `hreflang`, Open Graph, Twitter Card
- JSON-LD graph със `Organization`, `WebSite`, `ClothingStore` (3 локации), `FAQPage`
- Facebook присъствие и в SEO слоя чрез `sameAs` в structured data
- Локационна структура за:
	- ул. Екзарх Йосиф 10
	- ул. Поп Богомил 52
	- ул. Г. С. Раковски 85

## Performance profile

- Preload на hero изображение
- Lazy loading за второстепенни визуални елементи
- Малък front-end footprint без SPA runtime цена
- Мобилно-оптимизиран interface с ясни CTA елементи

## Conversion and UX logic

- **Primary CTA:** „Виж магазините“ (директен път към локации)
- **Secondary CTA:** Facebook (header, contact секция, mobile floating button)
- **Direct action CTA:** телефонен линк за моментален контакт
- Trust signals: ежедневно зареждане, падащи цени, ръчна селекция, ясно работно време
- FAQ секция за редуциране на бариери преди посещение

## Accessibility and quality

- Подобрена heading йерархия
- Линкове, различими не само по цвят (подчертаване + контраст)
- Семантична HTML структура, съвместима с автоматични accessibility проверки

## Hosting and deployment

- Проектът е подходящ за безплатен static deployment чрез GitHub Pages
- Без backend инфраструктура и без база данни
- Git-based workflow за бързи итерации и контрол на версиите

## Project structure

```text
.
├── index.html
├── about.html
├── blog/
│   ├── index.html
│   ├── kak-rabotyat-namalyavashtite-ceni.html
│   ├── rachno-selektirani-drehi.html
│   └── vsekidnevno-zarezhdane.html
├── robots.txt
├── sitemap.xml
├── site.webmanifest
├── _headers
└── _redirects
```

## Run locally

Опция 1 (VS Code Live Server):

- Отвори `index.html` с Live Server

Опция 2 (Python static server):

```bash
python -m http.server 8080
```

После отвори `http://localhost:8080`.

## Credits and attribution

- **Brand and business:** Re-Peat
- **Website implementation credit:** Mover Studio (https://moverstudio.online)
- **Official social channel used in project:** 
- **Footer attribution in production:** „Уеб изработка: Mover Studio“

## Outcome

Бърз, стабилен и SEO-ориентиран локален сайт, който комбинира:

- силно органично откриване
- ясна in-store конверсионна логика
- secondary Facebook engagement канал
- ниска техническа сложност и лесен deployment
