# Реєстр джерел v1.0 (нормалізований)

Основа: «Реєстр джерел для щотижневого моніторингу» v1.0 від 10.11.2026. Формат рядка (оновлено 11.11.2026, правило 14):
`id · назва · URL · кластер · клас · пріоритет · статус · доступ · у фіналі: N`
Статус: активне / на випробуванні / недоступне / прибране.
Доступ: curl напряму · RSS · через пошук (сайт недоступний напряму або блокує ботів) · не перевірено · недоступне (причина).
У фіналі: скільки новин із джерела дійшло до фінального сценарію; оновлюється після кожного випуску. Зміни статусу — лише після «так» Славіка.

## Етсі — офіційні
- E01 · Etsy Seller Handbook (+Site Updates) · etsy.com/seller-handbook · 1 · ОФ · P1 · статус: активне · доступ: через пошук (сайт блокує ботів) · у фіналі: 1 (#13: AI-фото)
- E02 · Etsy News · etsy.com/news · 1 · ОФ · P2 · статус: активне · доступ: через пошук · у фіналі: 0
- E03 · Etsy Investor Relations · investors.etsy.com · 1 · ОФ · P1 у звітні тижні / P3 · статус: активне · доступ: через пошук (сайт блокує ботів) · у фіналі: 1 (#13: Etsy Q3)
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
- S04 · Shopify Developer Changelog · shopify.dev/changelog · 2 · ОФ · P2 · статус: активне · доступ: не перевірено · у фіналі: 0
- S05 · Shopify Help Center · help.shopify.com · 2 · ОФ · P2 · статус: активне · доступ: curl напряму · у фіналі: 2 (#13: Agentic + Knowledge Base; Shop/Shop Pay умови)
- S06 · Shopify Blog (trend reports, trending products) · shopify.com/blog · 2/10 · ОФ/ІНЖ · P2 · статус: активне · доступ: curl напряму · у фіналі: 0
- S07 · Shopify Engineering · shopify.engineering · 2 · ОФ · P3 · статус: активне · доступ: не перевірено · у фіналі: 0
- S08 · Shopify IR + SEC · investors.shopify.com · 2 · ОФ · P1 у звітні тижні · статус: активне · доступ: через пошук (сайт блокує ботів) · у фіналі: 1 (#13: Shopify Q3 + AI ×3,3)
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
- U01 · Укрпошта (новини, e-export) · ukrposhta.ua · 1 · ОФ · P1 · статус: активне · доступ: не перевірено · у фіналі: 0
- U02 · Нова Пошта Global / NP Shopping · — · 1 · ОФ · P2 · статус: активне · доступ: не перевірено · у фіналі: 0
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
- T08 · Trend Hunter · trendhunter.com · 7 · ІНЖ · P2 · статус: недоступне · доступ: curl 403 (Trend Hunter блокує ботів) · у фіналі: 0
- T09 · Google Trends · trends.google.com · 7 · ОФ · P2 · статус: активне · доступ: curl 429 (Google блокує запити; є лише RSS трендів дня) · у фіналі: 0
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
- C01 · Reddit (r/Etsy, r/EtsySellers, r/shopify, r/ecommerce, r/PPC, r/handmade, r/smallbusiness) · reddit.com · 8 · АНОН · P1 · статус: активне · доступ: RSS (www.reddit.com/r/<sub>/new/.rss) · у фіналі: 4 (#13: мітка «Uses AI»; хвиля off-platform; Ads самі вмикаються; боти)
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
