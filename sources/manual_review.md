# Ручний перегляд (бот не бачить ці джерела)

## Telegram-чати (рішення Славіка 10.11.2026)
- https://t.me/EtsyBiznes
- https://t.me/EtsyBizChat
Мета: щопонеділка — **топ-10 питань продавців тижня** (не новини, а «що болить»), щоб частину розбирати в ефірі.
Статус: t.me заблоковано мережею сесії.
Варіанти розблокування:
1. Додати `t.me` в allowed hosts середовища (claude.ai/code → середовище → Network). Тоді бот читає публічний веб-перегляд t.me/s/<канал> (працює лише для публічних каналів; для груп-чатів веб-перегляду може не бути).
2. Надійніше: раз на тиждень Telegram Desktop → чат → «Export chat history» (JSON, лише текст, за 7 днів) → покласти в Google Drive у папку бота. Бот читає з Drive.

## Reddit
r/Etsy, r/EtsySellers, r/shopify, r/ecommerce — Славік не читає; доступ заблоковано мережею. Варіант: додати `www.reddit.com` в allowed hosts (Reddit часто блокує ботів і так — тоді фолбек: переказ через EcommerceBytes / Value Added Resource з позначкою [переказ]).

## Логін / пейвол
eRank Top Sellers · Etsy Community (частина гілок) · FB-групи · WGSN · Glimpse · Bloomberg.
