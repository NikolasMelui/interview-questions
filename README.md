# 📟 Список вопросов для технического интервью

Список для подготовки и проведения собеседований программистов. На одном интервью обычно выбирают **10–20 вопросов** из разных разделов — под уровень кандидата и стек вакансии.

**Уровни сложности** (внутри разделов — от простого к сложному):

- 🟢 базовый — junior, проверка фундамента
- 🟡 средний — middle, опыт и понимание «как устроено»
- 🔴 продвинутый — senior, глубина, trade-offs, продакшен

---

## О себе и мотивация

- 🟢 Расскажи о себе: образование, опыт в разработке, чем занимаешься сейчас.
- 🟢 Чем занимаешься вне работы? Есть ли хобби, связанное с профессией?
- 🟢 Какие у тебя планы и ожидания на ближайшие 1–2 года?
- 🟡 Расскажи про сильные и слабые стороны как разработчика. Над чем работаешь?
- 🟡 Какое образование и дополнительное обучение (курсы, пет-проекты, open source)?

## Смена места работы

- 🟢 Почему ищешь новую работу? Что не устраивает на текущем месте?
- 🟢 Расскажи про последнее место работы: роль, срок, зона ответственности, стек.
- 🟢 Что привлекло в нашей компании и в этой позиции?
- 🟡 Какие цели видишь на испытательном сроке и через год?
- 🟡 Как проходило твоё собеседование на прошлую работу? Что бы улучшил в процессе найма?

## Путь в профессию

- 🟢 Как попал в разработку? Сколько лет в профессии?
- 🟢 Как учился: источники, баланс теории и практики, первый коммерческий опыт.
- 🟡 Расскажи про самый значимый проект или фичу, которую делал от идеи до продакшена.

## Опыт и технологии

- 🟢 С каким стеком работал на коммерческих проектах? Что нравилось и что нет?
- 🟢 В каких проектах участвовал? Какую роль и какие задачи выполнял?
- 🟡 С какими техническими проблемами сталкивался? Как диагностировал и решал?
- 🟡 Какие организационные проблемы встречал (процессы, приоритеты, коммуникация)? Как с ними справлялся?
- 🟡 Самое серьёзное техническое достижение: что сделал, какой был эффект для команды/бизнеса?
- 🟡 Что чаще всего вызывает затруднения? Как готовишься к таким задачам на новом месте?
- 🟡 Любимый язык/стек и почему. Что бы выбрал для нового проекта с нуля?

## Опыт руководства (если релевантно)

- 🟢 Был ли опыт тимлида/менторства? Чем занимался помимо кода?
- 🟡 Как устроены были процессы: оценка задач, планирование, дейли, ретро?
- 🟡 Проводил ли собеседования? Какие вопросы задаёшь кандидатам?
- 🟡 Конфликт в команде, срыв сроков от бизнеса, болезнь ключевого человека — как действовал?
- 🔴 Увольнения и удержание: приходилось ли увольнять или удерживать? Как давал обратную связь?

## Иностранные языки

- 🟢 Уровень английского. Читаешь ли документацию и треды без переводчика?
- 🟡 Можешь ли обсудить техническую задачу устно или в переписке (issue, PR)?
- 🟡 Какие другие языки знаешь и на каком уровне?

## Обучение и развитие

- 🟢 Что изучал за последние 6–12 месяцев? Применял ли на работе?
- 🟢 Какими ресурсами пользуешься (книги, документация, курсы, конференции)?
- 🟡 Интересны ли смежные области (фронт/бэк/инфра)? Был ли опыт за пределами основной роли?
- 🟡 Готов ли инвестировать в обучение? Нужна ли поддержка от компании (курсы, конференции)?

## Организационные вопросы

- 🟢 Когда готов выйти на работу?
- 🟢 Ожидания по зарплате и формат работы (офис / гибрид / удалёнка).
- 🟡 Отношение к испытательному сроку и к редким переработкам — когда они оправданы?

---

## Базовая архитектура приложения

- 🟢 Клиент и сервер: кто инициирует запрос, что такое stateless HTTP.
- 🟢 Что происходит при вводе URL в браузере (упрощённо: DNS → TCP → HTTP → рендер).
- 🟢 Статический сайт, SPA, MPA, SSR, SSG, ISR — отличия и примеры.
- 🟢 Frontend vs backend vs fullstack — зона ответственности каждого.
- 🟢 Монолит vs микросервисы — в двух словах, плюсы и минусы.
- 🟡 Синхронный запрос к API vs фоновая обработка (очередь, webhook).
- 🟡 Reverse proxy и load balancer: nginx, HAProxy — зачем перед приложением.
- 🟡 API Gateway, BFF (Backend for Frontend) — когда нужны.
- 🟡 Слои приложения: presentation → business → data access — зачем разделять.
- 🟡 MVC на примере веб-приложения: где controller, view, model.
- 🟡 Stateless JWT vs server-side session — trade-offs.
- 🟡 Файловое хранилище: локальный диск vs S3-совместимое object storage.
- 🟡 CDN: что кэшируется, cache miss, инвалидация.
- 🟡 Версионирование API: URL (`/v2`), header, query — что выбирал.
- 🟡 Идемпотентность и повтор запросов (сеть оборвалась — клиент ретраит).
- 🟡 Feature flags и постепенный rollout без отдельного деплоя фронта.
- 🟡 Миграция с монолита: strangler fig pattern — слышал ли, применял ли.
- 🟡 Event-driven между сервисами: sync REST vs async messaging.
- 🟡 CAP и выбор БД в распределённой системе — практический смысл.
- 🟡 Observability: логи, метрики, трейсы — зачем три столпа.
- 🟡 Подготовка к новому проекту: README, env example, docker-compose, первый PR.
- 🟡 Документация архитектуры: ADR, C4, диаграмма компонентов — что использовали.
- 🔴 Спроектируй высокоуровнево: интернет-магазин (каталог, корзина, оплата, уведомления).
- 🔴 Как бы разделил монолитный Laravel/Node на сервисы — с чего начать.
- 🔴 Схема отказоустойчивости: что если упала БД, кэш, один из микросервисов.

## HTML

- 🟢 Что такое HTML и для чего он нужен?
- 🟢 Что такое DOCTYPE? Что будет, если его не указать?
- 🟢 Разница между `div` и `span`. Когда использовать каждый?
- 🟢 Семантическая вёрстка: зачем нужна, какие теги знаешь (`header`, `nav`, `main`, `article`…)?
- 🟢 Класс и `id`: отличия, специфичность, типичные ошибки.
- 🟢 Ссылки: типы (`href`, `mailto`, относительные/абсолютные), якорные ссылки.
- 🟢 Списки (`ul`, `ol`, `li`), таблицы (`table`, `tr`, `th`, `td`).
- 🟢 Формы: основные элементы и атрибуты (`input`, `label`, `name`, `required`, `type`).
- 🟢 Зачем `alt` у `img`? Что с доступностью, если `alt` пустой?
- 🟡 Теги `em`, `strong`, `i`, `b`: семантика vs визуальное оформление.
- 🟡 `head`: что обычно указывают (meta, title, link, script)?
- 🟡 Data-атрибуты: зачем и как использовать безопасно?
- 🟡 Подключение скриптов: разница `async` и `defer`.
- 🟡 Многоязычность: `lang`, `hreflang`.
- 🟡 Встроенная валидация в HTML5: какие атрибуты знаешь?
- 🟡 Доступность (a11y): ARIA-роли, `aria-label`, связка `label` + `input`.

## CSS

- 🟢 Что такое CSS и почему таблицы стилей называют «каскадными»?
- 🟢 `margin` и `padding`, `box-sizing: border-box`.
- 🟢 Селекторы: тег, класс, id. Разница `#id` и `.class`.
- 🟢 Свойства `background`: цвет, изображение, `background-size`, `position`.
- 🟢 Комментарии в CSS. Наследование и каскад — в двух словах.
- 🟡 Псевдоклассы и псевдоэлементы: примеры (`:hover`, `::before`).
- 🟡 Flexbox: основные свойства контейнера и элементов.
- 🟡 Grid: когда предпочтёшь grid вместо flex?
- 🟡 Медиа-запросы и адаптивная вёрстка.
- 🟡 `z-index` и контексты наложения (stacking context).
- 🟡 Специфичность и порядок селекторов. Как разрешить конфликт стилей?
- 🟡 Центрирование: по горизонтали и вертикали — известные способы.
- 🟡 `overflow` у `body`/`html` и сохранение скролла.
- 🟡 CSS-анимации и `@keyframes`.
- 🟡 Опыт с SVG в вёрстке.
- 🔴 Что дороже всего для браузера при отрисовке (repaint, reflow, composite)?
- 🔴 Методология БЭМ или другой подход к организации CSS — использовал?

## Препроцессоры и сборка

- 🟢 Зачем нужен bundler в современном фронте?
- 🟢 Dev-сервер vs production build — чем отличаются.
- 🟢 `package.json` scripts: `dev`, `build`, `preview` — что делают.
- 🟡 SASS/SCSS: переменные, nesting, mixins, partials, `@use` vs `@import`.
- 🟡 PostCSS: autoprefixer, postcss-preset-env — зачем поверх CSS.
- 🟡 CSS Modules vs global CSS vs CSS-in-JS — опыт и trade-offs.
- 🟡 Webpack: entry, output, loader, plugin — базовая схема.
- 🟡 Vite: почему быстрее в dev (ESM, esbuild), Rollup на build.
- 🟡 Rollup vs Webpack — когда Rollup уместен (библиотеки).
- 🟡 Tree shaking: условия (ESM, sideEffects в package.json).
- 🟡 Code splitting: dynamic `import()`, vendor chunk, route-based split.
- 🟡 Source maps: `cheap-module-source-map` vs hidden — зачем в prod.
- 🟡 Babel: зачем, presets, polyfills, `@babel/preset-env`.
- 🟡 TypeScript в сборке: `tsc` vs `esbuild`/`swc` transpile only.
- 🟡 Алиасы путей (`@/components`) — как настроить.
- 🟡 Env-переменные: `import.meta.env`, `VITE_`, не утекать секреты на клиент.
- 🟡 Минификация: JS (terser/esbuild), CSS (cssnano), HTML.
- 🟡 Asset pipeline: изображения, шрифты, `url-loader` / встроенные ассеты Vite.
- 🟡 ESLint + Prettier + Stylelint: разделение ролей, конфликт правил.
- 🟡 Husky, lint-staged, commitlint — pre-commit в команде.
- 🟡 CI: `npm ci`, кэш `node_modules`, артефакт `dist/`.
- 🟡 Monorepo: Turborepo, Nx, pnpm workspaces — опыт.
- 🟡 Micro-frontends: Module Federation — знаком ли.
- 🔴 Сборка тормозит 5+ минут — как ускорить (профилирование, cache, split config).
- 🔴 Настрой с нуля Vite + React/Vue + TS + ESLint + path aliases.

## JavaScript

- 🟢 Где выполняется JavaScript (браузер, Node.js, Deno, Bun)?
- 🟢 Примитивные и ссылочные типы. Что такое примитив «по значению» vs объект «по ссылке»?
- 🟢 `var`, `let`, `const` — отличия, TDZ, hoisting.
- 🟢 `==` vs `===`. `null` vs `undefined`. `NaN`.
- 🟢 Массивы: создание, `length`, мутация. `map`, `filter`, `reduce`, `find`, `some`, `every`.
- 🟢 Объекты: литералы, доступ к свойствам, optional chaining (`?.`), nullish coalescing (`??`).
- 🟢 Циклы: `for`, `while`, `for...of`, `for...in` — когда что уместно.
- 🟢 Строки и шаблонные литералы. Базовые методы (`split`, `slice`, `includes`).
- 🟢 Функции: declaration vs expression. Параметры по умолчанию.
- 🟡 Строгая/динамическая/слабая типизация. `typeof`, неявное приведение типов.
- 🟡 Замыкания: определение, пример, утечки памяти через замыкания.
- 🟡 `this`: function, стрелочная функция, метод, `call`/`apply`/`bind`.
- 🟡 Прототипы, цепочка прототипов, `Object.create`, классы ES6 (`extends`, `super`).
- 🟡 Деструктуризация, spread и rest для массивов и объектов.
- 🟡 Императивный vs декларативный стиль. Чистые функции, побочные эффекты.
- 🟡 `Symbol`, `BigInt`, `Map`/`Set` — зачем появились.
- 🟡 Итераторы и генераторы (`function*`, `yield`) — базовое понимание.
- 🟡 Event loop: call stack, очередь задач, microtasks vs macrotasks.
- 🟡 `Promise`: состояния, `then`/`catch`/`finally`, `Promise.all` / `allSettled` / `race`.
- 🟡 `async`/`await`: обработка ошибок, последовательный vs параллельный запуск.
- 🟡 DOM: выбор элементов, изменение атрибутов/классов, создание узлов.
- 🟡 События: bubbling, capturing, `preventDefault`, `stopPropagation`, делегирование.
- 🟡 `fetch`: методы, заголовки, body, обработка HTTP-ошибок (статус ≠ исключение).
- 🟡 JSON: `parse`/`stringify`, циклические ссылки, потеря `undefined`/`Date`.
- 🟡 Модули ESM: `import`/`export`, dynamic `import()`, отличие от CommonJS.
- 🟡 `try/catch/finally`, кастомные ошибки (`Error`, `cause`).
- 🟡 Рекурсия vs итерация. Хвостовая рекурсия — поддерживается ли в JS?
- 🟡 Web Workers / SharedArrayBuffer — когда нужны на фронте.
- 🟡 Proxy и Reflect — для чего используют (фреймворки, валидация).
- 🔴 Реализуй на доске: debounce, throttle, `Promise.all` с лимитом concurrency.
- 🔴 Реализуй простой `EventEmitter` или pub/sub.
- 🔴 Утечки памяти в SPA: detached DOM, глобальные слушатели, замыкания — как искать в DevTools.

## TypeScript

- 🟢 Зачем TypeScript? Что даёт на этапе разработки и в CI.
- 🟢 Примитивы, `string`/`number`/`boolean`, литеральные типы.
- 🟢 `interface` vs `type` — когда что выбрать.
- 🟢 Типизация функций: аргументы, возвращаемое значение, optional/required.
- 🟢 `enum` vs union of literals — плюсы и минусы.
- 🟡 `any`, `unknown`, `never`, `void` — когда что.
- 🟡 Union и intersection types. Discriminated unions — пример.
- 🟡 Type guards: `typeof`, `in`, пользовательские predicates (`value is T`).
- 🟡 Generics: функции, интерфейсы, constraints (`extends`).
- 🟡 `as` assertion — когда опасно, альтернативы.
- 🟡 `readonly`, `const` assertions, иммутабельные типы.
- 🟡 Utility types: `Partial`, `Required`, `Pick`, `Omit`, `Record`, `Exclude`, `Extract`.
- 🟡 `keyof`, indexed access types, mapped types — простой пример.
- 🟡 Перегрузка функций (overloads) — зачем.
- 🟡 `strict`, `strictNullChecks`, `noImplicitAny` — что ломается при включении.
- 🟡 Модули: `import type`, barrel-файлы, циклические зависимости.
- 🟡 Типизация React/Vue компонентов (props, events) — опыт.
- 🟡 `satisfies` operator — зачем (TS 4.9+).
- 🟡 Декораторы и metadata — использовал ли (Nest, class-validator)?
- 🟡 Работа с `fetch`/axios: типизация ответа API, ошибок, pagination.
- 🟡 `zod` / `io-ts` / runtime validation — зачем поверх типов.
- 🔴 Conditional types и `infer` — объясни на примере `ReturnType`.
- 🔴 Типизируй сложный API: вложенные объекты, optional fields, union по `kind`.
- 🔴 Миграция JS → TS на живом проекте: стратегия (`allowJs`, постепенная строгость).

## Хранение данных на клиенте

- 🟢 Зачем хранить данные в браузере? Примеры (настройки, черновик, корзина).
- 🟢 Cookies: размер, домен, path, срок жизни, `document.cookie` vs Set-Cookie.
- 🟢 `HttpOnly`, `Secure`, `SameSite=Lax/Strict/None` — защита и CORS.
- 🟢 First-party vs third-party cookies — почему ужесточают.
- 🟢 `localStorage` vs `sessionStorage`: объём, TTL, область видимости.
- 🟢 Синхронный API Web Storage — блокировка main thread на больших данных.
- 🟡 Когда cookies, когда localStorage — таблица trade-offs.
- 🟡 Session cookie vs JWT в localStorage — риски XSS и CSRF.
- 🟡 Refresh token: где хранить, rotation, logout на всех устройствах.
- 🟡 IndexedDB: object store, транзакции, асинхронность, лимиты.
- 🟡 Cache API (Service Worker): offline-first, stale-while-revalidate.
- 🟡 `sessionStorage` для multi-tab — изоляция вкладок.
- 🟡 Шифрование в localStorage — имеет ли смысл без защиты ключа.
- 🟡 GDPR / consent: что нельзя класть без согласия.
- 🟡 Очистка при logout: что удалять (storage, cookies, indexedDB, SW cache).
- 🟡 Private mode / Safari ITP — ограничения хранения.
- 🟡 Cross-tab sync: `storage` event, BroadcastChannel.
- 🟡 PWA: что кэшировать в SW vs IndexedDB.
- 🔴 Спроектируй auth flow для SPA: access + refresh, silent renew, 401 handling.
- 🔴 Утечка токена через XSS — меры на фронте и бэке.
- 🔴 Offline-редактор документа: стратегия sync при появлении сети.

## HTTP, сеть и API

- 🟢 Методы HTTP (GET, POST, PUT, PATCH, DELETE) — назначение.
- 🟢 Коды ответа: 2xx, 3xx, 4xx, 5xx — примеры.
- 🟡 HTTP vs HTTPS. Что даёт TLS?
- 🟡 Идемпотентность и безопасность методов.
- 🟡 TCP vs UDP: когда что используется.
- 🟡 WebSocket vs long polling / SSE — когда что выбрать.
- 🟡 REST: принципы, ресурсы, версионирование API.
- 🟡 GraphQL vs REST — плюсы и минусы (если знаком).
- 🟡 Кэширование: заголовки `Cache-Control`, `ETag`, CDN.
- 🟡 CORS: что это и как решаются типичные ошибки.
- 🟡 DNS, типы записей (A, AAAA, CNAME, MX). Что такое NS.
- 🟡 SSH: зачем, ключи, отличие от FTP.
- 🔴 Как спроектировал бы пагинацию, фильтрацию и rate limiting в публичном API?

## Безопасность

- 🟡 XSS: виды и защита на фронте и бэке.
- 🟡 CSRF: как работает и как защищаться.
- 🟡 SQL-инъекции: актуальны ли сегодня, prepared statements.
- 🟡 Хранение паролей: хеширование, соль, pepper.
- 🟡 JWT, сессии, OAuth2/OIDC — в общих чертах, где что уместно.
- 🔴 OWASP Top 10 — что из списка встречал в практике?

## Производительность

- 🟢 Почему важна производительность (UX, SEO, конверсия, cost).
- 🟢 Critical rendering path: HTML → CSS → JS → paint.
- 🟢 Reflow vs repaint vs composite — в двух словах.
- 🟢 Сжатие: gzip vs brotli на сервере/CDN.
- 🟡 Core Web Vitals: LCP, INP, CLS — что измеряют и как улучшать.
- 🟡 TTFB, FCP — от чего зависят на фронте и бэке.
- 🟡 Оптимизация изображений: WebP/AVIF, `srcset`, `sizes`, lazy load.
- 🟡 Шрифты: `font-display`, subset, preload, FOIT/FOUT.
- 🟡 Code splitting, dynamic import, prefetch/preload link.
- 🟡 Tree shaking и sideEffects — влияние на размер бандла.
- 🟡 Мемоизация в React/Vue (`memo`, `useMemo`) — когда помогает, когда нет.
- 🟡 Виртуализация длинных списков — зачем.
- 🟡 Debounce/throttle для search и scroll handlers.
- 🟡 HTTP/2 и HTTP/3 — мультиплексирование, что меняется для фронта.
- 🟡 Кэширование: browser (`Cache-Control`), CDN, application cache, Redis.
- 🟡 Cache invalidation — «вторая сложнейшая проблема».
- 🟡 Database: индексы, N+1, connection pool — связь с latency API.
- 🟡 Профилирование фронта: Performance tab, Lighthouse, Web Vitals extension.
- 🟡 Профилирование бэка: APM (Datadog, New Relic), `pprof`, slow query log.
- 🟡 Load testing: k6, Locust, JMeter — что измеряли перед релизом.
- 🟡 Rate limiting и backpressure — защита от перегрузки.
- 🟡 Cold start serverless / контейнеров — как минимизировать.
- 🔴 Страница грузится 8 секунд — план диагностики по слоям.
- 🔴 Кэш Redis + БД: согласованность при обновлении данных.
- 🔴 SLA 200ms на API при 10k RPS — архитектурные рычаги.

## Node.js

- 🟢 Что такое Node.js? Отличие от браузерного JS.
- 🟢 Для каких задач Node уместен, а для каких — нет.
- 🟢 Event-driven архитектура, неблокирующий I/O, однопоточный event loop.
- 🟢 `npm`/`yarn`/`pnpm`: scripts, зависимости, devDependencies.
- 🟢 `package.json`: `main`, `type: module`, `exports`, engines.
- 🟢 Синхронный vs асинхронный API (`readFile` vs `readFileSync`) — trade-offs.
- 🟡 V8, libuv: что под капотом в двух словах.
- 🟡 LTS vs Current — как выбирать версию для прода.
- 🟡 Callback hell → Promises → async/await. Обработка необработанных rejection.
- 🟡 `EventEmitter`: подписка, `once`, утечки слушателей.
- 🟡 `Buffer` и кодировки (UTF-8, binary).
- 🟡 Streams: readable/writable/transform/duplex, backpressure, pipe.
- 🟡 Работа с ФС: `fs.promises`, streams для больших файлов.
- 🟡 `path`, `os`, `crypto` (hash, random) — типичные кейсы.
- 🟡 CommonJS vs ESM в Node: `require`, `import`, `__dirname` в ESM.
- 🟡 `child_process`: exec, spawn — когда использовать.
- 🟡 `cluster` и Worker Threads — CPU-bound задачи.
- 🟡 HTTP-сервер на `http`/`https`: request/response, keep-alive.
- 🟡 Express: routing, middleware chain, error middleware.
- 🟡 Fastify / Koa / Nest — с чем работал, отличия по производительности и DX.
- 🟡 Валидация входа: Joi, Zod, class-validator — подход на проекте.
- 🟡 Аутентификация: JWT, sessions, passport — опыт и риски.
- 🟡 Подключение к БД: пул соединений, graceful shutdown.
- 🟡 ORM/Query builders: Prisma, TypeORM, Sequelize, Knex — плюсы/минусы.
- 🟡 WebSocket (`ws`, Socket.io) vs SSE — когда что.
- 🟡 Логирование: pino, winston, correlation id, уровни.
- 🟡 Env и конфиг: `dotenv`, 12-factor, секреты.
- 🟡 Тесты: Jest/Vitest, supertest, моки БД и HTTP.
- 🟡 ESLint + Prettier + husky/lint-staged в команде.
- 🟡 Memory leaks в Node: глобальные кэши, closures, timers — как искать.
- 🟡 `node --inspect`, clinic.js, APM — профилирование.
- 🔴 Спроектируй REST-сервис: слои, DI, единый формат ошибок, healthcheck.
- 🔴 Graceful shutdown: in-flight requests, закрытие БД и очередей.
- 🔴 Высокая нагрузка: clustering, rate limit, кэш, очередь задач (BullMQ).

## Go

- 🟢 Для каких задач Go подходит лучше всего? Где бы не выбирал Go?
- 🟢 Компилируемый язык: что получается на выходе, чем отличается от интерпретируемых runtime.
- 🟢 Базовые типы: `int`, `string`, `bool`, `byte`/`rune`. Нулевые значения.
- 🟢 Массив vs срез (`slice`): отличия, `len` и `cap`, как растёт срез при `append`.
- 🟢 `map`: особенности, можно ли итерировать во время записи, нулевой `map`.
- 🟢 `struct`: поля, теги, экспорт (заглавная/строчная буква).
- 🟢 `if`, `for`, `switch` — чем цикл в Go отличается от других языков.
- 🟢 `defer`: порядок выполнения, типичные кейсы (закрытие файлов, unlock).
- 🟡 Указатели: зачем в Go, когда передавать по значению, когда по указателю.
- 🟡 Методы: value receiver vs pointer receiver — влияние на мутацию и интерфейсы.
- 🟡 Интерфейсы: неявная реализация, пустой интерфейс `any`, type assertion и type switch.
- 🟡 Встраивание (embedding) структур и интерфейов — зачем и как работает.
- 🟡 Обработка ошибок: `error` как значение, `fmt.Errorf`, `%w`. Когда уместен `panic`/`recover`.
- 🟡 `errors.Is` и `errors.As` — зачем появились и примеры.
- 🟡 Пакеты и модули: `go mod`, `go.sum`, зачем коммитить lockfile, `internal/`, layout `cmd/`.
- 🟡 `go test`: table-driven tests, `-race`, benchmarks (`testing.B`).
- 🟡 Горутины: что это, стоимость по сравнению с OS-thread.
- 🟡 Каналы: буферизованные и небуферизованные, закрытие, чтение из закрытого канала.
- 🟡 `select`: несколько каналов, `default`, таймауты.
- 🟡 Синхронизация: `sync.Mutex`, `RWMutex`, `WaitGroup`, `sync.Once`, `atomic`.
- 🟡 Race condition: как ловить (`go test -race`), типичные ошибки в веб-сервисах.
- 🟡 `context.Context`: зачем, отмена, дедлайны, передача в HTTP и gRPC.
- 🟡 `net/http`: handler, middleware, `http.Server`, graceful shutdown.
- 🟡 Роутеры и фреймворки: stdlib vs Gin/Echo/chi — с чем работал, trade-offs.
- 🟡 `database/sql`: пул соединений, `QueryContext`, подготовленные запросы, транзакции.
- 🟡 Драйверы и ORM: `pgx`, `sqlx`, GORM — опыт, когда ORM мешает.
- 🟡 JSON: `encoding/json`, теги, `omitempty`, кастомный `MarshalJSON`/`UnmarshalJSON`.
- 🟡 Конфигурация: env, flags (`flag`), viper/аналоги — как делал на проектах.
- 🟡 Логирование: `slog`, zap, zerolog — структурированные логи, уровни, correlation id.
- 🟡 Линтеры: `go vet`, `staticcheck`, `golangci-lint` — что проверяют в CI.
- 🟡 Generics (Go 1.18+): constraints, когда упрощают код, когда усложняют.
- 🟡 gRPC / protobuf: опыт, отличие от REST, streaming.
- 🟡 Воркеры и очереди: fan-in/fan-out, worker pool, интеграция с Kafka/RabbitMQ/NATS.
- 🟡 Кэш в Go: `sync.Map` vs обычная `map` + mutex, Redis-клиенты.
- 🔴 Планировщик Go (GMP) — в общих чертах: горутина, поток ОС, очереди.
- 🔴 Escape analysis и аллокации: почему иногда важен pointer receiver и профилирование `pprof`.
- 🔴 Проектирование микросервиса: слои (handler → service → repo), DI без тяжёлого фреймворка, тестируемость.
- 🔴 Утечки горутин: как возникают (забытый `ctx`, блокировка на канале) и как диагностировать.
- 🔴 Высокая нагрузка: что оптимизировал (пул соединений, batch, ограничение горутин, профили CPU/heap).

## PHP

- 🟢 Где используется PHP сегодня (веб, CLI, workers)?
- 🟢 Типы данных, слабая/строгая типизация (`declare(strict_types=1)`).
- 🟢 Одинарные vs двойные кавычки, интерполяция.
- 🟢 Массивы: индексированные и ассоциативные, основные функции.
- 🟢 Включение файлов: `require`, `include`, `require_once`, autoload (PSR-4).
- 🟢 Суперглобалы: `$_GET`, `$_POST`, `$_SERVER`, `$_SESSION` — осторожность и безопасность.
- 🟡 ООП: классы, наследование, `final`, видимость, static.
- 🟡 Интерфейсы, абстрактные классы, трейты — отличия и примеры.
- 🟡 Пространства имён, Composer, `vendor/`, autoload.
- 🟡 Обработка ошибок: exceptions, `try/catch`, error levels, custom exceptions.
- 🟡 PSR-стандарты (PSR-1, PSR-4, PSR-7, PSR-12) — что знаешь.
- 🟡 Фреймворки: Laravel / Symfony / Yii — с чем работал, DI-контейнер.
- 🟡 Routing, middleware, контроллеры, сервис-слой.
- 🟡 Eloquent / Doctrine: ORM, N+1, eager loading, миграции.
- 🟡 Валидация и Form Request / Symfony Validator.
- 🟡 Аутентификация: sessions, Sanctum/Passport, OAuth.
- 🟡 Кэш: Redis, Memcached, tags, cache invalidation.
- 🟡 Очереди: Laravel Queue, Horizon, failed jobs.
- 🟡 Тесты: PHPUnit, Pest, моки, feature vs unit.
- 🟡 PHP-FPM: workers, `pm.max_children`, медленные запросы.
- 🟡 Nginx + PHP vs Apache — базовая схема запроса.
- 🟡 Безопасность: SQLi, XSS, CSRF, escaping, prepared statements.
- 🟡 PHP 8+: named args, match, enums, attributes, readonly, JIT — что применял.
- 🟡 Opcache, Composer 2, оптимизация autoload (`--optimize`).
- 🔴 Спроектируй модуль: repository, DTO, транзакции, идемпотентность.
- 🔴 Отладка prod: логи, slow query, Xdebug только на dev/stage.
- 🔴 Legacy PHP: как безопасно рефакторить монолит.

## Bitrix

- что такое комплексные компоненты, class.php, наследование компонентов
- как в битриксе реализовать миграции схемы БД (инфоблоки, веб-формы и тд)
- как работает технология "композитный сайт", какие знаете особенности работы с ней
- роль папки /local/ и ее структура

## Паттерны и принципы

- 🟢 Что такое паттерн проектирования? Зачем не зубрить все 23.
- 🟢 Три категории: порождающие, структурные, поведенческие — по одному примеру.
- 🟢 SOLID: каждая буква с примером нарушения в коде.
- 🟢 DRY, KISS, YAGNI — когда «сухость» вредна.
- 🟡 Порождающие: Singleton (почему часто антипаттерн), Factory, Builder, Prototype.
- 🟡 Структурные: Adapter, Facade, Decorator, Proxy, Composite.
- 🟡 Поведенческие: Strategy, Observer, Command, Iterator, State, Template Method.
- 🟡 MVC, MVP, MVVM — отличия, где встречал на практике.
- 🟡 Repository и Unit of Work — зачем поверх ORM.
- 🟡 Dependency Injection: constructor vs setter vs container.
- 🟡 Inversion of Control — что это в контексте фреймворков.
- 🟡 CQRS и Event Sourcing — когда оправданы, когда overkill.
- 🟡 Микросервисы vs монолит: критерии разбиения, bounded context.
- 🟡 Антипаттерны: God object, spaghetti code, magic numbers — из опыта.
- 🟡 GRASP: Low Coupling, High Cohesion — связь с рефакторингом.
- 🟡 Паттерны в JS/PHP/Go: как Singleton/Factory выглядят без классического ООП.
- 🟡 Чистая архитектура / hexagonal / layered — что использовали в команде.
- 🔴 Нарисуй и объясни: Observer или Strategy на доске + тестируемость.
- 🔴 Где на проекте был «лишний» паттерн и чем заменили?
- 🔴 Как применить SOLID к legacy без переписывания всего?

## Контейнеры и инфраструктура

- 🟢 Зачем контейнеры? Проблема «works on my machine».
- 🟢 Контейнер vs виртуальная машина: изоляция, ресурсы, скорость старта.
- 🟢 Образ vs контейнер. Registry (Docker Hub, GHCR).
- 🟢 Основные команды: `build`, `run`, `ps`, `logs`, `exec`, `stop`, `rm`.
- 🟡 Dockerfile: `FROM`, `COPY`, `RUN`, `CMD` vs `ENTRYPOINT`.
- 🟡 Слои образа и кэш сборки — как ускорить CI.
- 🟡 Multi-stage build — зачем (меньший образ, отделение build/runtime).
- 🟡 `.dockerignore`, размер образа, distroless/alpine — trade-offs.
- 🟡 Volumes vs bind mounts — данные и конфиги.
- 🟡 Сети Docker: bridge, host, compose network, DNS по имени сервиса.
- 🟡 Docker Compose: `depends_on`, healthcheck, profiles, override-файлы.
- 🟡 Один процесс на контейнер — почему рекомендуют.
- 🟡 Переменные окружения и secrets — что не класть в образ.
- 🟡 cgroups, namespaces, capabilities — в общих чертах.
- 🟡 Docker на Mac/Windows vs Linux — где нюансы производительности.
- 🟡 Сканирование образов (Trivy, Snyk) — был ли в пайплайне.
- 🟡 Kubernetes: Pod, Deployment, Service, Ingress — базовые сущности.
- 🟡 ConfigMap, Secret, liveness/readiness probes.
- 🟡 Helm / Kustomize — опыт шаблонизации манифестов.
- 🟡 Облако: managed K8s, RDS, object storage — что настраивал.
- 🔴 Zero-downtime deploy в K8s: rolling update, maxUnavailable.
- 🔴 Отладка: контейнер не стартует, OOMKilled, crash loop — шаги диагностики.
- 🔴 Безопасность: root в контейнере, read-only FS, non-root user.

## UNIX и инструменты

- 🟢 Какую ОС используешь для разработки? Linux, macOS, WSL?
- 🟢 Файловая система: пути, права `rwx`, `chmod`, `chown`.
- 🟢 Навигация и просмотр: `cd`, `ls`, `pwd`, `cat`, `less`, `head`, `tail`.
- 🟢 Поиск: `find`, `grep`/`rg`, `which`, `whereis`.
- 🟢 Процессы: `ps`, `top`/`htop`, `kill`, сигналы (SIGTERM, SIGKILL).
- 🟢 Перенаправление: `>`, `>>`, `|`, `2>&1`, stdin/stdout/stderr.
- 🟡 Shell-скрипты: shebang, переменные, `set -euo pipefail`.
- 🟡 `curl`/`wget` для проверки API и заголовков.
- 🟡 `ssh`, `scp`, `rsync` — доступ к серверам и деплой артефактов.
- 🟡 `tar`, `zip`, архивирование логов и бэкапов.
- 🟡 `cron` / systemd timers — периодические задачи.
- 🟡 `systemctl`: status, restart, journalctl — сервисы на Linux.
- 🟡 Сеть: `ping`, `traceroute`, `netstat`/`ss`, `lsof -i`, `dig`/`nslookup`.
- 🟡 `env`, экспорт переменных, `.bashrc` vs `.profile`.
- 🟡 `make`: targets, зависимости — использовал ли в проектах.
- 🟡 `tmux`/`screen` — долгие задачи на сервере.
- 🟡 `sudo`, least privilege, SSH keys vs пароли.
- 🟡 Настройка dev-окружения с нуля: git, docker, nvm/asdf, IDE.
- 🟡 Логи приложения на сервере: ротация, `logrotate`, централизация (ELK, Loki).
- 🟡 Диск: `df`, `du`, inode exhaustion — типичные проблемы.
- 🔴 Сервер «тормозит» — порядок диагностики (CPU, RAM, disk I/O, network).
- 🔴 Напиши однострочник: найти файлы >100MB за 7 дней, посчитать строки в логах за час.

## CI/CD и деплой

- 🟢 CI vs CD vs continuous deployment — определения.
- 🟢 Зачем автоматизировать сборку и тесты перед merge.
- 🟢 Этапы типичного пайплайна: lint → test → build → scan → deploy.
- 🟡 GitHub Actions / GitLab CI / Jenkins / TeamCity — с чем работал.
- 🟡 Структура pipeline: jobs, stages, artifacts, cache зависимостей.
- 🟡 Триггеры: push, PR, tag, schedule, manual approval.
- 🟡 Секреты в CI: variables, masked, environments (staging/prod).
- 🟡 Docker build в CI: layer cache, buildx, multi-arch.
- 🟡 Тесты в CI: параллель, flaky tests, coverage gates.
- 🟡 Quality gates: линтер, typecheck, sonar — что блокирует merge.
- 🟡 Деплой на staging vs production — кто и как апрувит.
- 🟡 Стратегии деплоя: rolling, blue-green, canary — плюсы и риски.
- 🟡 Rollback: по образу, по git tag, feature flags.
- 🟡 Infrastructure as Code: Terraform/Ansible/Pulumi — опыт.
- 🟡 Ansible: playbooks, idempotency, inventory — пример задачи.
- 🟡 Cron в K8s (CronJob) vs системный cron.
- 🟡 Миграции БД в деплое: когда запускать, backward-compatible changes.
- 🟡 Smoke / health checks после деплоя.
- 🟡 Observability после релиза: метрики, алерты, SLO.
- 🟡 DORA metrics — слышал ли, что измеряют команды.
- 🔴 Спроектируй pipeline для monorepo (frontend + backend + shared lib).
- 🔴 Как безопасно выкатить breaking change API с zero downtime?
- 🔴 CI упал только на main в пятницу — твои действия.

## Git

- 🟢 Зачем VCS? Локальный репозиторий vs remote.
- 🟢 `git init`, `clone`, `status`, `add`, `commit`, `log`, `diff`.
- 🟢 Ветки: `branch`, `checkout`/`switch`, зачем feature branches.
- 🟢 `merge` vs fast-forward — что происходит с историей.
- 🟢 `pull` = fetch + merge/rebase. `push` и upstream.
- 🟡 `stash`, `cherry-pick`, `revert` — когда применять.
- 🟡 `rebase` интерактивный: squash, reorder commits — риски на shared branches.
- 🟡 Конфликты: маркеры, `ours`/`theirs`, как не потерять чужой код.
- 🟡 `.gitignore`, tracked vs untracked, удаление из индекса.
- 🟡 `git blame`, `bisect` — поиск регрессии.
- 🟡 Tags: annotated vs lightweight, релизы по тегу.
- 🟡 Pull Request / Merge Request: описание, review checklist.
- 🟡 Code review: на что смотришь (логика, тесты, безопасность, нейминг).
- 🟡 Git flow, GitHub flow, trunk-based development.
- 🟡 Monorepo vs multirepo — опыт команды.
- 🟡 `submodule` / `subtree` — когда нужны, подводные камни.
- 🟡 Hooks: pre-commit (lint), commit-msg, pre-push.
- 🟡 Signed commits, GPG — использовали ли.
- 🟡 `reflog` — восстановление «потерянного» коммита.
- 🟡 Large files: LFS — когда нужен.
- 🔴 Переписали историю на `main` — последствия и как чинить команде.
- 🔴 Стратегия hotfix в проде при trunk-based development.
- 🔴 Как организовать релизы: semver, changelog, conventional commits.

## Алгоритмы и структуры данных

- 🟢 Что такое алгоритм? Корректность, конечность, понятность.
- 🟢 Массив: доступ по индексу, вставка/удаление — сложность.
- 🟢 Связный список: односвязный, двусвязный — когда лучше массива.
- 🟢 Стек (LIFO) и очередь (FIFO) — примеры в коде (call stack, BFS).
- 🟢 «Большое O»: O(1), O(n), O(log n), O(n²), O(n log n) — интуиция.
- 🟢 Лучший, средний, худший случай. Амортизированная сложность.
- 🟡 Рекурсия vs итерация. Переполнение стека.
- 🟡 Бинарный поиск: условие монотонности, off-by-one.
- 🟡 Сортировки: bubble/insertion (учебные), merge, quick, heap — сложность.
- 🟡 Stable sort — когда важен.
- 🟡 Hash table: hash function, коллизии, chaining vs open addressing.
- 🟡 `Map`/`Set` в JS — что под капотом ожидаешь.
- 🟡 Деревья: BST, balanced (AVL/Red-Black — названия), обход in/pre/post-order.
- 🟡 BFS и DFS: очередь vs стек, применение (кратчайший путь, компоненты).
- 🟡 Граф: представление (adjacency list/matrix), directed/weighted.
- 🟡 Topological sort — зачем (зависимости задач, build order).
- 🟡 Heap / priority queue — top-K, merge k lists.
- 🟡 Два указателя: пара в отсортированном массиве, палиндром.
- 🟡 Sliding window: максимум подмассива фиксированной длины.
- 🟡 Prefix sum — быстрые запросы суммы на отрезке.
- 🟡 Жадные алгоритмы — когда дают оптимум, контрпример.
- 🟡 Динамическое программирование: overlapping subproblems, memoization.
- 🟡 Big-O практики: почему O(n²) на 1000 элементов может быть ок, на 1M — нет.
- 🔴 Реализуй: reverse linked list, valid parentheses, merge two sorted arrays.
- 🔴 Найди дубликат / missing number — оптимизация по памяти.
- 🔴 Задача на граф: число островов, есть ли цикл — BFS/DFS на доске.
- 🔴 Как бы выбрал структуру для LRU cache (hash + doubly linked list).

## Тестирование

- 🟢 Зачем автотесты? Что они не гарантируют.
- 🟢 Unit vs integration vs e2e — определения и границы.
- 🟢 Пирамида тестирования vs ромб / трофей — современные взгляды.
- 🟢 Что такое test case: arrange, act, assert.
- 🟢 Мок vs стаб vs фейк vs spy — отличия.
- 🟡 Покрытие кода (coverage): line/branch — когда метрика вредна.
- 🟡 TDD: red-green-refactor — пробовал ли, где помогло.
- 🟡 BDD (Cucumber, Gherkin) — опыт, ценность для бизнеса.
- 🟡 Jest / Vitest: snapshots, matchers, `vi.mock`.
- 🟡 PHPUnit / Pest: data providers, mocking HTTP.
- 🟡 Testing Library: почему не тестировать implementation details.
- 🟡 E2E: Playwright vs Cypress — селекторы, CI, параллель.
- 🟡 Contract testing (Pact) — между микросервисами.
- 🟡 Фикстуры БД: in-memory SQLite, Testcontainers, транзакции с rollback.
- 🟡 Factory / faker для тестовых данных.
- 🟡 Flaky tests: причины (тайминг, порядок, сеть) и как чинить.
- 🟡 Тесты в CI: блокирующие merge, отчёт, parallel shards.
- 🟡 Regression и smoke suite перед релизом.
- 🟡 Property-based testing — слышал ли (fast-check, Hypothesis).
- 🟡 Нагрузочное тестирование vs функциональное.
- 🟡 QA в команде: кто пишет e2e, кто ревьюит тесты разработчиков.
- 🟡 Тестирование API: supertest, httptest, Postman/Newman в CI.
- 🔴 Как тестировать код с БД, Kafka, внешним payment API.
- 🔴 Legacy без тестов — с чего начать (characterization tests, seam).
- 🔴 Баланс скорости CI и уверенности: что запускать на PR vs nightly.

## СУБД и данные

- 🟢 Что такое СУБД? Реляционные vs нереляционные — критерии выбора.
- 🟢 Таблица, строка, столбец, схема, первичный ключ.
- 🟢 SQL: `SELECT`, `WHERE`, `ORDER BY`, `LIMIT`/`OFFSET`.
- 🟢 `INSERT`, `UPDATE`, `DELETE` — базовый синтаксис.
- 🟢 `INNER` / `LEFT` / `RIGHT` / `FULL` JOIN — когда какой.
- 🟢 `GROUP BY`, агрегаты (`COUNT`, `SUM`, `AVG`), `HAVING`.
- 🟢 `PRIMARY KEY`, `FOREIGN KEY`, уникальные ограничения.
- 🟢 Индексы: B-tree, зачем, когда помогают и когда мешают.
- 🟡 `UNION` vs `UNION ALL`. Подзапросы vs JOIN — читаемость и план.
- 🟡 `EXISTS` vs `IN`. Коррелированные подзапросы.
- 🟡 Оконные функции (`ROW_NUMBER`, `RANK`, `LAG`/`LEAD`) — пример.
- 🟡 `CASE`, COALESCE, работа с NULL.
- 🟡 Нормализация (1NF–3NF) и денормализация — trade-offs.
- 🟡 Транзакции, ACID. `BEGIN` / `COMMIT` / `ROLLBACK`.
- 🟡 Уровни изоляции: dirty read, phantom read — что предотвращает каждый.
- 🟡 Deadlock — как возникает и как обрабатывать в приложении.
- 🟡 Constraints: `NOT NULL`, `CHECK`, `UNIQUE`, FK ON DELETE CASCADE.
- 🟡 Prepared statements, параметризованные запросы, SQL-инъекции.
- 🟡 Миграции: версионирование схемы, backward-compatible changes.
- 🟡 MySQL vs PostgreSQL: типы, JSON, MVCC, full-text — отличия.
- 🟡 План запроса: `EXPLAIN` / `EXPLAIN ANALYZE` — на что смотреть.
- 🟡 Составной индекс, покрывающий индекс, leftmost prefix rule.
- 🟡 N+1 в ORM — как обнаружить и исправить.
- 🟡 Пагинация: offset vs keyset (cursor) — проблемы больших offset.
- 🟡 Полнотекстовый поиск в БД vs Elasticsearch — когда что.
- 🟡 Репликация: master-replica, lag, read-your-writes.
- 🟡 Шардирование: по ключу, hotspots, resharding.
- 🟡 Партиционирование таблиц — зачем (архив, производительность).
- 🟡 NoSQL: document (MongoDB), column, graph — кейсы.
- 🟡 CAP-теорема — в двух словах для собеседования.
- 🟡 MongoDB: документ, индексы, aggregation pipeline — опыт.
- 🟡 Connection pool: размер, таймауты, idle connections.
- 🟡 Бэкапы: full/incremental, point-in-time recovery, проверка restore.
- 🔴 Медленный запрос в проде — пошаговая диагностика.
- 🔴 Спроектируй схему: пользователи, заказы, платежи — FK, индексы, soft delete.
- 🔴 Миграция с MySQL на PostgreSQL / с монолитной БД на сервисы — риски.

## In-memory и кэш

- 🟢 Зачем in-memory cache перед БД?
- 🟢 Redis vs Memcached: типы данных, персистентность, кластер.
- 🟢 TTL — как выбирать время жизни ключа.
- 🟢 Ключи: naming convention, версионирование (`user:123:v2`).
- 🟡 Cache-aside (lazy loading) — типичный flow чтения/записи.
- 🟡 Read-through, write-through, write-behind — отличия.
- 🟡 Cache invalidation: по ключу, по тегу, TTL-only — trade-offs.
- 🟡 Thundering herd / cache stampede — singleflight, jitter TTL.
- 🟡 Hot key problem в Redis cluster.
- 🟡 Eviction policies: LRU, LFU, `volatile-lru`, `noeviction`.
- 🟡 Redis data structures: string, hash, list, set, sorted set — кейсы.
- 🟡 `INCR`, atomic operations, distributed lock (Redlock) — осторожность.
- 🟡 Pub/Sub в Redis vs Streams — когда что.
- 🟡 Персистентность: RDB snapshot vs AOF, потеря данных при crash.
- 🟡 Redis Sentinel и Cluster — high availability.
- 🟡 Session store в Redis — зачем и риски.
- 🟡 Rate limiter на Redis (sliding window, token bucket).
- 🟡 Мониторинг: hit rate, memory usage, slowlog.
- 🟡 Локальный in-process cache (LRU) + Redis — двухуровневый кэш.
- 🔴 Кэш и консистентность: обновили БД, кэш устарел — стратегии.
- 🔴 Redis упал — как ведёт себя приложение (fallback, circuit breaker).
- 🔴 Проектирование кэша для каталога с частыми обновлениями цен.

## Очереди и брокеры сообщений

- 🟢 Зачем асинхронная очередь вместо синхронного HTTP?
- 🟢 Producer, consumer, broker — роли.
- 🟢 At-most-once, at-least-once, exactly-once — определения.
- 🟢 Почему «exactly-once» сложно и что делают на практике.
- 🟡 RabbitMQ: exchange types (direct, topic, fanout), queue, binding.
- 🟡 Kafka: topic, partition, offset, consumer group.
- 🟡 RabbitMQ vs Kafka vs NATS — когда что выбрать.
- 🟡 Идемпотентность consumer: ключ идемпотентности, dedup table.
- 🟡 Ordering: single partition vs параллелизм.
- 🟡 Retry: exponential backoff, max attempts, DLQ.
- 🟡 Dead Letter Queue — что делать с «мёртвыми» сообщениями.
- 🟡 Poison message — как не зациклить retry.
- 🟡 Visibility timeout (SQS-аналог) — зачем.
- 🟡 Outbox pattern — согласованность БД и события.
- 🟡 Saga / choreography vs orchestration — распределённые транзакции.
- 🟡 Schema registry (Avro/Protobuf) в Kafka.
- 🟡 Backpressure: consumer не успевает — что делать.
- 🟡 Мониторинг lag, alerting на consumer group.
- 🟡 Приоритетные очереди, delayed messages.
- 🟡 Тестирование: testcontainers, embedded broker.
- 🔴 Спроектируй: оплата → списание → email → аналитика (события и откаты).
- 🔴 Дубликат сообщения при at-least-once — как обработать в коде.
- 🔴 Kafka rebalance storm — слышал ли, как минимизировать.

## Домены и почта

- 🟢 Что такое доменное имя? Регистратор vs DNS-хостинг.
- 🟢 DNS-резолвинг: рекурсивный resolver, TTL, кэш.
- 🟢 Запись A / AAAA — на что указывает.
- 🟢 CNAME vs ALIAS/ANAME — ограничения CNAME на apex.
- 🟢 NS-записи — делегирование зоны.
- 🟡 TXT-записи: верификация, SPF, DKIM, DMARC.
- 🟡 MX-запись и приоритет — маршрутизация почты.
- 🟡 SPF: что разрешает отправку, типичные ошибки `-all`.
- 🟡 DKIM: подпись писем, селектор, ротация ключей.
- 🟡 DMARC: политика при fail SPF/DKIM, отчёты.
- 🟡 Reverse DNS (PTR) — зачем для почтовых серверов.
- 🟡 Subdomain: `api.`, `staging.`, wildcard `*.`
- 🟡 SSL-сертификат: Let's Encrypt, HTTP-01 vs DNS-01 challenge.
- 🟡 Перенос домена: смена NS, propagation, downtime.
- 🟡 Почтовый сервер: Postfix, Exim, облачные (SendGrid, SES, Mailgun).
- 🟡 SMTP порты: 25, 465, 587 — отличия.
- 🟡 IMAP vs POP3 — хранение на сервере.
- 🟡 SPF + forwarding — почему ломается и что делать.
- 🟡 Блоклисты (Spamhaus), reputation IP — диагностика «письма в спам».
- 🟡 Настройка `noreply@` и bounce handling.
- 🔴 Письма с домена уходят в spam — чеклист проверки.
- 🔴 Поднять почту на своём VPS vs transactional API — trade-offs.
- 🔴 DNS propagation: сайт не открывается после смены A-записи — шаги.

---

## Как пользоваться списком

1. **Перед интервью** — выбери несколько разделов по стеку вакансии + 1 блок про опыт/soft skills.
2. **На интервью** — начинай с 🟢, углубляйся до 🟡/🔴 по ответам; не задавай все вопросы подряд.
3. **После** — дополняй список вопросами, которые реально помогли отличить сильного кандидата от слабого.

Список открыт для правок: удаляйте неактуальное для вашего стека, добавляйте вопросы по вашим проектам и внутренним сервисам.
