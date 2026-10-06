# Polymarket 加密涨跌市场数据 · 完整版 · 免费样本

Polymarket 加密 Up/Down 市场数据完整版的**免费样本**：一个真实、未经修改的 UTC 日（2026-09-08），
目录结构与正式交付的数据完全一致，针对样本写的代码可以原样用在正式数据上。

Free sample of the Polymarket crypto Up/Down market data (full edition): one real,
unmodified UTC day (2026-09-08), laid out exactly as the delivered archive.

## 下载 / Download

**[polymarket-data-samples.tar.gz](https://github.com/outcometick/polymarket-data-samples/releases/latest/download/polymarket-data-samples.tar.gz)**

```bash
curl -L https://github.com/outcometick/polymarket-data-samples/releases/latest/download/polymarket-data-samples.tar.gz | tar xz
```

每个文件的行数与 sha256 见 [`samples/manifest.json`](samples/manifest.json)；字段说明见
[数据使用说明.md](数据使用说明.md)（English: [DATA_GUIDE.md](DATA_GUIDE.md)）。

## 样本包含的文件 / Files in this sample

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

## 正式数据 / Full data

正式数据通过 API key 交付，按天、按币种、按周期下载。接口文档：https://outcometick.com/docs

仅供研究 / 回测，不构成投资建议。
