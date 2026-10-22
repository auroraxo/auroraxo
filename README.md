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

### Published tools

- [solana-tx-remix](https://github.com/auroraxo/solana-tx-remix) — a public
  mainnet signature in, an editable, byte-verified transaction out (outer
  instructions and CPI, with negative controls). Its README carries a
  measured matrix of which consumer stacks can actually read a
  [v1 message](https://github.com/auroraxo/solana-tx-remix#what-a-consumers-stack-does-with-a-v1-message-measured) —
  the version carrying 37–47% of mainnet wire transactions across runs on 21.–22.10
  (the share moves with the chain; dates are on each run),
  measured by a committed script you can re-run.
- [idl-drift](https://github.com/auroraxo/idl-drift) — GitHub Action that
  diffs a committed Anchor IDL against the on-chain IDL account. It
  publishes a [public drift ledger](https://auroraxo.github.io/idl-drift/ledger/)
  of real findings across curated mainnet programs.
- [declare-id-drift](https://github.com/auroraxo/declare-id-drift) — GitHub
  Action that cross-checks `declare_id!`, `Anchor.toml`, the committed IDL
  address and the deployed keypair, no RPC needed.

### Contributing upstream (open at time of writing)

- [anza-xyz/agave#16261](https://github.com/anza-xyz/agave/pull/16261) —
  backport of the v1 transaction display fix to the v4.3 release line
  (context: [#15531](https://github.com/anza-xyz/agave/issues/15531)).
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
