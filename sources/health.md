# Здоров'я джерел

Формат: дата · id · доступ (відкрилось / заблоковано / логін / пейвол / через пошук) · тез у дайджесті · що пройшло гейт · примітка.
Тут — лише доступ, шум і першість. Лічильник «дійшло до фіналу» — тільки в `sources/registry.md` (CLAUDE.md, 8Г). Записи 10.11 нижче — історія; актуальний стан — найновіший запис.

## 10.11.2026 — тест доступу (Етап 1) + дайджест #1
Мережа хмарної сесії: прямий HTTP і WebFetch заблоковані для всіх зовнішніх сайтів (DNS не резолвиться / проксі 403). Працює лише WebSearch.

| id | Доступ | Тез дав | Пройшло гейт |
|---|---|---|---|
| C07 Telegram @EtsyBiznes / @EtsyBizChat | заблоковано (t.me) | 0 | — |
| C01 Reddit | заблоковано | 0 | — |
| E04 SEC EDGAR | через пошук | 4 (Etsy, Shopify, Amazon, eBay, Payoneer) | 4 |
| E05 Etsy Community | через пошук | 2 | 2 (⚠️ 1/3) |
| EA02 Value Added Resource | через пошук | 4 | 4 (2 першим) |
| EA01 EcommerceBytes | заблоковано напряму; у пошуку — лише старі статті | 0 | — |
| M02 Digital Commerce 360 | через пошук | 1 | 1 |
| R01/R02 CBP, Federal Register | через пошук | 1 | 1 |
| R14 BDO (юрфірми) | через пошук | 1 | 1 |
| R11 Avalara | через пошук | 1 | 1 |
| S02/S03 Shopify Editions/News | лише вендорні перекази | 1 | 1 (✅✅ 2/3) |
| U01 Укрпошта | через пошук (медіа-перекази) | 0 нових | — |
| M07 PYMNTS | через пошук | 1 | 1 |
| G01 Google Search Central | через пошук | 0 (core update не було) | — |
| A03 Meta | вторинні блоги | 1 | ⚠️ 1/3 |

Першими повідомили (кандидати в P1-підсилення): Value Added Resource (Etsy cyber-message, EU €2 для Etsy), PPC Land (Etsy фото-правило, Shopify AI ×3,3 — **немає в реєстрі → кандидат**).

## 10.11.2026 (пізніше) — після ввімкнення Full network access
Відкривається напряму: community.etsy.com, valueaddedresource.net, changelog.shopify.com, shopify.com/news, marketplacepulse.com, modernretail.co, molodybiz.com/blog, youtube.com (список відео), Reddit через RSS (www.reddit.com/r/<sub>/new/.rss).
Блокують ботів (403): etsy.com (Seller Handbook), sec.gov, cbp.gov, ukrposhta.ua, reddit JSON / old.reddit (логін) → фолбек: WebSearch + VAR/EcommerceBytes [переказ].
Telegram @EtsyBiznes (6 622 учасники) і @EtsyBizChat (7 345) — це групи-чати, публічного веб-перегляду історії немає → потрібен експорт (див. manual_review.md).
YouTube-субтитри через yt-dlp — «Sign in to confirm you're not a bot» → субтитри дає Славік (YouTube Studio) у Drive.

## 11.11.2026 — перевірка доступів на старті циклу #14 (curl з браузерним User-Agent)
Відкриваються напряму (200): E05 Etsy Community Announcements, C02 Etsy Community, E09 Etsy Trend Edit, EA01 EcommerceBytes, EA02 Value Added Resource, EA03 CindyLouWho2, EA04 Marketplace Pulse, EA05 Marmalead, EA06 eRank, EA07 Alura, EA08 EverBee, EA09 Koalanda (головна), EA11 Growing Your Craft, EA13 Tamebay, S01 Shopify Changelog, S03 Shopify News, S04 Shopify Dev Changelog, S05 Help Center, S06 Shopify Blog, S07 Shopify Engineering, SA01 Shopifreaks, M01 Modern Retail, M02 Digital Commerce 360, M03 Retail Dive, M04 Supply Chain Dive, M05 Practical Ecommerce, M07 PYMNTS, M08 TechCrunch, M13 Digiday, N01 PPC Land, N04 Adweek, R02 Federal Register, R03 White House, R07 EC Taxation & Customs, R09 gov.uk, R11 Avalara, R12 Zonos, U03 Meest, U05 Western Bid, U07 Payoneer newsroom, U10 Верховна Рада, U12 buh.ua, U13 Дія.Бізнес, U15 Forbes.ua, U16 Інтерфакс-Україна, T01 Pantone, T04 Pinterest Business, T09 Google Trends RSS (лише загальні теми дня), A01 Google Ads & Commerce Blog, A02 Merchant Center Help, A12 Baymard, G01 Google Search Central, G03 Search Engine Journal, G04 Ahrefs, AI02 Anthropic, AI01 OpenAI (лише RSS).
Блокують (403/401): E01 etsy.com, V02 Etsy API без ключа (очікувано), AI01 openai.com (сторінка), K01 Amazon IR, K02 eBay IR, G02 Search Engine Land (і feed), M09 CNBC (і RSS), M10 Reuters (401), M15 eMarketer, R05 CPSC, R08 Council of the EU, R10 Royal Mail, T05 Faire, T08 Trend Hunter, U01 Укрпошта, AP News, OECD → через пошук [переказ].
Не відповіли / дивне: T11 Adobe DEI (таймаут двічі), R06 ftc.gov (404 на головній), Koalanda статистика (таймаут).
C01 Reddit RSS: 200 з паузою 3–5 с, 429 при частих запитах; пошук через RSS — forbidden.
Drive «Молоді Новини — бот»: папки Telegram і Субтитри порожні.
