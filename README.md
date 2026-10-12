### LET ME COOK

I do security research and bug bounties, and I contribute fixes to open source projects. When I find a bug and the fix is clearer than the report, I send a PR.

Yes, most of my public repos are forks. That is on purpose: each one carries a branch of mine on its way upstream (or already merged). I fork to contribute, not to collect.

#### Building

[ARTEX](https://github.com/BaaRai/ARTEX): an AI autonomous penetration testing system. I build it and run it daily for my own research.

#### Merged upstream

[morluto/rea](https://github.com/morluto/rea), six merges in under a week:

- [#1130](https://github.com/morluto/rea/pull/1130): app analysis crashed whenever a JavaScript module imported itself.
- [#1285](https://github.com/morluto/rea/pull/1285): the Hopper verifier's interior navigation probe assumed the first instruction is longer than one byte.
- [#1374](https://github.com/morluto/rea/pull/1374): the Ghidra verifier skipped dense jump tables. Now proven on an optimized fixture.
- [#1382](https://github.com/morluto/rea/pull/1382): clang folds cross-branch tail calls into one basic block. The fixture now survives the optimizer.
- [#1447](https://github.com/morluto/rea/pull/1447): new HarmonyOS package analysis tool, hap/hsp/app-pack inventory.
- [#1929](https://github.com/morluto/rea/pull/1929): setup client support for the DSH agent harness.

[Niko1221/Strata](https://github.com/Niko1221/Strata): loop guard for periodic one-word loops, shipped in v0.1.42 ([commit](https://github.com/Niko1221/Strata/commit/253e09f1)).

#### Open PRs

On rea: [#1889](https://github.com/morluto/rea/pull/1889) (wasm module admission), [#1892](https://github.com/morluto/rea/pull/1892) (firmware extraction gap reporting), [#1898](https://github.com/morluto/rea/pull/1898) (recordless legacy MIPS32 in Ghidra), [#1922](https://github.com/morluto/rea/pull/1922) (32-bit ARM lane in Ghidra).

Elsewhere:

- [openclaw/openclaw #167161](https://github.com/openclaw/openclaw/pull/167161): zombie processes accumulated after Codex app-server transports closed on Linux.
- [NousResearch/hermes-agent #135110](https://github.com/NousResearch/hermes-agent/pull/135110): cron occurrences consumed by the gate now record a durable incident row.
- [bendlang/bend #1469](https://github.com/bendlang/bend/pull/1469): Process.run works on hosts without Bun.
- [Autumn-27/Norma #3](https://github.com/Autumn-27/Norma/pull/3): recover real input token usage when the API reports zeros in message_start.
- [codecrafters-io/build-your-own-x #2047](https://github.com/codecrafters-io/build-your-own-x/pull/2047): audited all 368 links in the README, replaced the 12 that are actually dead.
- [monid-ai/monid #106](https://github.com/monid-ai/monid/pull/106): keep an explicit null consolidate output instead of restoring the raw payload.
- [earendil-works/pi #10654](https://github.com/earendil-works/pi/issues/10654): mcp.json server url should expand env references like headers do. Fix is on my fork, waiting for a maintainer go-ahead before opening the PR (their gate).

#### Elsewhere

Three microservice fixes merged in 2025 on team repos, and assorted private tooling for recon and pentest automation.
