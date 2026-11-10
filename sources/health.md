# Здоров'я джерел

Формат: дата · id · доступ (відкрилось / заблоковано / логін / пейвол / через пошук) · тез у дайджесті · що пройшло гейт · примітка.

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
