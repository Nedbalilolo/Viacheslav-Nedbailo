# Реєстр джерел v1.0 (нормалізований)

Основа: «Реєстр джерел для щотижневого моніторингу» v1.0 від 10.11.2026. Формат рядка (оновлено 11.11.2026, правило 14):
`id · назва · URL · кластер · клас · пріоритет · статус · доступ · у фіналі: N`
Статус: активне / на випробуванні / недоступне / прибране.
Доступ: curl напряму · RSS · через пошук (сайт недоступний напряму або блокує ботів) · не перевірено · недоступне (причина).
У фіналі: скільки новин із джерела дійшло до фінального сценарію; оновлюється після кожного випуску. Зміни статусу — лише після «так» Славіка.


## ВЕРТИКАЛІ — СТАН ПОКРИТТЯ (CLAUDE.md, розділ 5б; 11 вертикалей; станом на 12.11.2026)
Основа — перевірка живими запитами 12.11.2026: `research_notes/2026-11-12_sources_check.md`.
1. Макро-рамка (США, UK, ЄС + топ-3 ЄС, Австралія, НЗ) — **ЧАСТКОВО.** США, UK, ЄС — офіційне першоджерело працює (P01–P03). Топ-3 ЄС — через Eurostat. Австралія й НЗ — лише карткові витрати, частки онлайну немає (P04, P05).
2. Глобальні події — **ЧАСТКОВО.** Federal Register API/RSS (P06), юрфірми (P07, P08), українські медіа (P09, P10); CBP і Укрпошта — лише через пошук.
3. Поведінка покупців — **ЧАСТКОВО.** McKinsey RSS (P11) + консалтинг (P12); глибокі трендові бази — платні.
4. Маркетинг і технології — **ЗАКРИТО.** RSS Google Search Central, SER, Google Ads, Meta, OpenAI, Shopify Dev Changelog (P13–P16, A01, G01, AI01, S04).
5. Візуальні тренди — **ЧАСТКОВО, ВРУЧНУ.** Pantone, Pinterest Predicts, Etsy/Shutterstock/Adobe — раз на рік (P17); у дайджест не йдуть (правило 12).
6. Ключові слова й попит — **НЕ ЗАКРИТО.** Google Trends — 429; Trends API — alpha за заявкою; Etsy API і Keyword Planner — не підключено.
7. Категорії, що ростуть — **ЧАСТКОВО.** Квартальні звіти Etsy/Shopify (P18, P19), Census/ONS; щомісячного трекера немає до Etsy API (V02).
8. Топ-магазини та їхнє просування — **ЧАСТКОВО.** RSS магазинів Etsy (P20) працює; продажі магазинів — лише через Etsy API (V02); рекламні бібліотеки — вручну.
9. Оновлення платформ — **ЗАКРИТО.** Shopify Changelog RSS (S01), Etsy Community (E05), специфікація Etsy API (P21), eBay Seller Updates (P22).
10. Топ-блогери й експерти — **ЧАСТКОВО.** Механізм є: YouTube RSS працює (P23), блоги з RSS; зміст відео — після Gemini key (P24); імена — чекають Славіка.
11. Експорт з України — **ЧАСТКОВО.** Нова пошта, Shopify Payments, e-Residency (P25–P27); Укрпошта — лише через пошук і контакт.

## Етсі — офіційні
- E01 · Etsy Seller Handbook (+Site Updates) · etsy.com/seller-handbook · 1 · ОФ · P1 · статус: активне · доступ: через пошук (сайт блокує ботів) · у фіналі: 1 (#13: AI-фото)
- E02 · Etsy News · etsy.com/news · 1 · ОФ · P2 · статус: активне · доступ: через пошук · у фіналі: 0
- E03 · Etsy Investor Relations · investors.etsy.com · 1 · ОФ · P1 у звітні тижні / P3 · статус: активне · доступ: curl напряму + RSS investors.etsy.com/news-events/press-releases/rss (перевірено 12.11.2026) · у фіналі: 1 (#13: Etsy Q3)
- E04 · SEC EDGAR (Etsy 10-Q/10-K/8-K) · sec.gov · 1 · ОФ · P3/звітні тижні · статус: активне · доступ: через пошук (сайт блокує ботів) · у фіналі: 3 (#13: Etsy Q3; маркетинг Etsy; 3 сигнали звіту)
- E05 · Etsy Community Announcements · community.etsy.com/forum/announcements-290 · 1 · ОФ · P1 · статус: активне · доступ: curl напряму · у фіналі: 1 (#13: апеляції)
- E06 · Etsy Help Center (Fees, House Rules, Creativity Standards) · help.etsy.com · 1 · ОФ · P2 · статус: активне · доступ: через пошук (сайт блокує ботів) · у фіналі: 1 (#13: Cyber Specials)
- E07 · Ranking Disclosures · etsy.com/legal · 1 · ОФ · P3 · статус: активне · доступ: через пошук (сайт блокує ботів) · у фіналі: 0
- E08 · Etsy Seller Trend Report · etsy.com/seller-handbook · 7 · ОФ · P3 (березень, жовтень) · статус: активне · доступ: через пошук · у фіналі: 0
- E09 · Etsy Trend Edit · etsyedit.com · 7 · ОФ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- E10 · Etsy Design Awards · etsy.com/etsydesignawards · 1 · ОФ · P3 (серпень–листопад) · статус: активне · доступ: через пошук (сайт блокує ботів) · у фіналі: 0
- E11 · Etsy Up / YouTube Etsy · youtube.com/@Etsy · 1 · ОФ · P3 (вересень–жовтень) · статус: активне · доступ: список відео — curl; субтитри — недоступні (від Славіка) · у фіналі: 0
- E12 · Соцмережі Etsy + керівництво (Kruti Patel Goyal, Dayna Isom Johnson) · — · 1 · ОФ · P2 · статус: активне · доступ: не перевірено · у фіналі: 0
- E13 · Etsy Seller newsletter · (пересилає Славік) · 1 · ОФ · P2 · статус: активне · доступ: ручне · у фіналі: 0

## Етсі — аналітики й інструменти
- EA01 · EcommerceBytes · ecommercebytes.com · 1 · ІНЖ · P1 · статус: активне · доступ: curl напряму · у фіналі: 0
- EA02 · Value Added Resource · valueaddedresource.net · 1 · ІНЖ · P1 · статус: активне · доступ: curl напряму · у фіналі: 3 (#13: Share & Save; AI-фото; «порадила спамити»)
- EA03 · CindyLouWho2 · cindylouwho2.com/blog · 1 · ІНЖ · P2 · статус: активне · доступ: не перевірено · у фіналі: 1 (#13: апеляції)
- EA04 · Marketplace Pulse · marketplacepulse.com · 1/10 · ІНЖ · P2 · статус: активне · доступ: curl напряму · у фіналі: 0
- EA05 · Marmalead blog · blog.marmalead.com · 1 · ІНЖ · P2 · статус: активне · доступ: не перевірено · у фіналі: 0
- EA06 · eRank blog/Help (+Top Sellers) · erank.com · 1/10 · ІНЖ · P2 · статус: активне · доступ: через пошук · у фіналі: 0
- EA07 · Alura · alura.io · 1 · ІНЖ · P3 · статус: активне · доступ: не перевірено · у фіналі: 1 (#13: Share & Save)
- EA08 · EverBee · everbee.io · 10 · ІНЖ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- EA09 · Koalanda · koalanda.com · 10 · ІНЖ · P3 щомісяця · статус: активне · доступ: не перевірено · у фіналі: 0
- EA10 · EtsyHunt, RankHero · — · 10 · ІНЖ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- EA11 · Growing Your Craft · growingyourcraft.com · 1 · ІНЖ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- EA12 · EcomCrew · ecomcrew.com · 1 · ІНЖ · P3 · статус: активне · доступ: через пошук · у фіналі: 0
- EA13 · Tamebay · tamebay.com · 1 · ІНЖ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- EA14 · Dylan Jahraus · — · 1 · ІНЖ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0

## Shopify — офіційні
- S01 · Shopify Changelog · changelog.shopify.com · 2 · ОФ · P1 · статус: активне · доступ: curl напряму · у фіналі: 0
- S02 · Shopify Editions · shopify.com/editions · 2 · ОФ · P1 (січень/червень/жовтень) · статус: активне · доступ: через пошук · у фіналі: 0
- S03 · Shopify Newsroom · shopify.com/news · 2 · ОФ · P1 · статус: активне · доступ: curl напряму · у фіналі: 1 (#13: Agentic)
- S04 · Shopify Developer Changelog · shopify.dev/changelog · 2 · ОФ · P2 · статус: активне · доступ: RSS shopify.dev/changelog/feed.xml; тег Action Required — окремо сторінкою ?tags=action-required (перевірено 12.11.2026) · у фіналі: 0
- S05 · Shopify Help Center · help.shopify.com · 2 · ОФ · P2 · статус: активне · доступ: curl напряму · у фіналі: 2 (#13: Agentic + Knowledge Base; Shop/Shop Pay умови)
- S06 · Shopify Blog (trend reports, trending products) · shopify.com/blog · 2/10 · ОФ/ІНЖ · P2 · статус: активне · доступ: curl напряму · у фіналі: 0
- S07 · Shopify Engineering · shopify.engineering · 2 · ОФ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- S08 · Shopify IR + SEC · investors.shopify.com · 2 · ОФ · P1 у звітні тижні · статус: активне · доступ: curl напряму, shopify.com/investors (перевірено 12.11.2026) · у фіналі: 1 (#13: Shopify Q3 + AI ×3,3)
- S09 · Shopify Magic/Sidekick · shopify.com/magic · 9 · ОФ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0

## Shopify — аналітики (вторинне, лише як підказка)
- SA01 · Shopifreaks · shopifreaks.com · 2 · ІНЖ · P2 · статус: активне · доступ: не перевірено · у фіналі: 0
- SA02 · Fudge.ai «Shopify Updates» · fudge.ai · 2 · ІНЖ · P2 · статус: активне · доступ: через пошук · у фіналі: 0
- SA03 · Huptech, Codilar, Flatline, AdsX, Ask Phill, Ambaum, Revize, Ecommerce-Platforms, Tante-E · — · 2 · ІНЖ (вендор) · P3 · статус: активне · доступ: не перевірено · у фіналі: 0

## Галузеві медіа
- M01 · Modern Retail · modernretail.co · 5–7 · ІНЖ · P1 · статус: активне · доступ: curl напряму · у фіналі: 2 (#13: ChatGPT; TikTok Shop)
- M02 · Digital Commerce 360 · digitalcommerce360.com · 1/2/10 · ІНЖ · P1 · статус: активне · доступ: через пошук · у фіналі: 1 (#13: AI-фото)
- M03 · Retail Dive · retaildive.com · 7 · ІНЖ · P2 · статус: активне · доступ: не перевірено · у фіналі: 0
- M04 · Supply Chain Dive · supplychaindive.com · 1 · ІНЖ · P2 · статус: активне · доступ: не перевірено · у фіналі: 0
- M05 · Practical Ecommerce · practicalecommerce.com · 5 · ІНЖ · P2 · статус: активне · доступ: через пошук · у фіналі: 0
- M06 · eCommerceFuel · ecommercefuel.com · 5 · ІНЖ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- M07 · PYMNTS · pymnts.com · 1/2 · ІНЖ · P2 · статус: активне · доступ: через пошук · у фіналі: 0
- M08 · TechCrunch · techcrunch.com · 9 · ІНЖ · P2 · статус: активне · доступ: через пошук · у фіналі: 0
- M09 · CNBC · cnbc.com · 7 · ІНЖ · P2 · статус: активне · доступ: не перевірено · у фіналі: 0
- M10 · Reuters · reuters.com · 7 · ІНЖ · P2 · статус: активне · доступ: не перевірено · у фіналі: 0
- M11 · Bloomberg · bloomberg.com · 7 · ІНЖ (пейвол) · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- M12 · Forbes, Business Insider, The Verge · — · 7 · ІНЖ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- M13 · Digiday · digiday.com · 4/6 · ІНЖ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- M14 · Motley Fool / Yahoo Finance (транскрипти) · — · 1/2 · ІНЖ · P3 у звітні тижні · статус: активне · доступ: не перевірено · у фіналі: 1 (#13: 3 сигнали звіту Etsy)
- M15 · eMarketer · emarketer.com · 7/10 · ІНЖ (частково платно) · P3 · статус: активне · доступ: через пошук · у фіналі: 0
- M16 · Oberlo · oberlo.com · 10 · ІНЖ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- M17 · Statista · statista.com · 10 · ІНЖ (лише з першоджерелом) · P3 · статус: активне · доступ: через пошук · у фіналі: 0

## Регуляторика, митниця, логістика
- R01 · CBP (FAQ, CSMS, прес-релізи) · cbp.gov · 1 · ОФ · P1 · статус: активне · доступ: через пошук (сайт блокує ботів) · у фіналі: 0
- R02 · Federal Register · federalregister.gov · 1 · ОФ · P1 · статус: активне · доступ: через пошук · у фіналі: 0
- R03 · White House · whitehouse.gov · 1 · ОФ · P2 · статус: активне · доступ: не перевірено · у фіналі: 0
- R04 · USPS · usps.com · 1 · ОФ · P3 сезонно · статус: активне · доступ: через пошук · у фіналі: 0
- R05 · CPSC · cpsc.gov · 1 · ОФ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- R06 · FTC / FCC · ftc.gov · 1 · ОФ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- R07 · European Commission, Taxation and Customs Union · taxation-customs.ec.europa.eu · 1 · ОФ · P1 · статус: активне · доступ: не перевірено · у фіналі: 0
- R08 · Council of the EU · consilium.europa.eu · 1 · ОФ · P2 · статус: активне · доступ: не перевірено · у фіналі: 0
- R09 · UK HMRC / gov.uk · gov.uk · 1 · ОФ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- R10 · Royal Mail · royalmail.com · 1 · ОФ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- R11 · Avalara blog · avalara.com/blog · 1 · ІНЖ · P1 · статус: активне · доступ: через пошук · у фіналі: 0
- R12 · Zonos · zonos.com · 1 · ІНЖ · P1 · статус: активне · доступ: не перевірено · у фіналі: 0
- R13 · Thomson Reuters ONESOURCE · — · 1 · ІНЖ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- R14 · Юрфірми (Thompson Hine, Alston & Bird, Snell & Wilmer, BDO, Crowell & Moring, Keller and Heckman) · — · 1 · ІНЖ · P3 · статус: активне · доступ: через пошук · у фіналі: 0
- R15 · ShipperHQ, Portless, Iscompliant, Gerlach · — · 1 · ІНЖ (вендор) · P3 · статус: активне · доступ: не перевірено · у фіналі: 0

## Україна
- U01 · Укрпошта (новини, e-export) · ukrposhta.ua · 1 · ОФ · P1 · статус: активне · доступ: через пошук (сайт і e-export блокують ботів, 403; перевірено 12.11.2026) · у фіналі: 0
- U02 · Нова Пошта Global / NP Shopping · novaposhta.ua, novaposhtaglobal.ua · 1 · ОФ · P2 · статус: активне · доступ: curl напряму (перевірено 12.11.2026) · у фіналі: 0
- U03 · Meest · meest.com · 1 · ОФ · P2 · статус: активне · доступ: не перевірено · у фіналі: 0
- U04 · SkladUSA · — · 1 · ОФ/вендор · P2 · статус: активне · доступ: не перевірено · у фіналі: 0
- U05 · Western Bid · westernbid.com · 1 · ІНЖ/вендор · P2 · статус: активне · доступ: не перевірено · у фіналі: 0
- U06 · DiFFreight · — · 1 · вендор · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- U07 · Payoneer newsroom · payoneer.com · 1 · ОФ · P2 · статус: активне · доступ: через пошук · у фіналі: 0
- U08 · PayPal Україна · — · 1 · ОФ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- U09 · Hutko, WayForPay · — · 2 · ОФ/вендор · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- U10 · Верховна Рада · rada.gov.ua · 1 · ОФ · P2 · статус: активне · доступ: не перевірено · у фіналі: 0
- U11 · ДПС / НБУ · tax.gov.ua, bank.gov.ua · 1 · ОФ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- U12 · buh.ua · buh.ua · 1 · ІНЖ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- U13 · Дія.Бізнес · business.diia.gov.ua · 1 · ОФ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- U14 · Made with Bravery · madewithbravery.com · 1 · ОФ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- U15 · Forbes.ua · forbes.ua · 1 · ІНЖ · P2 · статус: активне · доступ: через пошук · у фіналі: 0
- U16 · Інтерфакс-Україна · interfax.com.ua · 1 · ІНЖ · P2 · статус: активне · доступ: не перевірено · у фіналі: 0
- U17 · Mind.ua, dev.ua, LIGA, UNN, ThePage, Mezha, kurs.com.ua, epravda · — · 1 · ІНЖ · P3 · статус: активне · доступ: через пошук · у фіналі: 0

## Тренди й споживач (у новини — лише поведінка/економіка покупця, не продуктові тренди)
- T01 · Pantone · pantone.com · 7 · ОФ · P3 (грудень, лютий, вересень) · статус: активне · доступ: не перевірено · у фіналі: 0
- T02 · WGSN · wgsn.com · 7 · ОФ (платно) · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- T03 · Coloro · coloro.com · 7 · ОФ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- T04 · Pinterest Predicts / Newsroom / Trends · business.pinterest.com · 7 · ОФ · P3 (грудень) / P2 (Trends) · статус: активне · доступ: не перевірено · у фіналі: 1 (#13: Pinterest після Різдва)
- T05 · Faire Forecast · faire.com/forecast · 7/10 · ОФ · P3 (січень) · статус: активне · доступ: не перевірено · у фіналі: 0
- T06 · Shopify trend reports · shopify.com/blog · 7/10 · ОФ · P3 · статус: активне · доступ: через пошук · у фіналі: 0
- T07 · Vogue, WWD, FashionUnited, Sourcing Journal, InStyle, Elle Decor тощо · — · 7 · ІНЖ · P3 · статус: активне · доступ: не перевірено · у фіналі: 1 (#13: готовність купувати через AI)
- T08 · Trend Hunter · trendhunter.com · 7 · ІНЖ · P2 · статус: недоступне · доступ: curl 403 (Trend Hunter блокує ботів) → ручний перегляд Славіком раз на квартал, бот нагадує · у фіналі: 0
- T09 · Google Trends · trends.google.com · 7 · ОФ · P2 · статус: активне · доступ: curl 429 (Google блокує запити) → обов'язкові точкові перевірки 5–10 запитів під тему випуску через пошук · у фіналі: 0
- T10 · Glimpse · meetglimpse.com · 7 · ІНЖ (платно) · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- T11 · Adobe Digital Insights / DEI · business.adobe.com · 7/10 · ІНЖ · P2 у Q4 · статус: активне · доступ: через пошук · у фіналі: 1 (#13: онлайн США сезон)
- T12 · Deloitte, NRF, Salesforce, McKinsey, Mintel, NielsenIQ, DHL · — · 7/10 · ІНЖ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0

## Платний трафік
- A01 · Google Ads Help + Ads & Commerce Blog · blog.google · 4 · ОФ · P2 · статус: активне · доступ: не перевірено · у фіналі: 0
- A02 · Google Merchant Center Help · support.google.com/merchants · 3/4 · ОФ · P2 · статус: активне · доступ: не перевірено · у фіналі: 0
- A03 · Meta for Business / Help Center · facebook.com/business · 4 · ОФ · P2 · статус: активне · доступ: не перевірено · у фіналі: 0
- A04 · TikTok for Business / Seller Center · — · 4 · ОФ · P2 · статус: активне · доступ: не перевірено · у фіналі: 0
- A05 · Pinterest Business Help · — · 4 · ОФ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- A06 · Amazon Ads · — · 4 · ОФ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- A07 · Etsy Ads / Offsite Ads (Handbook, Fees policy) · etsy.com · 1/4 · ОФ · P1 · статус: активне · доступ: через пошук · у фіналі: 0
- A08 · Triple Whale, Varos, Tinuiti, Skai, WARC тощо · — · 4 · ІНЖ · P3 · статус: активне · доступ: не перевірено · у фіналі: 1 (#13: CPM +13%)
- A09 · Search Engine Land / Journal (PPC) · — · 3/4 · ІНЖ · P2 · статус: активне · доступ: через пошук · у фіналі: 0
- A10 · Social Media Examiner, Sprout Social · — · 4 · ІНЖ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- A11 · Klaviyo, Attentive, Omnisend, Postscript · — · 5 · ІНЖ · P3 (жовтень–грудень) · статус: активне · доступ: не перевірено · у фіналі: 0
- A12 · Baymard Institute · baymard.com · 5 · ІНЖ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0

## SEO / GEO
- G01 · Google Search Central + Status Dashboard · developers.google.com/search · 3 · ОФ · P1 · статус: активне · доступ: через пошук · у фіналі: 0
- G02 · Search Engine Land · searchengineland.com · 3 · ІНЖ · P1 · статус: активне · доступ: через пошук · у фіналі: 0
- G03 · Search Engine Journal · searchenginejournal.com · 3 · ІНЖ · P2 · статус: активне · доступ: через пошук · у фіналі: 0
- G04 · Ahrefs · ahrefs.com/blog · 3 · ІНЖ (вендор) · P2 · статус: активне · доступ: не перевірено · у фіналі: 0
- G05 · Semrush · semrush.com · 3 · ІНЖ (вендор) · P2 · статус: активне · доступ: не перевірено · у фіналі: 0
- G06 · SE Ranking, Similarweb, SparkToro, Seer, BrightEdge, Muck Rack, Otterly, Profound, Peec, Backlinko, BuiltWith · — · 3 · ІНЖ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0

## AI-інструменти
- AI01 · OpenAI news (ChatGPT shopping) · openai.com · 9/3 · ОФ · P1 · статус: активне · доступ: через пошук · у фіналі: 1 (#13: ChatGPT як канал пошуку)
- AI02 · Anthropic news · anthropic.com/news · 9 · ОФ · P2 · статус: активне · доступ: не перевірено · у фіналі: 0
- AI03 · Google: Gemini, AI Mode, UCP · blog.google · 9/3 · ОФ · P1 · статус: активне · доступ: через пошук · у фіналі: 0
- AI04 · Canva Newsroom · — · 9 · ОФ · P2 · статус: активне · доступ: не перевірено · у фіналі: 0
- AI05 · Adobe Firefly · blog.adobe.com · 9 · ОФ · P2 · статус: активне · доступ: не перевірено · у фіналі: 0
- AI06 · Kling, Veo, Seedance · — · 9 · ОФ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0

## Спільноти
- C01 · Reddit (r/Etsy, r/EtsySellers, r/shopify, r/ecommerce, r/PPC, r/handmade, r/smallbusiness) · reddit.com · 8 · АНОН · P1 · статус: активне · доступ: RSS (www.reddit.com/r/<sub>/new/.rss) · у фіналі: 4 (#13: мітка «Uses AI»; хвиля off-platform; Ads самі вмикаються; боти) · постійне джерело, не прибирати (Славік, 11.11.2026)
- C02 · Etsy Community Forums (гілки продавців) · community.etsy.com · 8 · АНОН · P1 · статус: активне · доступ: через пошук · у фіналі: 0
- C03 · LinkedIn · — · 8 · АНОН/ІНЖ · P2 · статус: активне · доступ: не перевірено · у фіналі: 0
- C04 · X / Threads · — · 8 · АНОН · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- C05 · FB-групи продавців · — · 8 · АНОН · P3 · статус: недоступне · доступ: логін · у фіналі: 0
- C06 · Substack галузеві · — · 8 · АНОН/ІНЖ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- C07 · Telegram: @EtsyBiznes, @EtsyBizChat (лише топ-питань продавців, не новини) · t.me · 8 · АНОН · P1 · статус: недоступне · доступ: потрібен експорт від Славіка (групи без веб-перегляду) · у фіналі: 0
- C08 · Handmade-Hub UA · — · 8 · АНОН · P2 · статус: активне · доступ: не перевірено · у фіналі: 0
- C09 · Українські Etsy-коучі (індикатор міфів) · — · 8 · АНОН · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- C10 · YouTube-креатори про Etsy · — · 8 · АНОН · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- C11 · Trustpilot · — · 8 · АНОН · P3 · статус: активне · доступ: не перевірено · у фіналі: 0

## Конкурентні маркетплейси (кластер 10)
- K01 · Amazon (IR, Seller Central news) · ir.aboutamazon.com · 10 · ОФ · P2 щомісяця/звітні тижні · статус: активне · доступ: через пошук · у фіналі: 0
- K02 · eBay (IR) · investors.ebayinc.com · 10 · ОФ · P2 щомісяця/звітні тижні · статус: активне · доступ: через пошук · у фіналі: 1 (#13: eBay Q3)
- K03 · TikTok Shop · — · 10 · ОФ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- K04 · Whatnot, Faire, Temu · — · 10 · ОФ/ІНЖ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- K05 · Artisans Cooperative, Finnalby · — · 10 · ІНЖ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0

## Додано 11.11.2026 (дали новини у фінал #13, рішення Славіка: активні)
- N01 · PPC Land · ppc.land · 1/2/4 · ІНЖ · P2 · статус: активне · доступ: через пошук · у фіналі: 2 (#13: Shopify Q3 + AI ×3,3; AI-фото)
- N02 · Campaign / LBB / Shots (рекламна преса) · campaignlive.com, lbbonline.com, shots.net · 6 · ІНЖ · P3 · статус: активне · доступ: через пошук · у фіналі: 1 (#13: святкова реклама Etsy)
- N03 · PayPal Newsroom / Payments Dive · newsroom.paypal-corp.com, paymentsdive.com · 7 · ОФ/ІНЖ · P3 · статус: активне · доступ: через пошук · у фіналі: 1 (#13: тривога покупців і BNPL)
- N04 · Adweek · adweek.com · 6/7 · ІНЖ · P3 · статус: активне · доступ: через пошук · у фіналі: 1 (#13: Deloitte 16% про AI-покупки)
- I01 · Кабінети магазинів і команда МБ (внутрішнє) · Etsy Shop Manager, Shopify Admin, чат команди · 1/2 · дані каналу · P1 · статус: активне · доступ: скріни й нотатки від Славіка і команди · у фіналі: 6 (#13: Share & Save; Quick list; перейменування варіацій; Holiday checklist; Knowledge Base; Shop/Shop Pay)

## На випробуванні (вертикалі 1 і 4; не впроваджено до рішення Славіка)
- V01 · Google Ads Keyword Planner (через акаунт Славіка) · ads.google.com · вертикаль 1 · ОФ · P2 · статус: на випробуванні · доступ: не підключено — умови в sources/access_setup.md · у фіналі: 0
- V02 · Etsy Open API v3 · openapi.etsy.com · вертикаль 4 · ОФ · P2 · статус: на випробуванні · доступ: потрібен ключ застосунку (Славік реєструє) · у фіналі: 0

## Перевірено 12.11.2026 (дослідження джерел; висновки — research_notes/2026-11-12_sources_check.md)
Нові рядки. Статус «на випробуванні» = висновок ПІДКЛЮЧАЮ або НА ВИПРОБУВАННІ; «ручний перегляд» = ВРУЧНУ. Наявні рядки реєстру вище не змінено — розбіжності доступу перелічено в кінці розділу.
- P01 · US Census, Quarterly Retail E-Commerce · census.gov/retail/ecommerce.html · верт. 1/7 · ОФ · P3 (щокварталу) · статус: на випробуванні · доступ: curl напряму · у фіналі: 0
- P02 · ONS Retail sales GB (бюлетень + датасет internet sales, ряд J4MC) · ons.gov.uk · верт. 1/7 · ОФ · P3 (щомісяця) · статус: на випробуванні · доступ: curl напряму · у фіналі: 0
- P03 · Eurostat, E-commerce statistics for individuals (+ API isoc_ec_ibuy) · ec.europa.eu/eurostat · верт. 1/3 · ОФ · P3 (раз на рік, лютий) · статус: на випробуванні · доступ: curl напряму, API без ключа · у фіналі: 0
- P04 · ABS Monthly Household Spending Indicator · abs.gov.au · верт. 1 · ОФ (інша методологія) · P3 · статус: на випробуванні · доступ: curl напряму · у фіналі: 0
- P05 · Stats NZ Electronic card transactions · stats.govt.nz · верт. 1 · ОФ (інша методологія) · P3 · статус: на випробуванні · доступ: curl напряму, xlsx · у фіналі: 0
- P06 · Federal Register — API і RSS документів CBP · federalregister.gov/api/v1 · верт. 2 · ОФ · P1 · статус: на випробуванні · доступ: API і RSS без ключа · у фіналі: 0
- P07 · Thompson Hine SmarTrade · thompsonhinesmartrade.com/feed · верт. 2 · ІНЖ · P2 · статус: на випробуванні · доступ: RSS · у фіналі: 0
- P08 · KPMG TaxNewsFlash · kpmg.com/us/en/taxnewsflash.html · верт. 2 · ІНЖ · P3 · статус: на випробуванні · доступ: curl напряму · у фіналі: 0
- P09 · AIN.ua · ain.ua/feed · верт. 2/11 · ІНЖ · P2 · статус: на випробуванні · доступ: RSS · у фіналі: 0
- P10 · Mind.ua · s.mind.ua/rss/ua/all.xml · верт. 2/11 · ІНЖ · P2 · статус: на випробуванні · доступ: RSS (незвичне кодування) · у фіналі: 0
- P11 · McKinsey Insights · mckinsey.com/insights/rss · верт. 3 · ІНЖ · P2 · статус: на випробуванні · доступ: RSS · у фіналі: 0
- P12 · Deloitte Insights, Bain, Kantar, NielsenIQ, Circana · — · верт. 3 · ІНЖ · P3 (раз на місяць) · статус: на випробуванні · доступ: curl напряму (сторінки) · у фіналі: 0
- P13 · Search Engine Roundtable · seroundtable.com/index.rdf · верт. 4 · ІНЖ · P2 · статус: на випробуванні · доступ: RSS · у фіналі: 0
- P14 · Meta Newsroom · about.fb.com/feed · верт. 4 · ОФ · P2 · статус: на випробуванні · доступ: RSS · у фіналі: 0
- P15 · TikTok Newsroom · newsroom.tiktok.com/en-us · верт. 4 · ОФ · P3 · статус: на випробуванні · доступ: curl напряму · у фіналі: 0
- P16 · Google Search Central Blog RSS · developers.google.com/search/blog/feed.xml · верт. 4 · ОФ · P1 · статус: на випробуванні · доступ: RSS (доповнює G01) · у фіналі: 0
- P17 · Річні звіти візуальних трендів: Shutterstock, Adobe Stock (+ Pantone T01, Pinterest Predicts T04, Etsy Trend Report E08) · — · верт. 5 · ОФ · P3 (грудень) · статус: ручний перегляд · доступ: Shutterstock і Adobe 403 → через пошук · у фіналі: 0
- P18 · Etsy IR — прес-релізи RSS · investors.etsy.com/news-events/press-releases/rss · верт. 7 · ОФ · P1 у звітні тижні · статус: на випробуванні · доступ: RSS · у фіналі: 0
- P19 · Shopify IR + Shopify News · shopify.com/investors · верт. 7 · ОФ · P1 у звітні тижні · статус: на випробуванні · доступ: curl напряму · у фіналі: 0
- P20 · RSS магазинів Etsy (за списком Славіка) · etsy.com/shop/НАЗВА/rss · верт. 8 · ОФ · P2 · статус: на випробуванні · доступ: RSS (10 останніх лістингів), чекає списку магазинів · у фіналі: 0
- P21 · Специфікація Etsy Open API (порівняння щотижня) · etsy.com/openapi/generated/oas/3.0.0.json · верт. 9 · ОФ · P3 · статус: на випробуванні · доступ: curl напряму · у фіналі: 0
- P22 · eBay Seller Updates + Community Announcements · ebay.com/sellercenter/resources/seller-updates · верт. 9 · ОФ · P2 · статус: на випробуванні · доступ: curl напряму · у фіналі: 0
- P23 · YouTube RSS каналів (список нових відео; блогери — після імен від Славіка) · youtube.com/feeds/videos.xml · верт. 10 · — · P2 · статус: на випробуванні · доступ: RSS · у фіналі: 0
- P24 · Gemini API — зміст публічних YouTube-відео · ai.google.dev · верт. 10 · ОФ · P2 · статус: на випробуванні · доступ: потрібен ключ (Славік) · у фіналі: 0
- P25 · Нова пошта / Nova Poshta Global · novaposhta.ua, novaposhtaglobal.ua · верт. 11 · ОФ · P2 · статус: на випробуванні · доступ: curl напряму · у фіналі: 0
- P26 · Shopify Payments — supported countries · help.shopify.com · верт. 11 · ОФ · P3 · статус: на випробуванні · доступ: curl напряму (буває 403 «Verifying your connection», повтор допомагає) · у фіналі: 0
- P27 · e-Residency Естонії · e-resident.gov.ee · верт. 11 · ОФ · P3 · статус: на випробуванні · доступ: curl напряму (FAQ — 403) · у фіналі: 0
- P28 · Google Trends API alpha · developers.google.com/search/apis/trends · верт. 6 · ОФ · P2 · статус: на випробуванні · доступ: потрібна заявка й схвалення Google · у фіналі: 0
- P29 · Shopify /products.json окремих магазинів · <магазин>/products.json · верт. 8 · неофіційно · P3 · статус: на випробуванні · доступ: залежить від магазину (Allbirds 200, Gymshark 403) · у фіналі: 0
- P30 · Блоги з RSS: Seth Godin, Simon Willison, One Useful Thing (Mollick) · — · верт. 10 · ІНЖ · P3 · статус: на випробуванні · доступ: RSS · у фіналі: 0
- P31 · CBP CSMS (бюлетені митниці) · content.govdelivery.com/accounts/USDHSCBP · верт. 2 · ОФ · P2 · статус: ручний перегляд · доступ: окремі бюлетені відкриваються, стрічки немає (406) · у фіналі: 0
- P32 · Економічна правда · epravda.com.ua · верт. 2/11 · ІНЖ · P3 · статус: ручний перегляд · доступ: 403 → через пошук · у фіналі: 0
- P33 · BCG, PwC Voice of the Consumer · — · верт. 3 · ІНЖ · P3 · статус: ручний перегляд · доступ: 403 → через пошук · у фіналі: 0
- P34 · Amazon Best Sellers / Movers & Shakers · amazon.com/Best-Sellers/zgbs · верт. 7 · ОФ · P3 (раз на місяць) · статус: ручний перегляд · доступ: технічно 200, але умови Amazon проти роботів → очима · у фіналі: 0
- P35 · Meta Ad Library, Google Ads Transparency Center, TikTok Creative Center · — · верт. 8 · ОФ · P3 · статус: ручний перегляд · доступ: 403 / 429 / рендер скриптом · у фіналі: 0
- P36 · Amazon Seller Central News · sellercentral.amazon.com · верт. 9 · ОФ · P3 · статус: ручний перегляд · доступ: потрібен логін · у фіналі: 0
- P37 · X API (pay-per-use) · docs.x.com · верт. 10 · ОФ · P3 · статус: ручний перегляд · доступ: платно, поки без акаунтів для стеження · у фіналі: 0
- P38 · Instagram, TikTok (акаунти блогерів) · — · верт. 10 · — · P3 · статус: ручний перегляд · доступ: лише вручну · у фіналі: 0

Розбіжності з наявними рядками:
- E03, S08, S04, U01, U02 — виправлено 12.11.2026 («так» Славіка).
- G01, A01: «через пошук» / «не перевірено» — RSS працюють (див. P16; A01 не змінено, на рішення).
- V02 Etsy Open API: потрібен саме Personal App (Seller App обмежений своїм магазином); ключ — keystring:shared_secret.

## Вертикаль 10 — YouTube-канали (рішення Славіка 12.11.2026; доступ: RSS youtube.com/feeds/videos.xml?channel_id=…, перевірено 12.11.2026, усі 200 і по 15 відео)
Зміст відео — після Gemini API key (P24). Авторитетність бот не перевіряв — канали обрав Славік.
- Y01 · Alex Hormozi · youtube.com/@AlexHormozi · channel_id UCUyDOdBWhC1MCxEjC46d-zw · верт. 10 (бізнес) · P3 · статус: на випробуванні · доступ: RSS · у фіналі: 0
- Y02 · The Futur · youtube.com/@TheFutur · channel_id UC-b3c7kxa5vU-bnmaROgvog · верт. 10 (бренд, ціни) · P3 · статус: на випробуванні · доступ: RSS · у фіналі: 0
- Y03 · The Diary Of A CEO · youtube.com/@TheDiaryOfACEO · channel_id UCGq-a57w-aPwyi3pW7XLiHw · верт. 10 (бізнес) · P3 · статус: на випробуванні · доступ: RSS · у фіналі: 0
- Y04 · Seth Godin (блог) · seths.blog/feed · верт. 10 (маркетинг) · P3 · статус: на випробуванні · доступ: RSS · у фіналі: 0
- Y05 · Etsy Success · youtube.com/@EtsySuccess · channel_id UCO9e0tqE1Zh-iHtofu08pxA · верт. 10/9 (Etsy, офіційний) · P2 · статус: на випробуванні · доступ: RSS · у фіналі: 0
- Y06 · Dylan Jahraus · youtube.com/@dylanjahraus · channel_id UCeO8Gmc2B-3G2fgcFnRR4Xw · верт. 10 (Etsy) · P2 · статус: на випробуванні · доступ: RSS · у фіналі: 0
- Y07 · Matt Diggity · youtube.com/@MattDiggity · channel_id UCP5A5lVxaT7cO_LehpxjTZg · верт. 10 (SEO) · P3 · статус: на випробуванні · доступ: RSS (останнє відео 17.08.2026) · у фіналі: 0
- Y08 · Mark Tilbury · youtube.com/@marktilbury · channel_id UCxgAuX3XZROujMmGphN_scA · верт. 10 (бізнес, AI) · P3 · статус: на випробуванні · доступ: RSS · у фіналі: 0
- Y09 · Shopify · youtube.com/@shopify · channel_id UCIv38OrggTu3vNkCAo96-CQ · верт. 10/9 (Shopify, офіційний) · P2 · статус: на випробуванні · доступ: RSS · у фіналі: 0
- Y10 · Learn With Shopify · youtube.com/@learnwithshopify · channel_id UC7geKfz2-IH0rsgRBtHTm0g · верт. 10/9 (Shopify, офіційний) · P2 · статус: на випробуванні · доступ: RSS · у фіналі: 0
- Y11 · Davie Fogarty · youtube.com/@DavieFogarty · channel_id UC-JHxwWL4-WoqyQIYsBvTbA · верт. 10 (DTC, медіабаїнг) · P3 · статус: на випробуванні · доступ: RSS (останнє відео 29.09.2026) · у фіналі: 0
- Y12 · Kate Hayes · youtube.com/@KateHayes · channel_id UCfXzRcRPMHw_AF7EdRtyiJQ · верт. 10 · P3 · статус: на випробуванні — пробний канал (Славік: «на випробуванні»), рахувати окремо · доступ: RSS · у фіналі: 0
Пов'язані рядки: EA14 Dylan Jahraus і E11 YouTube Etsy лишаються як є; Y06 і Y05 — їхній канал-доступ.
