### Hi, I'm Aayush 👋

I'm a software engineer at **Airbus**, where I build C++/Qt software for an iPad app that 40,000 pilots use every day. I care about the parts of software that have to be fast, predictable and correct.

**Currently building:** [`lob-engine`](https://github.com/aayxshkumar/lob-engine), a C++20 limit order book and matching engine. It's tested against a naive reference book on every operation, and its latency is benchmarked as p50 / p99 / p99.9. Two measured steps took it from 21.2M to 67.5M operations per second: flat price-level arrays with a bitset, then an open-addressing table in place of `std::unordered_map`. On 20 minutes of recorded Binance BTCUSDT order flow it runs 5.2× faster than the `std::map` version. Write-up: [From 21M to 68M ops/s](https://aayxshkumar.github.io/order-book-3x.html).

**Selected work**
- [`lob-engine`](https://github.com/aayxshkumar/lob-engine): matching engine, differential testing, benchmarks on synthetic and real Binance data (C++20)
- [`gemini-code`](https://github.com/aayxshkumar/gemini-code): my fork of Muruganandham18/gemini-code, a Gemini coding-agent CLI. I added Windows-first support, crash resume and multi-root workspaces (TypeScript)
- [`ai-hedge-fund`](https://github.com/aayxshkumar/ai-hedge-fund): an extension of virattt/ai-hedge-fund for Indian markets, with NSE/BSE data and Zerodha integration (Python)

**Also:** Certified Kubernetes Administrator (CKA) · previously DevOps at Airbus (AWS) and LLM evaluation infrastructure at Turing.

[Portfolio](https://aayxshkumar.github.io) · [LinkedIn](https://linkedin.com/in/aayush-kumr) · aayushkumr25@gmail.com
