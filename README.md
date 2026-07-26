# Meme Radar — DLMM Edition 📡

**Free, open-source Solana memecoin scanner. 12 checks to cut the memecoin jungle down to a shortlist worth a manual look — built with DLMM entries in mind.**

> ⚠️ **This is not a miracle tool.** It is one tool among others. It will not find you the next 100x, it will not remove the risk, and a clean score can still rug. It filters the obvious garbage so you can spend your attention on the few candidates that deserve real due diligence. The decision — and the risk — stay 100% yours. Read the [full disclaimer](DISCLAIMER.md).

<!-- screenshot desktop ici -->

---

## What it does

Hundreds of tokens launch on Solana every day. Checking each one by hand — mint authority, LP lock, holder distribution, dev wallet history — takes minutes per token. This scanner does those checks automatically, continuously, and ranks what survives.

The angle: it was built by a [Meteora DLMM](https://meteora.ag) liquidity provider, for DLMM entries. It can filter for tokens with DLMM pools and favors the profile that matters for LPing (real holders, real volume, liquidity depth) rather than pure momentum chasing.

**One HTML file. No server, no signup, no wallet connection — ever.** It runs entirely in your browser; your API keys are stored locally and never leave your machine.

## The 12 checks

Each token is scored against 12 criteria, including:

- **Mint & freeze authority** revoked
- **LP locked / burned**
- **Bundle detection** (supply grouped at launch)
- **Holder count & growth** (configurable minimum, unique on-chain owners — not the inflated numbers)
- **Top-10 holder concentration**
- **Snipers / insiders share**
- **DLMM pool available** (only / first — toggleable)
- **Dev wallet age & behavior** (fresh wallets are a red flag)
- **Flagged serial deployers** (known rugger wallets, editable list)
- **Tribute-token detection** (tokens riding a KOL's name, editable list)

On top of the score, a **risk index** aggregates penalties, plus:

- 🌀 **Wash-trading heuristic** — unique buyers/sellers per hour vs. volume
- ⛔ **Security cross-check** — transfer fees, hooks, mutable balances (GoPlus vs. RugCheck divergences)
- ♻️ **Recycled ticker detection**
- 𝕏 **Social signals** — account link, mentions, community size (informational only)
- Organic score & suspicious-audit flag from Jupiter

## Data sources

[DexScreener](https://dexscreener.com) · [RugCheck](https://rugcheck.xyz) · [Helius](https://helius.dev) · [Jupiter](https://jup.ag) · [GeckoTerminal](https://geckoterminal.com) · [GoPlus](https://gopluslabs.io)

All free public endpoints. The only key you need is a **free Helius API key** (used for unique-holder counts and dev wallet history).

## Getting started

1. **Download** `meme_radar.html` (desktop) or `meme_radar_mobile.html` (phone)
2. **Open it** in Chrome (or any modern browser)
3. **Paste your free Helius API key** in the settings — get one at [helius.dev](https://helius.dev) in two minutes
4. Let it scan. Adjust filters (token age, liquidity floor, DLMM only, minimum holders) to taste.

Your settings, flagged-dev list and KOL list persist locally in your browser (localStorage). Export/import them as JSON from the settings panel.

## What it is NOT

- ❌ Not financial advice
- ❌ Not a buy signal
- ❌ Not a guarantee — a clean score can still rug; a flagged token can still pump
- ❌ Not protection against DLMM-specific risks: divergence loss on a volatile token can eat an LP position even when the token doesn't rug

## Support the project

If this saved you from one rug, that's the whole business model 🤝

**SOL donations:** `Em5aKcZ6VvmFnYmAcUDCodkoiBokGGSYabhFRwh9rb3A`

Follow [@DLMMRadar](https://x.com/DLMMRadar) for flagged-token receipts and updates.

## License

[MIT](LICENSE) — do what you want with it, at your own risk.

---

## 🇫🇷 Version française

**Scanner de memecoins Solana, gratuit et open-source. 12 critères pour réduire la jungle à une courte liste méritant un vrai examen — pensé pour les entrées DLMM.**

Ce n'est **pas un outil miracle** : c'est un outil parmi d'autres. Il ne trouvera pas le prochain x100 et n'élimine pas le risque — un bon score peut quand même rugger. Il trie les pièges évidents pour que vous concentriez votre attention sur les rares candidats qui méritent une vraie analyse. La décision, et le risque, restent 100 % les vôtres.

**Un simple fichier HTML.** Pas de serveur, pas d'inscription, jamais de connexion wallet. Tout tourne dans votre navigateur ; vos clés API restent en local.

**Démarrage :** téléchargez `meme_radar.html` (ordinateur) ou `meme_radar_mobile.html` (mobile), ouvrez-le dans Chrome, collez votre clé Helius gratuite ([helius.dev](https://helius.dev)) dans les réglages. L'interface est disponible en français et en anglais (bouton FR/EN).

Les 12 critères couvrent : autorités mint/freeze révoquées, LP verrouillée, détection de bundles, nombre et croissance des holders réels, concentration du top 10, part des snipers/insiders, présence d'un pool DLMM, âge et comportement du wallet du dev, deployers en série fichés, détection des tokens « tribute ». S'y ajoutent un indice de risque, une heuristique de wash trading, un croisement de sécurité GoPlus/RugCheck, la détection de tickers recyclés et des signaux sociaux 𝕏.

**Dons (SOL) :** `Em5aKcZ6VvmFnYmAcUDCodkoiBokGGSYabhFRwh9rb3A`
