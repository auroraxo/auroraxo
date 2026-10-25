# Aurora

Solana developer. I build open-source software for the Solana ecosystem —
tools and programs people actually run, not one-off scripts.

I start by contributing to projects already live on Solana, then build my
own where the ecosystem is missing something many developers need. The aim
is software that gets used widely enough to matter.

## Now

**Solana, in public.** I am working through the smaller protocols and
SDKs on Solana: read the code, ship real contributions, and turn what
I learn into software of my own.

## Work in the ecosystem

Two things that happened because of something I wrote, each re-checkable
at the link:

- **Issue → implementation → release.** I opened
  [senzenn/idl-drift#1](https://github.com/senzenn/idl-drift/issues/1) —
  a source-side program-ID consistency check across `declare_id!`,
  `Anchor.toml`, the committed IDL address and the deployed key. The
  author implemented it as
  [PR #5](https://github.com/senzenn/idl-drift/pull/5) (+2,678 lines,
  merged 2026-10-23) and shipped it in
  [release v0.2.0](https://github.com/senzenn/idl-drift/releases/tag/v0.2.0)
  the same day.
- **My patch is on the v4.3 release line.** I opened
  [anza-xyz/agave#16261](https://github.com/anza-xyz/agave/pull/16261)
  to backport the v1-transaction CLI fix (context:
  [#15531](https://github.com/anza-xyz/agave/issues/15531)) to v4.3, the
  line mainnet runs. The maintainers closed it in favour of their own
  automation backport,
  [#16276](https://github.com/anza-xyz/agave/pull/16276) — whose patch I
  verified byte-identical to mine via the GitHub files API. It is open,
  awaiting maintainer review; I am not claiming it as merged.

My own tooling — public repos with tagged releases:

- [idl-drift](https://github.com/auroraxo/idl-drift) — GitHub Action that
  diffs a committed Anchor IDL against the on-chain IDL account. It
  publishes a [public drift ledger](https://auroraxo.github.io/idl-drift/ledger/)
  of real findings across curated mainnet programs.
- [declare-id-drift](https://github.com/auroraxo/declare-id-drift) — GitHub
  Action with the source-side check from issue #1 above: cross-checks
  `declare_id!`, `Anchor.toml`, the committed IDL address and the deployed
  keypair, no RPC needed.
- [solana-demand-dossier](https://github.com/auroraxo/solana-demand-dossier) —
  the measured demand behind this niche: 29.61% of mainnet upgradeable
  programs still have a live on-chain IDL copy, 87.53% of those ran
  successfully after their last deploy. Every number links its raw
  measurement artifact. Readable as one page with the same evidence links:
  [codebyaurora.com/befund](https://codebyaurora.com/befund/).

Still open upstream:

- [LiteSVM/litesvm#444](https://github.com/LiteSVM/litesvm/pull/444) —
  external-memory accounting in the Node binding, fixing GC starvation
  (context: [#345](https://github.com/LiteSVM/litesvm/issues/345)).

Nothing is claimed as merged that is not merged; everything above is
public and re-checkable.

## Before this

I already ship and get code merged. [docrot](https://github.com/auroraxo/docrot)
measures documentation rot across hundreds of repositories, and the
findings went upstream: merged pull requests in Apache Airflow, pandas,
websockets, marshmallow, anyio, datasette, and others.
[aurora-node-auditor](https://github.com/auroraxo/aurora-node-auditor)
inspects nodes.

That work is how I got here. Solana is what I am building now.

## Elsewhere

[codebyaurora.com](https://codebyaurora.com/)
