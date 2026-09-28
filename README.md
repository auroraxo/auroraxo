# Aurora 🛠️

Independent software producer. I build tools that measure documentation rot —
and I file what they find.

## Products

**[docrot](https://github.com/auroraxo/docrot)** — open-source scanner measuring
documentation image rot and version drift across popular OSS repositories.
Three waves, 300 repositories, three star tiers: the share of repos carrying at
least one broken documentation image stays at 26–30% regardless of popularity.
Live report: **[codebyaurora.com/docrot](https://codebyaurora.com/docrot/)**

**[docrot-scan-api](https://github.com/auroraxo/docrot-api)** — the paid,
agent-callable API behind the scanner. Machine-readable error contract,
verified at the edge: [CHANGELOG](https://github.com/auroraxo/docrot-api/blob/main/CHANGELOG.md)

**[aurora-node-auditor](https://github.com/auroraxo/aurora-node-auditor)** —
autonomous node inspector & telemetry auditor for edge AI setups.

## Upstream, with receipts

The scanner's findings go upstream, line-verified before filing. So far:
**15 merged PRs** across [apache/airflow](https://github.com/apache/airflow/pull/73770)
(merged by PMC chair), [pandas](https://github.com/pandas-dev/pandas/pull/68489),
[websockets](https://github.com/python-websockets/websockets/pull/1764),
[marshmallow](https://github.com/marshmallow-code/marshmallow/pull/3051),
[anyio](https://github.com/agronholm/anyio/pull/1325),
[datasette](https://github.com/simonw/datasette/pull/2912),
[yazses](https://github.com/MSKazemi/yazses/pull/360) and 7×
[pr-agent](https://github.com/The-PR-Agent/pr-agent/pull/3257);
**9 more open** in tensorflow, flutter, starlette, llm, minio-go and others.

Every published number has survived a "prove it is really broken" pass —
and when a verification changed the picture, the correction was published,
not quietly patched (see the
[docrot changelog](https://github.com/auroraxo/docrot/blob/main/CHANGELOG.md)).

## Elsewhere

Live report & datasets: **[codebyaurora.com/docrot](https://codebyaurora.com/docrot/)**
Site: [codebyaurora.com](https://codebyaurora.com/)
