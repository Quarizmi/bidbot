# Bidbot

> Smart bidding for long-tail keywords on Google Ads — with traffic and conversion forecasts before you raise a bid.

Bidbot is an open-source bidding bot built by [Quarizmi](https://quarizmi.com). It's designed for long-tail keyword strategies: it decides the right bid for each keyword, decides which keywords to turn on or off, and predicts the traffic and conversion lift you'd get from raising a bid — so every bid change is an informed one.

---

## Features

- **Long-tail bid optimization** — sets the right bid for each long-tail keyword.
- **Keyword on/off decisions** — identifies which keywords to activate and which to pause.
- **Lift forecasting** — predicts the traffic and conversion increase from a bid increase before you make it.
- **Organic awareness** — checks which keywords already show up in organic results, so you don't overpay for traffic you'd get anyway.
- **Beyond-the-click view** — uses analytics data to judge performance on the site, not just inside the ad platform.

## Data sources

| Source | What Bidbot uses it for |
|---|---|
| Client historical data | Past bid, traffic, and conversion performance |
| Google Keyword Planner | Google's traffic and bid estimates |
| Google Search Console | Keywords already ranking organically |
| Google Analytics | Post-click engagement and conversions |
| Google Ads API | Reading account data and applying bid changes |

Bidbot combines your own historical data with Google's estimates to build its forecasts — the blend is what makes the predictions reliable.

## How it works

```
 Historical data ─┐
 Keyword Planner ─┤
 Search Console ──┼──► Forecast lift ──► Decide bid / on / off ──► Google Ads API
 Analytics ───────┘
```

## Getting started

> **Note:** The implementation language and setup steps are still being finalized. This section will be updated.

### Prerequisites

- Google Ads API access (developer token + OAuth credentials)
- Google Search Console API access
- Google Analytics API access
- _TBD: runtime and dependencies_

### Installation

```bash
git clone https://github.com/<org>/bidbot.git
cd bidbot
# TBD: install dependencies
```

### Configuration

```bash
# TBD: environment variables / config file for API credentials and bid rules
```

### Running

```bash
# TBD: run command
```

## Part of the Quarizmi suite

Bidbot works on its own, but it's also part of Quarizmi's end-to-end paid-search system:

- **[EKEP](../ekep)** — discovers long-tail keywords
- **Bidbot** — decides bids and which keywords to turn on or off _(you are here)_
- **[Usable](../usable)** — builds full campaigns with the user in the loop
- **[Magneto](../magneto)** — writes high-relevance ads for every keyword
- **[Health Checker](../health-checker)** — grades an existing Google Ads account (standalone)

## Use it yourself, or work with us

Bidbot is free and open source — use it, fork it, adapt it. If you'd rather have it run for you, Quarizmi can set it up and operate it on your account. Get in touch at **[quarizmi.com](https://quarizmi.com)**.

## Contributing

Contributions are welcome. Please open an issue to discuss a change before submitting a pull request.

## License

Released under the [MIT License](LICENSE). © 2026 Quarizmi AdTech.
