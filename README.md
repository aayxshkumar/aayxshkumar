I'm Aayush Kumar, a software developer at Airbus in Bengaluru. For the past year I've written C++ and Qt/QML for an iPad app that 40,000 pilots use every day. I graduated from NIT Kurukshetra in 2025.

### [lob-engine](https://github.com/aayxshkumar/lob-engine)

A limit order book and matching engine in C++20. Every operation is checked against a deliberately naive reference book, and the tests caught all 16 bugs planted to test them. Two measured changes took a mixed synthetic workload from 20.9M to 65.2M ops/s on one thread: flat price-level arrays with a bitset, then an open-addressing id table in place of `std::unordered_map`.

<picture><source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/aayxshkumar/lob-engine/main/docs/throughput-dark.svg"><img src="https://raw.githubusercontent.com/aayxshkumar/lob-engine/main/docs/throughput-light.svg" width="660" alt="Throughput, million ops/s, Apple M4, one thread. Synthetic mixed workload, median of 10 runs: std::map 20.9M, arrays + bitset 35.7M, id table 65.2M. 20 minutes of Binance BTCUSDT replayed, a small book that fits in cache: std::map 14.7M, id table 79.4M."></picture>

On 20 minutes of recorded Binance BTCUSDT order flow it runs 5.4× faster than the `std::map` version, but that book never held more than 4,203 orders, so it fit in cache.

The [write-up](https://aayxshkumar.github.io/order-book-3x.html) walks through each change, including the one that made it slower first, and the [claims ledger](https://aayxshkumar.github.io/claims.html) links every number to its evidence. I build it with Claude Code; the [colophon](https://aayxshkumar.github.io/colophon.html#ai) says how.

### Other work

- [`gemini-code`](https://github.com/aayxshkumar/gemini-code): my fork of [Muruganandham18/gemini-code](https://github.com/Muruganandham18/gemini-code), a CLI that drives Gemini through browser automation. My releases (v0.8 to v0.13) added Windows-first support, crash resume and multi-root workspaces. TypeScript.
- [`clickhouse-flatfile-tool`](https://github.com/aayxshkumar/clickhouse-flatfile-tool): moves data both ways between ClickHouse and CSV or TSV files, with schema mapping and a preview before each transfer. React and Node; a take-home for Zeotap.
- [`healthtrack`](https://github.com/aayxshkumar/healthtrack): offline-first patient records that run PostgreSQL in the browser through PGlite. React and TypeScript; a take-home for Medblocks.
- [`ai-hedge-fund`](https://github.com/aayxshkumar/ai-hedge-fund): extends [virattt/ai-hedge-fund](https://github.com/virattt/ai-hedge-fund) to Indian markets, with Yahoo Finance data, NSE/BSE tickers and a Zerodha Kite Connect integration with paper and live trading modes. Python.

Most of my other public repos are take-home assignments and earlier learning projects.

Before this role I was a DevOps intern at Airbus, where the team adopted my AWS migration proof of concept. Before that I worked on LLM evaluation pipelines at Turing.

I'm looking for quant developer, low-latency C++ and SRE roles.

[aayxshkumar.github.io](https://aayxshkumar.github.io) · [LinkedIn](https://www.linkedin.com/in/aayxshkumar) · aayushkumr25@gmail.com
