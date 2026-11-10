# Shopify / SEO-GEO / AI-шопінг / AI-інструменти для контенту — 09.09–10.11.2026 (фокус 20.10–10.11)

> Методологія і обмеження цього запуску (читати першим):
> - Пряме відкриття сторінок у цій сесії НЕ працювало: changelog.shopify.com, www.shopify.com, shopify.dev, anatta.io, shopifreaks.com, fudge.ai — `ENOTFOUND` (хости поза дозволеною мережею сесії). Тому **усе нижче — `[через пошук]`**: зміст отримано з вебпошуку (резюме сторінок), першоджерело напряму НЕ відкрите. Жодного факту не позначено 3/3, бо незалежність джерел не перевірено по повних текстах.
> - Рівні: `2/3` = два незалежні джерела (зокрема офіційна сторінка + незалежне медіа) збігаються в пошукових резюме; `1/3` = одне джерело або лише вендорні/агенційні блоги (за правилами брифу вони — підказка, не підтвердження).
> - Щоб підняти рівні до 3/3, треба дозволити в мережі сесії: changelog.shopify.com, www.shopify.com, shopify.dev, help.shopify.com.

## 1. Shopify Changelog жовтень–листопад 2026: що корисно малому мерчанту

### Takeaway
У жовтні в changelog — кілька практичних речей для малих брендів (планування й A/B знижок на Basic+, передача compare-at price AI-агентам, market-driven shipping для всіх, Canvas для дизайну з Sidekick). Пряме відкриття changelog не вдалося, тож усе 1/3–2/3 і потребує звірки в адмінці.

### Cited Findings
- **Discount scheduling + A/B testing знижок для планів Basic і вище, 02.10.2026** [ОФ][через пошук] 1/3 (лише агентський трекер Common Thread). Навіщо вам: перед BFCM запустити дві версії знижки (напр. −15% vs безкоштовна доставка від $X) і подивитись, яка дає більше маржі. Шлях (очікуваний, перевірити): Admin → Discounts → Create discount → розклад/тест. — [Common Thread Co, Every Shopify Update in 2026](https://commonthreadco.com/blogs/coachs-corner/every-shopify-update-in-2026-updated-weekly)
- **Compare-at price передається AI-агентам через Shopify Catalog, 09.10.2026** [ОФ][через пошук] 2/3 (Shopify Fall '26 merchant page у пошуковому резюме + незалежний блог). Навіщо: ваші знижки (закреслена ціна) тепер видно в ChatGPT/Gemini/Copilot-видачі без налаштувань — але лише якщо поле compare-at заповнене чесно (FTC-ризик у США за фейкові «було/стало»). — [Shopify News, Fall '26 merchant](https://www.shopify.com/news/fall-26-edition-merchant); [Kevion Technologies](https://keviontechnologies.in/blog/shopify-updates-october-2026-what-to-do)
- **Market-driven shipping відкрито всім мерчантам з 01.10.2026** [ОФ][через пошук] 1/3 (агентський блог). Навіщо: окремі тарифи доставки для США / ЄС / UK у межах Markets — критично для українських відправників, де ціна доставки в UK і US різна. — [Kevion Technologies](https://keviontechnologies.in/blog/shopify-updates-october-2026-what-to-do)
- **Canvas — дизайн «повністю кастомного» магазину разом із Sidekick, 01.10.2026** [ОФ][через пошук] 1/3 (пошукове резюме changelog). Навіщо: переробити головну/лендінг під BFCM без розробника. — [Shopify Changelog](https://changelog.shopify.com/)
- **Guaranteed flat-rate shipping тепер із Managed Markets, 23.10.2026** [ОФ][через пошук] 1/3. ⚠️ Managed Markets (Global-e) доступний лише мерчантам із підтримуваних країн реєстрації — для ФОП з України, ймовірно, нерелевантно; перевірити. — [Shopify Changelog](https://changelog.shopify.com/)
- **Translate & Adapt auto-sync до 8 мов (EU та US/Canada мерчанти)** [ОФ][через пошук] 1/3, дата не встановлена. Навіщо: автопереклад сторінок для ЄС-маркетів. — [Shopify Changelog](https://changelog.shopify.com/)
- **Автоматичний податок на return shipping fees у США з 23.10.2026** [ОФ][через пошук] 1/3. Навіщо: якщо ви берете плату за повернення з американців — перевірте налаштування tax, щоб не «з'їсти» податок із маржі. — [Kevion Technologies](https://keviontechnologies.in/blog/shopify-updates-october-2026-what-to-do)
- Нерелевантно для аудиторії (для повноти): POS 11.17 (13.10), POS-ідентифікація клієнтів (28.10), виплати постачальникам з Shopify Balance — лише US-мерчанти (06.10). — [Shopify Changelog](https://changelog.shopify.com/); [Consensus](https://consensus.pt/shopify/news/shopify-updates-october-2026/)
- Агрегатор Spyingbee налічує «60 product updates in October 2026» — [ІНЖ] 1/3, не для екрана. — [Spyingbee](https://spyingbee.com/updates/shopify/2026-10)

### Inferences
- Для «зроби цього тижня» найсильніше: (1) A/B знижки перед BFCM (якщо підтвердиться доступність на Basic); (2) перевірити compare-at price на ключових товарах, бо вони тепер ідуть в AI-видачу; (3) розвести тарифи доставки по Markets.
- Не вдалося знайти в цьому вікні підтверджених changelog-записів про Shopify Messaging/email, B2B чи subscriptions — не означає, що їх немає (changelog не відкрився).

### Gaps
- Повний список changelog-записів 20.10–10.11 — недоступний (хост заблоковано). Потрібна ручна перевірка або дозвіл мережі.
- Точні шляхи в Admin для discount A/B — не підтверджені офіційною help-сторінкою.
- Агентний / AI-канал в Analytics: є лише вендорні описи дашборду Agentic Storefronts (Sales/Orders/Sessions по AI-платформах, з березня 2026) — [Easysell](https://easysellapp.com/blogs/wiki/shopify-agentic-storefronts-analytics-ai-sales-dashboard-2026). 1/3, [ІНЖ], поза вікном як новина; у вікні нового звіту не знайдено.

## 2. Shopify Fall '26 Edition (28.10.2026): що з цього малим мерчантам, GA vs early access, дедлайни

### Takeaway
Edition «Exponential» побудована довкола агентної комерції: сторінка Sales channels → Agentic (база знань для агентів), продаж у Google AI Mode / Gemini з checkout Shopify, Shop Pay в агентах, керування магазином з ChatGPT/Copilot/Gemini/Perplexity, оновлений Sidekick. Жорсткий дедлайн підтверджено: script tags перестають працювати на вітрині 01.03.2027.

### Cited Findings
- **Назва й дата:** Fall '26 Edition «Exponential», 28.10.2026, «150+ оновлень» [ОФ][через пошук] 2/3 (офіційна сторінка Shopify у видачі + незалежні огляди; цифру «150+» — лише блог, 1/3). — [Shopify News](https://www.shopify.com/news/fall-26-edition-merchant); [Witscode](https://witscode.com/blogs/shopify-editions-fall-2026); [Ordoro, 06.11.2026](https://blog.ordoro.com/2026/11/06/shopify-editions-fall-2026/)
- **Sales channels → Agentic (knowledge base для AI-агентів)** [ОФ][через пошук] 2/3. Мерчант переглядає й публікує факти, які отримують агенти: вікно повернень, країни доставки, подарункові послуги тощо; агенти отримують лише опубліковані факти. Сторінка також показує, чи магазин придатний для Shopify Catalog, і що виправити. — [Shopify News](https://www.shopify.com/news/fall-26-edition-merchant); [Fudge.ai](https://www.fudge.ai/blog/shopify-fall-2026-edition/); [Coalition Technologies](https://coalitiontechnologies.com/blog/shopify-editions-fall-26)
  - ⚠️ Нюанс (1/3, блог): чернетки фактів зі сторінок вітрини НЕ публікуються автоматично, але факти політик і контактів з адмінки публікуються одразу — їх треба перевірити. — [Fudge.ai](https://www.fudge.ai/blog/shopify-fall-2026-edition/)
  - Стара окрема апка Knowledge Base закривається **15.01.2027** [через пошук] 1/3. — те саме джерело.
  - 🔧 Дата появи: один блог — 26.10, інші — 28.10 (дата Edition).
- **Продаж у Google Search (у т.ч. AI Mode) і в Gemini app з checkout на Shopify, замовлення — у звичайній адмінці** [ОФ][через пошук] 2/3. — [Shopify News](https://www.shopify.com/news/fall-26-edition-merchant); [CFOtech](https://cfotech.com.au/story/shopify-unveils-ai-shopping-tools-in-fall-26-update)
- **Shop Pay усередині агентів Muse (Meta), Claude Duet, Grok Bot, Instinct** [ОФ][через пошук] 2/3 (сторінка Edition + транскрипт Q3-дзвінка). — [Shopify News](https://www.shopify.com/news/fall-26-edition-merchant); [Webull, Q3 2026 transcript](https://www.webull.com/news/15860362194492416)
- **shop.md / «shop skill»** — покупець може «направити» ChatGPT, Claude чи інший агент на shop.md і шукати серед 1+ млрд товарів, платити Shop Pay, трекати замовлення [ОФ][через пошук] 1/3 (резюме офіційної сторінки; цифру «1+ млрд» не верифіковано). — [Shopify News](https://www.shopify.com/news/fall-26-edition-feature)
- **Керування замовленнями/запасами з ChatGPT, Copilot, Gemini, Perplexity через Shopify connectors; Sidekick перебудовано (пише код, шукає в інтернеті), Canvas — редизайн магазину** [ОФ][через пошук] 1/3–2/3. — [Shopify News](https://www.shopify.com/news/fall-26-edition-merchant); [Meetanshi](https://meetanshi.com/blog/shopify-fall-edition-2026/)
- **GA vs early access:** 🔧 джерела розходяться. Один огляд: checkout-інструменти для агентів запрацювали ще 28.09, за місяць до Edition. Інший: багато фіч — early access / поступове розгортання, зокрема checkout custom fields НЕ встигнуть до BFCM 2026. [ІНЖ] 1/3 кожне. — [Anatta](https://anatta.io/blog/shopify-editions-fall-2026/) (не відкрилось, переказ з пошуку) [переказ]; [Sezerium](https://sezerium.com/blog/shopify-editions-fall-26-what-merchants-and-app-builders-need-to-know/)
- **WebMCP** — у пошукових резюме цього запуску конкретики не знайдено. Не вигадувати.
- **ДЕДЛАЙН script tags** [ОФ][через пошук] 2/3 (shopify.dev changelog + Shopify community dev forum, обидва Shopify, але різні канали; + сторонні блоги):
  - 26.08.2026 — script tags на Order status page перестали працювати (вже минуло).
  - 01.10.2026 — апки більше не можуть створювати/оновлювати script tags; існуючі ще працюють.
  - **01.03.2027 — storefront script tags перестають виконуватися.** Стосується всіх версій API; заміна — app embed block / theme app extension / web pixels. Пост changelog датовано 24.08.2026.
  - Мерчанти, що ставлять уражені апки, бачать банер-попередження про 01.03.
  — [shopify.dev changelog](https://shopify.dev/changelog/online-store-script-tags-deprecation); [community.shopify.dev](https://community.shopify.dev/t/deprecation-script-tags-will-stop-running-on-march-1-2027/37108); [Shopify dev docs](https://shopify.dev/docs/apps/build/online-store/script-tag-deprecation)
  - ⚠️ Чутка з блогів: офлайн-токени без терміну дії → HTTP 403 з 01.04.2027 — в офіційних джерелах НЕ знайдено, 1/3, не озвучувати.

### Inferences
- «Зроби цього тижня»: (1) Admin → Sales channels → Agentic: перечитати кожен опублікований факт (повернення, доставка в US/UK/EU, терміни з України — щоб агент не пообіцяв «доставку за 3 дні»); виправити блокери Catalog-eligibility. (2) Пройтись по апках: якщо будь-яка показує банер про 01.03.2027 (відгуки, чати, пікселі, upsell) — написати розробнику або шукати заміну на app embed; перевірити Online Store → Themes → Customize → App embeds. (3) Заповнити compare-at чесно.
- Для українських ФОП продаж через Google AI Mode / Gemini, ймовірно, обмежений тим самим, що й Google-checkout (US-фокус) — потребує перевірки.

### Gaps
- Офіційний список «GA / early access» по кожній фічі не отримано (www.shopify.com і shopify.dev не відкрились).
- WebMCP — даних немає.
- Чи доступний Google AI Mode checkout через Shopify для магазинів, зареєстрованих поза США — невідомо.

## 3. Shopify Q3 2026 call — практичні сигнали (лише як сигнали)

### Takeaway
Крім відомих хедлайнів, на дзвінку прозвучали якісні сигнали: «AI вже не лише канал discovery», Shop Pay як гаманець в агентах навіть для не-Shopify мерчантів. Цифри international GMV / Shop Pay за Q3 2026 надійно не підтверджені.

### Cited Findings
- Фінкельштейн: AI «більше не просто канал discovery»; агенти Muse, Instinct, Claude Duet, Grokbot партнеряться з Shopify, щоб checkout мерчантів працював, а покупці платили Shop Pay [ОФ-транскрипт][через пошук] 1/3 (один транскрипт-агрегатор). — [Webull transcript](https://www.webull.com/news/15860362194492416); також [EarningsWhispers](https://www.earningswhispers.com/transcript/SHOP/Q32026) (не відкрито)
- 🔧 «International GMV +41%», «Shop Pay GMV $29 млрд, +67%» — у джерелах змішано Q3 2025 і Q3 2026 (Hudson Labs — передзвіткові оцінки). НЕ використовувати. — [Hudson Labs](https://www.hudson-labs.com/research/shopify-q3-2026-earnings-preview-shop-results-preview)
- Контекст Q2 2026: international GMV +37%, B2B GMV +76% [через пошук] 1/3. — [Eastern Progress](https://www.easternprogress.com/shopify-q2-earnings-call-spotlights-ai-commerce-and-growth/article_7b9e0495-102c-5521-bcae-1297105599a4.html)

### Inferences
- Сигнал для аудиторії: Shopify вкладається в те, щоб покупець з агента платив Shop Pay — увімкнений Shop Pay стає «квитком» в агентні канали.

### Gaps
- Shareholder letter Q3 2026 не відкрито (shopify.com заблоковано, sec.gov блокує ботів).

## 4. Google Search: апдейти, AI Mode shopping/checkout, Merchant Center, Search Console

### Takeaway
У вікні — September 2026 spam update (анонс 24.09, завершення 08.10 за одним джерелом); core update у вересні–листопаді НЕ підтверджено. Merchant Center: промо-бейджі в AI Mode (≈12.10), Loyalty Customer Match в AI Mode/Gemini (≈02.10, US), фазовий запуск UCP-хабу для checkout в AI Mode/Gemini (≈06–09.10, US, early access).

### Cited Findings
- **Spam update вересень 2026:** анонс 24.09, завершення 08.10 [ОФ-подія][через пошук] 1/3 (Medium-допис; дашборд напряму не відкрито). 🔧 SER у жовтневому огляді писав, що ще розгортається; SER-відео 09.10 — «Spam Update Done». Ціль — масовий programmatic контент і parasite SEO (Similarweb). Статус оцінюю 2/3 щодо факту апдейту, 1/3 щодо дат. — [Medium](https://medium.com/@sohaibsaeed/google-october-2026-spam-update-d12c96f4be6e); [SER October report](https://www.seroundtable.com/october-2026-google-webmaster-report-42185.html); [SER video 09.10](https://www.seroundtable.com/video-10-09-2026-42263.html); [Similarweb](https://www.similarweb.com/blog/insights/ai-news/ai-search-news-update/)
- **Жовтневого core update немає:** станом на 19.10 дашборд показував останнім September spam update; форумні «шторми» — без підтвердження [через пошук] 1/3. Останній підтверджений core — May 2026 (21.05–02.06), поза вікном. — [Search Engine Watch](https://searchenginewatch.com/google-october-2026-update-rumors/); [Search Engine Land](https://searchengineland.com/google-may-2026-core-update-rollout-is-now-complete-479119)
- **Search Console — звіт Generative AI performance:** рахує покази посилань у AI Overviews і AI Mode, БЕЗ кліків/CTR; кліки йдуть у класичний Performance. Листопадовий огляд: Google дав зрозуміти, що кліків там не буде [ІНЖ][через пошук] 1/3. — [eSEOspace, 13.10](https://eseospace.com/blog/search-console-generative-ai-performance-report/); [Numinix](https://www.numinix.com/blog/november-2026-seo-algorithm-news-update/)
- **Промо-бейджі в AI Mode (Shopping ads), ≈12.10.2026:** активні схвалені Merchant Center promotions показуються автоматично, окрема кампанія не потрібна [через пошук] 1/3 (два агентські блоги, не незалежні медіа). — [Ecommerce Fastlane](https://ecommercefastlane.com/google-ai-mode-promotions-bfcm-2026/); [Common Thread Co](https://commonthreadco.com/blogs/coachs-corner/google-ai-mode-is-now-displaying-promotional-offers-in-shopping-ads-what-ecommerce-brands-must-set-up-before-bfcm)
- **Loyalty Customer Match → AI Mode і Gemini, ≈02.10.2026;** допуск і не-рекламодавців; AI Mode/Gemini — лише US [через пошук] 2/3 (SER — незалежне медіа + агентство). — [Search Engine Roundtable](https://www.seroundtable.com/google-loyalty-customer-match-expands-42216.html); [Common Thread Co](https://commonthreadco.com/blogs/coachs-corner/google-loyalty-customer-match-is-now-in-ai-mode-what-ecommerce-brands-must-do-before-q4)
- **UCP-хаб у Merchant Center (checkout у AI Mode/Gemini), ≈06–09.10.2026:** фазовий US-запуск; треба збудувати інтеграцію, подати interest form, чекати відбору → sandbox [через пошук] 2/3. — [Shopifreaks](https://www.shopifreaks.com/google-rolls-out-a-merchant-center-hub-that-lets-us-merchants-add-checkout-to-product-listings-in-ai-mode-and-gemini-through-ucp/) (не відкрилось, [переказ]); [BigCommerce](https://www.bigcommerce.com/articles/ecommerce/google-agentic-checkout/)

### Inferences
- «Зроби цього тижня»: створити в Merchant Center → Marketing → Promotions промо на BFCM (найдешевший спосіб отримати бейдж в AI Mode); у Search Console подивитись Generative AI-звіт — які сторінки потрапляють в AI Overviews. Shopify-мерчантам UCP-хаб руками будувати не треба — Shopify дає Google-канал через Edition (п.2).

### Gaps
- Google Search Status Dashboard напряму не відкрито — дати spam update не 3/3.
- Офіційних постів Google (blog.google, support.google.com/merchants) у видачі не знайдено — усе з медіа/агенцій.
- Зміни вимог до product data / free listings у вікні — не знайдено.

## 5. ChatGPT / Perplexity / Gemini / Copilot shopping для мерчантів

### Takeaway
Instant Checkout у ChatGPT з комісією ~4% для Shopify-мерчантів фактично згорнуто 24.03.2026 (поза вікном): покупка завершується на checkout самого магазину. Але довідка OpenAI (оновл. 19.10.2026) досі згадує, що ChatGPT «може показувати Instant Checkout» для частини товарів — тобто статус «згорнуто для всіх» не 100%.

### Cited Findings
- 24.03.2026 OpenAI відійшла від Instant Checkout, фокус — discovery; покупки Shopify-мерчантів — на їхньому сайті (in-app browser у мобільному ChatGPT або нова вкладка) [ОФ][через пошук] 2/3 (OpenAI-пост + CNBC). Контекст, поза вікном. — [OpenAI, Powering Product Discovery](https://openai.com/index/powering-product-discovery-in-chatgpt/); [CNBC, 20.03.2026](https://www.cnbc.com/2026/03/20/open-ai-agentic-shopping-etsy-shopify-walmart-amazon.html)
- Shopify/Etsy-мерчантам не потрібно подаватися — дані вже інтегровано; інші — product feed напряму в OpenAI [ОФ][через пошук] 1/3–2/3. — [OpenAI](https://openai.com/index/powering-product-discovery-in-chatgpt/); [Ezyconn, перевірено 20.10.2026](https://ezyconn.com/blog/chatgpt-shopping-for-online-stores)
- 🔧 Довідка OpenAI, оновлена 19.10.2026, досі: ChatGPT «may also show an Instant Checkout option» для деяких eligible товарів [через пошук] 1/3 (сам help-центр не відкрито). — переказ із пошукового резюме, джерело-агрегатор [Growthcentr](https://www.growthcentr.com/how-to-sell-on-chatgpt-in-2026/) [переказ]
- Стара комісія 4% для Shopify (PYMNTS, початок 2026) — після березня для Shopify-мерчантів, імовірно, не діє: Shopify help (за блогами) — у адмінці немає налаштування ChatGPT direct checkout, оплата через ваш checkout, додаткової комісії понад процесинг немає [через пошук] 1/3. — [PYMNTS](https://www.pymnts.com/commerce/ecommerce/2026/shopify-merchants-to-pay-4percent-fee-on-sales-made-through-chatgpt-checkout/); [Hypotenuse](https://www.hypotenuse.ai/blog/chatgpts-instant-checkout-the-next-phase-of-agentic-commerce)
- Етсі: актуальних (2026) даних про статус/комісію Etsy в ChatGPT — не знайдено.
- Причина згортання: за словами президента Shopify, інтегрувались лише ~12 мерчантів [через пошук] 1/3, не на екран. — [Growthcentr](https://www.growthcentr.com/how-to-sell-on-chatgpt-in-2026/)
- Perplexity / Copilot / Gemini: у вікні окремих нових merchant-анонсів не знайдено, окрім Shopify Edition (Gemini/AI Mode checkout, connectors до Copilot/Perplexity — п.2).

### Inferences
- Для Shopify-мерчанта практично: ChatGPT = канал discovery, що веде на ваш checkout → важливі якість фіда (назви, атрибути, ціни, наявність) і швидкий мобільний checkout, а не «комісія 4%».

### Gaps
- Нових OpenAI-анонсів для мерчантів, датованих 09.09–10.11.2026, не знайдено.
- Статус Etsy в ChatGPT у 2026 — не встановлено.

## 6. Нові AI-інструменти для фото/відео/лістингів у вікні + правило Etsy про необроблене фото

### Takeaway
Конкретних релізів Canva / Firefly / Nano Banana / Veo / Kling для продуктових фото, датованих вікном, у пошуку не підтверджено. Головна новина в цьому кластері — правило Etsy від 22.10.2026: щонайменше одне фото реального товару на реальному фоні, без жодного редагування; решту фото можна редагувати, зокрема AI.

### Cited Findings
- **Etsy, 22.10.2026:** кожен лістинг фізичного товару — щонайменше одне фото реального виробу на реальному фоні, не змінене жодним чином; інші фото можна редагувати (світло, колір, кроп, фон), у т.ч. AI; заборонено AI-згенеровані функціональні гайди (патерни, рецепти, інструкції) і повністю бот-згенеровані лістинги; у формі лістингу з'явився прапорець-підказка для зображень, які Etsy вважає AI [ОФ-подія][через пошук] 2/3 (TechRadar + ppc.land + Retail Dive — незалежні медіа). — [TechRadar](https://techradar.com/ai-platforms-assistants/every-listing-must-include-at-least-one-photo-of-the-actual-item-etsy-is-finally-cracking-down-on-ai-images-and-text-in-listings-and-apparently-this-is-just-the-start); [PPC Land](https://ppc.land/etsy-forces-sellers-to-show-one-unaltered-photo-in-every-listing/); [Retail Dive](https://retaildive.com/news/etsy-updates-ai-use-policies-emphasize-craftsmanship/833838); [Value Added Resource](https://www.valueaddedresource.net/etsy-bans-ai-patterns/)
  - 🔧 Позиція фото: одні — не обов'язково перше; інші — Etsy хоче, щоб воно було першим. Не стверджувати на екрані.
  - 🔧 Розкриття AI: суперечливо (одні — розкривати AI-редагування лише як best practice; інші — політика покриває і AI-modified зображення). Перевірити Seller Handbook / House Rules.
- Shopify Magic / Sidekick: у Fall '26 — Sidekick перебудовано (код, вебпошук), Canvas для дизайну (п.2). Окремих нових фіч для продуктових фото — не підтверджено.
- Nano Banana / Firefly / Canva: знайдено лише недатовані вендорні туторіали (композиція продукт+фон+модель, background removal у Canva Pro); жоден не прив'язаний до релізу у вікні [ІНЖ] 1/3, не новина. — [Fibre2Fashion](https://emerge.fibre2fashion.com/blogs/10818/how-to-use-nano-banana-for-shopify-hero-banners-collection-tiles-and-pdp-images); [NewsBytes](https://www.newsbytesapp.com/news/science/googles-new-ai-tool-can-give-your-product-photos-a-makeover/tldr)

### Inferences
- Практичний воркфлоу для Etsy+Shopify після 22.10: знімати 1 «сирий» кадр на реальному фоні (телефон, денне світло) → він обов'язково в Etsy-лістингу; AI-генерацію лайфстайлу/фону лишити для решти слотів і для Shopify (там такого правила немає). «Зроби цього тижня»: пройтися по топ-20 лістингах Etsy і перевірити, чи є серед фото хоч одне без обробки.

### Gaps
- Релізи Canva / Adobe Firefly / Google Veo / Nano Banana / Kling у вікні — не знайдено надійних джерел; потрібен прицільний пошук у їхніх newsroom (blog.google, news.adobe.com, canva.com/newsroom).
- Точний текст правила Etsy з Seller Handbook — не відкрито (etsy.com заблоковано за CLAUDE.md).
