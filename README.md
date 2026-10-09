### LET ME COOK

I do security research and bug bounties, and I contribute fixes to open source projects. When I find a bug and the fix is clearer than the report, I send a PR.

Yes, most of my public repos are forks. That is on purpose: each one carries a branch of mine on its way upstream (or already merged). I fork to contribute, not to collect.

#### Merged upstream

- [morluto/rea #1130](https://github.com/morluto/rea/pull/1130): app analysis crashed whenever a JavaScript module imported itself, self edges are forbidden by the graph schema. Skipped at composition and disclosed in limitations.
- [morluto/rea #1285](https://github.com/morluto/rea/pull/1285): the real-Hopper verifier's interior navigation probe assumed the first instruction is longer than one byte. Now anchored to the first multi-byte instruction.

#### Open PRs

- [commaai/connect #822](https://github.com/commaai/connect/pull/822) and [#827](https://github.com/commaai/connect/pull/827): hiring challenge bounties. Video-driven playback state, and url handling as the single source of truth for navigation.
- [openclaw/openclaw #167161](https://github.com/openclaw/openclaw/pull/167161): zombie processes accumulated after Codex app-server transports closed on Linux. Added identity-scoped reaping.
- [NousResearch/hermes-agent #135110](https://github.com/NousResearch/hermes-agent/pull/135110): cron occurrences consumed by the gate left no trace. Now they record a durable incident row.
- [codecrafters-io/build-your-own-x #2047](https://github.com/codecrafters-io/build-your-own-x/pull/2047): audited all 368 links in the README, replaced the 12 that are actually dead.
- [monid-ai/monid #106](https://github.com/monid-ai/monid/pull/106): keep an explicit null consolidate output instead of restoring the raw payload.
- [earendil-works/pi #10654](https://github.com/earendil-works/pi/issues/10654): mcp.json server url should expand env references like headers do. Fix is on my fork, waiting for a maintainer go-ahead before opening the PR (their gate).

#### Elsewhere

Three microservice fixes merged in 2025 on team repos, and assorted private tooling for recon and pentest automation.
