# Aurora

Hi — I build open-source software for the Solana ecosystem. Small, focused
tools that run locally and answer one concrete question, plus contributions
upstream where I find real gaps.

Everything here is public and re-checkable: tagged releases, open issues,
and measurements that link their raw data.

## Building now

- **[sememe](https://github.com/auroraxo/sememe)** — a local meaning layer
  for Solana. `sememe pull <program>` fetches and verifies a program
  interface, then instructions, accounts, and events decode offline.
  RFC stage; v0.4 releases are tagged.
- **[reeflog](https://github.com/auroraxo/reeflog)** — a durable local
  mailbox for Solana events. A cursor-addressed append-only journal with
  gap-fill, reorg sealing, and webhook fan-out, so a consumer resumes
  without gaps after a crash, disconnect, or reorg. Running live against
  mainnet-beta.
- **[signerd](https://github.com/auroraxo/signerd)** — a scoped signing
  daemon for Solana keys: the ssh-agent pattern. The key lives once in a
  local daemon; processes hold grants, never secrets. Early v0 prototype —
  not a security-reviewed wallet, and not for real funds.

## Next

- **sememe:** catalog import and a local daemon on top of the verified
  pull/decode core.
- **reeflog:** longer mainnet runs, a second transport (Yellowstone gRPC),
  more real consumers.
- **signerd:** a professional security review before anything real flows
  through it.

## Upstream

Three things that happened because of something I wrote, each re-checkable
at the link:

- **[senzenn/idl-drift#1](https://github.com/senzenn/idl-drift/issues/1)** —
  I proposed a source-side program-ID consistency check across
  `declare_id!`, `Anchor.toml`, the committed IDL address, and the deployed
  key. The author implemented it as
  [PR #5](https://github.com/senzenn/idl-drift/pull/5) (merged 2026-10-23)
  and shipped it in
  [release v0.2.0](https://github.com/senzenn/idl-drift/releases/tag/v0.2.0).
- **[LiteSVM/litesvm#444](https://github.com/LiteSVM/litesvm/pull/444)** —
  external-memory accounting in the Node binding, fixing GC starvation
  (context: [#345](https://github.com/LiteSVM/litesvm/issues/345)). Open,
  awaiting maintainer review.
- **[anza-xyz/agave#16261](https://github.com/anza-xyz/agave/pull/16261)** —
  a v4.3 backport of the v1-transaction CLI fix. The maintainers closed it
  in favour of their own automation backport
  ([#16276](https://github.com/anza-xyz/agave/pull/16276)); both are now
  closed without merging, and the underlying
  [issue #15531](https://github.com/anza-xyz/agave/issues/15531) stays
  open. Nothing here is claimed as merged that is not merged.

## Before this

- [idl-drift](https://github.com/auroraxo/idl-drift) and
  [declare-id-drift](https://github.com/auroraxo/declare-id-drift) — GitHub
  Actions that check a committed Anchor IDL against the deployed program:
  on-chain and in source. idl-drift publishes a
  [public drift ledger](https://auroraxo.github.io/idl-drift/ledger/) of
  real findings across curated mainnet programs.
- [solana-demand-dossier](https://github.com/auroraxo/solana-demand-dossier) —
  the measured demand behind that niche; every number links its raw
  measurement artifact, also readable as one page at
  [codebyaurora.com/solana-findings](https://codebyaurora.com/solana-findings/).
- [docrot](https://github.com/auroraxo/docrot) — measures documentation
  image rot across hundreds of repositories; the findings went upstream as
  merged pull requests in Apache Airflow, pandas, websockets, marshmallow,
  anyio, datasette, and others.

## Elsewhere

- [codebyaurora.com](https://codebyaurora.com/)
- Issues and questions on any repo are welcome — they get answered here.
