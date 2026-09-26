<div align="center">

# FatNarwhal

**Markets, quant tools, and the code behind them.**

[fatnarwhal.com](https://fatnarwhal.com) · [Tusk](https://fatnarwhal.com/tusk) · [Gallery](https://fatnarwhal.com/gallery)

</div>

---

FatNarwhal is a markets and finance site built around two things most
finance content doesn't have: real data, and real code you can run
yourself. This org is the code half — public, MIT-licensed, and meant to
be forked.

## What's here

**[Tusk](https://fatnarwhal.com/tusk)** is FatNarwhal's in-browser IDE:
write a quant tool, run it against real market data, fork someone else's,
publish your own, no install required. The repos in this org are the
GitHub side of that same idea — clone one as a starter, or (where noted)
run the identical tool live on the site.

| Repo | Language | Live on Tusk? |
|---|---|---|
| [`montecarlo-python`](https://github.com/fatnarwhal/montecarlo-python) | Python | **Yes** — pick a ticker and run it |
| [`spsc-tickdecoder-c`](https://github.com/fatnarwhal/spsc-tickdecoder-c) | C | Clone-and-run starter |
| [`spsc-tickdecoder-cpp`](https://github.com/fatnarwhal/spsc-tickdecoder-cpp) | C++ | Clone-and-run starter |
| [`spsc-tickdecoder-rust`](https://github.com/fatnarwhal/spsc-tickdecoder-rust) | Rust | Clone-and-run starter |
| [`tickrules-ocaml`](https://github.com/fatnarwhal/tickrules-ocaml) | OCaml | Clone-and-run starter |

The three `spsc-tickdecoder-*` repos implement the same lock-free
single-producer/single-consumer ring buffer and ITCH-style tick decoder,
once per systems language, from a shared spec — so a benchmark run in one
is directly comparable to the same run in another. `montecarlo-python` and
`tickrules-ocaml` are companion projects that play to what Python and
OCaml are actually good at, rather than joining a speed contest.

## Using these repos

Every repo here is a **GitHub template repo** — hit "Use this template"
on any of them to start your own project from it, no forking required.
Each one is self-contained: its own README, tests, and a CI workflow that
builds and tests on every push.

## License

Everything in this org is MIT-licensed. Take it, modify it, ship it.

## About FatNarwhal

FatNarwhal is built and run by [Michael Incorvaia](https://github.com/michaelincorvaia).
Questions, ideas, or found a bug — open an issue on the relevant repo.
