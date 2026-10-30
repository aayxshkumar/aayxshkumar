### Aayush Kumar

I'm a software engineer at **Airbus**, where I build C++/Qt software for an iPad app that 40,000 pilots use every day. I care about the parts of software that have to be fast, predictable and correct.

**Currently building:** [`lob-engine`](https://github.com/aayxshkumar/lob-engine), a C++20 limit order book and matching engine. It's tested against a naive reference book on every operation. Two measured steps took it from 20.9M to 35.7M to 65.2M operations per second: flat price-level arrays with a bitset, then an open-addressing table in place of `std::unordered_map`. On 20 minutes of recorded Binance BTCUSDT order flow it runs 5.4× faster than the `std::map` version, but that book never held more than 4,203 orders, so it fit in cache. Write-up: [From 21M to 65M ops/s](https://aayxshkumar.github.io/order-book-3x.html). Every number, with its evidence: [claims ledger](https://aayxshkumar.github.io/claims.html). Built with Claude Code; the [colophon](https://aayxshkumar.github.io/colophon.html#ai) says how.

<picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/aayxshkumar/lob-engine/main/docs/throughput-dark.svg"><img src="https://raw.githubusercontent.com/aayxshkumar/lob-engine/main/docs/throughput-light.svg" width="660" alt="Throughput, million ops/s, Apple M4, one thread. Synthetic mixed workload, median of 10 runs: std::map 20.9M, arrays + bitset 35.7M, id table 65.2M. 20 minutes of Binance BTCUSDT replayed, a small book that fits in cache: std::map 14.7M, id table 79.4M."></picture>

**Selected work**
- [`lob-engine`](https://github.com/aayxshkumar/lob-engine): matching engine, differential testing, benchmarks on synthetic and real Binance data (C++20)
- [`gemini-code`](https://github.com/aayxshkumar/gemini-code): my fork of Muruganandham18/gemini-code, a Gemini coding-agent CLI. I added Windows-first support, crash resume and multi-root workspaces (TypeScript)
- [`ai-hedge-fund`](https://github.com/aayxshkumar/ai-hedge-fund/tree/improve-decision-making): an extension of virattt/ai-hedge-fund for Indian markets, with Yahoo Finance data, NSE/BSE tickers and a Zerodha (Kite Connect) integration with paper and live trading modes (Python)

**Also:** Certified Kubernetes Administrator (CKA) · before this role, a DevOps internship at Airbus (AWS) and LLM evaluation pipelines at Turing.

[Portfolio](https://aayxshkumar.github.io) · [LinkedIn](https://www.linkedin.com/in/aayush-kumr) · aayushkumr25@gmail.com
