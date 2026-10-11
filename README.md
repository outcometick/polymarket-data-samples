# Polymarket Crypto Up/Down Market Data — Full Edition · Free Sample

[Polymarket historical data](https://outcometick.com/polymarket-historical-data) for the crypto Up/Down markets, collected 24/7 by [OutcomeTick](https://outcometick.com). This repository hosts a **free sample** of the
full edition: one real, unmodified UTC day (2026-09-08), laid out exactly as the delivered archive, so code
written against the sample runs unchanged on the full data.

> **中文：** 本仓库是 [OutcomeTick](https://outcometick.com/zh) 采集的[Polymarket 历史数据](https://outcometick.com/zh/polymarket-historical-data)（加密 Up/Down 市场）完整版的**免费样本**：一个真实、未经修改的
> UTC 日（2026-09-08），目录结构与正式交付的数据完全一致，针对样本写的代码可以原样用在正式数据上。

## Download / 下载

**[polymarket-data-samples.tar.gz](https://github.com/outcometick/polymarket-data-samples/releases/latest/download/polymarket-data-samples.tar.gz)**

```bash
curl -L https://github.com/outcometick/polymarket-data-samples/releases/latest/download/polymarket-data-samples.tar.gz | tar xz
```

Per-file row counts and sha256: [`samples/manifest.json`](samples/manifest.json).
Field reference: [DATA_GUIDE.md](DATA_GUIDE.md) · 中文字段说明：[数据使用说明.md](数据使用说明.md)

## What the full edition contains / 完整版包含的数据

- **[Order book](https://outcometick.com/polymarket-order-book-data)** — full-depth snapshots, incremental updates, and best bid/ask
- **Trades** — price, size, side, millisecond timestamp, on-chain tx hash
- **Markets** — the opening price (price to beat), the settled outcome, each market's own TWAP settlement config
- **[Chainlink settlement streams](https://outcometick.com/chainlink-settlement-data)** — instantaneous, TWAP30s and TWAP60s
- **Klines** — OHLC built from the settlement stream, 1 second to 1 month
- Seven assets, 5-minute and 15-minute markets

> **中文：** 盘口快照 + 增量 + 最优价、逐笔成交、市场信息（开盘价、结算结果、TWAP 结算配置）、Chainlink 瞬时 / TWAP30s / TWAP60s 结算流、K 线；7 个币种、5 分钟 / 15 分钟市场。

## Files in this sample / 样本包含的文件

| path | rows |
|---|---|
| `data/chainlink/daily/prices/BTCUSD/BTCUSD-prices-2026-09-08.csv.gz` | 81,970 |
| `data/chainlink-twap-30s/daily/prices/BTCUSD/BTCUSD-twap30s-prices-2026-09-08.csv.gz` | 81,946 |
| `data/chainlink-twap-60s/daily/prices/BTCUSD/BTCUSD-twap60s-prices-2026-09-08.csv.gz` | 81,969 |
| `data/polymarket/daily/markets/BTC-5m/BTC-5m-markets-2026-09-08.jsonl.gz` | 292 |
| `data/polymarket/daily/book/BTC-5m/BTC-5m-book-2026-09-08.jsonl.gz` | 141,402 |
| `data/polymarket/daily/price_change/BTC-5m/BTC-5m-price_change-2026-09-08.jsonl.gz` | 3,516,537 |
| `data/polymarket/daily/best_bid_ask/BTC-5m/BTC-5m-best_bid_ask-2026-09-08.jsonl.gz` | 1,314,078 |
| `data/polymarket/daily/last_trade_price/BTC-5m/BTC-5m-last_trade_price-2026-09-08.jsonl.gz` | 480,491 |

## Learn more / 了解更多

- [OutcomeTick](https://outcometick.com) — prediction-market data for Polymarket and Predict.fun · [中文站](https://outcometick.com/zh)
- [Documentation](https://outcometick.com/docs) — quickstart and complete task examples · [中文文档](https://outcometick.com/zh/docs)
- [API reference](https://outcometick.com/docs/api) · [Data schemas](https://outcometick.com/docs/schemas) · [Settlement rules](https://outcometick.com/docs/settlement)
- [Settlement statistics for BTC](https://outcometick.com/data/polymarket/btc) — per-asset data page
- [Backtest in the browser](https://outcometick.com/backtest) — run a strategy on the archive without downloading anything
- Community / 社区: [Discord](https://discord.gg/ZDMqkptwm5) (English and 中文) · [Telegram](https://t.me/+TcK_hJOzOz5mZTk1)

The full data is delivered with an API key and downloaded by day, asset and interval.
正式数据通过 API key 交付，按天、按币种、按周期下载。

For research and backtesting only; not investment advice. / 仅供研究与回测，不构成投资建议。
