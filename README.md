### Hi, I'm Aayush 👋

I'm a software engineer at **Airbus**, where I build C++/Qt software for an iPad app that 40,000 pilots use every day. I care about the parts of software that have to be fast, predictable and correct.

**Currently building:** [`lob-engine`](https://github.com/aayxshkumar/lob-engine), a C++20 limit order book and matching engine. It's tested against a naive reference book on every operation. Two measured steps took it from 21.2M to 67.5M operations per second: flat price-level arrays with a bitset, then an open-addressing table in place of `std::unordered_map`. On 20 minutes of recorded Binance BTCUSDT order flow it runs 5.2× faster than the `std::map` version. Write-up: [From 21M to 68M ops/s](https://aayxshkumar.github.io/order-book-3x.html). Every number, with its evidence: [claims ledger](https://aayxshkumar.github.io/claims.html).

<picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/aayxshkumar/lob-engine/main/docs/throughput-dark.svg"><img src="https://raw.githubusercontent.com/aayxshkumar/lob-engine/main/docs/throughput-light.svg" width="660" alt="Throughput, million ops/s, Apple M4, one thread. Synthetic mixed workload: std::map 21.2M, arrays + bitset 34.3M, id table 67.5M. 20 minutes of Binance BTCUSDT replayed: std::map 15.9M, id table 81.9M."></picture>

**Selected work**
- [`lob-engine`](https://github.com/aayxshkumar/lob-engine): matching engine, differential testing, benchmarks on synthetic and real Binance data (C++20)
- [`gemini-code`](https://github.com/aayxshkumar/gemini-code): my fork of Muruganandham18/gemini-code, a Gemini coding-agent CLI. I added Windows-first support, crash resume and multi-root workspaces (TypeScript)
- [`ai-hedge-fund`](https://github.com/aayxshkumar/ai-hedge-fund): an extension of virattt/ai-hedge-fund for Indian markets, with NSE/BSE data and Zerodha integration (Python)

**Also:** Certified Kubernetes Administrator (CKA) · previously DevOps at Airbus (AWS) and LLM evaluation infrastructure at Turing.

[Portfolio](https://aayxshkumar.github.io) · [LinkedIn](https://linkedin.com/in/aayush-kumr) · aayushkumr25@gmail.com
