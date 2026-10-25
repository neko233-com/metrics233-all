# Delivery evidence

Updated: 2026-10-26. Source, local tests, packages, hosted CI, browser evidence and production deployment are separate acceptance layers.

## Current composition

| Module | Source | Published/runtime boundary |
| --- | --- | --- |
| metrics233-server | 17ddd844a2c6c64b2cf902e16619189dfc0dc6e1 | Documentation receipt over immutable runtime 6270a48/v0.2.31. Formal public release, complete tag CI, actual ZIP validation, anonymous downloads, native production rollout and production Edge are accepted. |
| metrics233-lib-go | 4f63688e023bce29b1e6b79c14733e246bc277b6 | Go SDK release 0.1.0; real game reporting remains active. |
| metrics-lib-rust | 3a58fff2901e001984b45791fb884d23e3d8f9b7 | Official crates.io metrics233 0.1.0 is available; this pin only updates its guidance. |
| metrics233-client-sdk-typescript | 152ee85e628cca8a3126cc61b2bb9593c062a1ba | GitHub v0.1.0 plus installable tgz; npm registry upload is separate. |
| metrics233-client-sdk-csharp | 95a93a7d1b19d1f5d14b555996d0afa7c37a1209 | GitHub v0.1.0 plus Metrics233.Client NuGet artifact; NuGet.org upload is separate. |
| metrics233-client-sdk-rust | 8c78e875f278e9d764733486367bb1afe260ee71 | Official crates.io 0.1.0 and GitHub v0.1.0 share identical immutable package bytes. Current pin records installation and real-server acceptance. |

## 0.2.31 public release, complete CI and production Edge accepted

Source/tag 6270a48a800eaf74f4ff8153baed159eff13d81c/v0.2.31 fixes current-snapshot expiry and overdue refresh
after a suspended tab. It retains GitHub Dark chrome, independent Grafana classic/gauge palettes, historical
curves, mounted cards/canvases, note/search drafts and explicit NIC selection. Red regressions reproduce both old
failures before the corrections. Five focused browser cases pass in 9.6s, 174 units/build pass and the complete
candidate browser suite passes 106 cases/three environment skips/7.5m without retries.

Two clean-source five-platform builds produce identical seven-file deliveries. ZIP/CRC/architecture/provenance
and Windows-native version checks pass; the actual Windows ZIP repeats all 106 cases/three skips without retries.
The actual Linux ZIP (in-container SHA/version verified) passes two formal confined runtime/browser rounds in
158.247s and a separate four-database/three real SQL-browser run in 210.734s; SQL browser itself takes 26.2s.
Its eight memory.current snapshots max at 134332416 bytes, without presenting that as a kernel peak.

Edge uses an independent loopback-only instance of the same Linux ZIP. With refresh Off, actual synthetic HTTP
body counters become unknown after the real 90-second deadline; open note/search drafts remain. New samples and
manual refresh restore nonzero rates. A multiline note saves and matches the combined note/SDK search. No captured
warnings/errors or browser-clock/response substitution; the unassociated host is correctly unknown. Owned temporary
pages, container, volume and verification image are cleaned; shared caches remain. Production data is untouched.
[Complete exact-tag workflow 40222966206](https://github.com/neko233-com/metrics233-server/actions/runs/40222966206)
passes: test 41m54s, complete Go vet/race 31m29s, 106 default browser cases/three environment skips/8.1m without
retries, two owned real-Tempo API/browser rounds and Docker 7m53s. Dedicated SQL and Tempo runs cover the real
environments skipped by the default suite. [v0.2.31](https://github.com/neko233-com/metrics233-server/releases/tag/v0.2.31)
was formally published at 2026-10-25 19:32:55 UTC; all seven anonymous official HTTPS downloads (215594380 bytes)
match the independently verified local artifacts.

The existing single private native pipeline deploys fixed source 6270a48 as 0.2.31 after private tests/vet,
backup/target preflight, 174 frontend units/build, complete Go tests, collector cross-builds and immutable
archive/download checks. Official account/ingest readiness and actual process/source/version/hash readback pass.
Private control-plane identities and credentials remain separate; native unit settings are not described as
the confined Docker settings.

Production Edge reloads the deployed release and observes seven real reporting identities. With refresh Off,
an actual wait past 90 seconds expires all 21 host CPU/memory/disk values and 14 service receive/send values to
unknown, with overdue footers and retained open note/search drafts. Manual refresh restores current values and
freshness. Release filtering returns two cards, LAN-IP search one and the Rust gateway category one. The gateway
retains three racing gauges and two real traffic curves; idle service bytes remain separate from active physical
NIC traffic. A temporary note is saved, found and reopened, then restored to its original empty value.
Fourteen unpaused rules show zero firing/pending and current evaluations; actual LAN CPU warning parameters are
30s evaluation/600s sustained trigger/300s recovery/3600s cooldown. The original business entry, empty search and
default 5s refresh are restored; final seven cards have complete numeric resources and no captured browser
warnings/errors. No clocks/responses are replaced, fake production samples injected, thresholds changed or
extra provider notifications sent for this check. GitHub Dark console chrome and Grafana classic/racing renderers
remain independent. The server roadmap stays 96%; this is not unlimited capacity or optional-technology parity.

## Accepted online behavior

The default embedded runtime additionally passes a ten-minute isolated sustained workload: 4000 series,
500 samples/s, 304000 ACKed observations and 600 queries from one reader concurrent with writes. Latest-value sum and total sample
count remain exact after restart. The actual verified Linux v0.2.30 binary in unchanged formal confinement records
87609344-byte cgroup peak, 5320 KiB complete active data before restart and no OOM/throttling. Write/query p95 are
17.534/13.223ms. This is a specific declared workload; image/cache/backups and arbitrary cardinality/compression
are not folded into these active-data figures. See the child sustained-profile contract.

Real Tempo 3.1.1 OTLP ingestion, TraceQL search, span hierarchy/duration/error state, missing trace and authenticated
HTTP/browser deep links pass locally; Edge inspects the same actual daemon data. The deterministic leading-zero
case also passes twice. The first cold-pull stderr/ID failure and cancelled test job remain. Full source 86f1081
passes all vet/race, 103 default browser cases/three skips (8.3m) and repeated Docker, but its old randomized
fixture fails on a valid leading-zero ID. That complete workflow remains failed. Final deterministic 15b917a passes
[focused hosted verification](https://github.com/neko233-com/metrics233-server/actions/runs/40219239682), including
two zero-retry actual Linux/browser rounds in 21.222s, negative cases and vet (job 2m38s).
[Combined b0c9045 full verification](https://github.com/neko233-com/metrics233-server/actions/runs/40220691425)
passes: test job 42m07s, complete vet/race 31m40s, 103 default browser cases/three environment skips/8.1m without
retries, repeated Docker 8m52s and two actual Tempo/browser rounds in 20.272s. The dedicated live step executes
the contract skipped by the unowned default suite. R2c closes; these are interoperability tests, not a production
Tempo installation or a new binary rollout.

The earlier production [v0.2.30](https://github.com/neko233-com/metrics233-server/releases/tag/v0.2.30) fixes source 17791c5.
GitHub Dark page/panel/navigation/control layers stay independent from Grafana classic lines and racing gauges.
Active-NIC defaults use fresh traffic and retain explicit choices; content-width instruments use three/two/one/one
columns at 1512/1100/768/390px. Edge verifies seven real instance cards, release/category/IP search, multiline-note
save/search/reopen/restoration, real per-NIC receive/send and independent service bytes. Same-scope card/canvas,
search draft and manual NIC remain mounted/selected through refresh; no overflow or console warnings/errors were
captured. Mobile normal-click/keyboard closing now uses a visible backdrop outside the 250px drawer.

The actual Windows ZIP passes 103 zero-retry browser cases with two external-SQL skips (7.4 min). The Linux ZIP
passes ten normal mobile-shell rounds (41.9 s) and two unchanged confined runtime/browser rounds (156.531 s).
Two five-platform builds are byte-identical; independent ZIP/source/architecture/binary checks and all seven
anonymous official downloads pass. [Full exact-tag CI](https://github.com/neko233-com/metrics233-server/actions/runs/40210846886)
is green: test 28m00s including full Go vet/race and hosted browser 103 passed/two SQL-environment skips (7.3 min,
no retries), Docker 10m50s. Native production passed its full worker, actual process/source/hash checks and official
account/token healthcheck. The docs-only pin does not imply recompiling the runtime; private deployment identities
remain separate. A new real SQL-browser run or native Darwin/Linux arm64 execution is not claimed. Roadmap remains 95%.

### Earlier 0.2.29 acceptance and retained failure

Production 0.2.29 fixes immutable source 352c4c5. Host automatic NIC choice uses fresh traffic and preserves the
first useful selection; manual idle/missing choices retain their exact history. Content-width instruments use
three/two/one columns without changing the GitHub Dark console or the independent Grafana/racing palettes.
The actual Windows ZIP passes 103 browser cases with zero retries and two external-SQL skips. The initial missing-Go
PATH attempt (16 fixture startup failures) is retained separately. Actual Linux ZIP runtime/browser passes twice
(159.852 seconds); independent five-platform builds produce identical seven-file sets. Edge on seven real instances
verifies search/categories/environments, Chinese note persistence/restoration, per-NIC rates, original card/canvas
retention and 1512/1100/768/390 containment. Full hosted race and Docker pass; the final Linux mobile-backdrop case
failed twice (102 passed/two skipped/one failed). Its immutable tag/draft remain; the 0.2.30 correction passes Windows
five/Linux ten zero-retry repetitions; its final publication/download closure is recorded above. Child contracts distinguish current Grafana workflows
from the historical October 12 audit. Weighted server roadmap remains 95%.

### Previous public release closure

Public release closure is accepted. [Final v0.2.28](https://github.com/neko233-com/metrics233-server/releases/tag/v0.2.28)
fixes ebfd82c and passes [full exact-tag CI](https://github.com/neko233-com/metrics233-server/actions/runs/40198818834).
Its two five-platform builds produce identical seven-file delivery sets; independent ZIP CRC, source/provenance,
architecture and binary checks pass. Every published file was anonymously downloaded over HTTPS and hash-matched.
Both README languages are packaged. Actual Windows ZIP browser validation passes 101 cases without retries,
with two external-SQL skips; all three SQL browser cases separately pass against real MySQL/PostgreSQL.
Actual Linux ZIP confined runtime/browser passes twice (152.120 s), and real database integration passes (207.759 s).
Native production 0.2.28 and Edge verify seven real instances, the completed GitHub Dark layers, search/category/
environment, note save/search/reopen/restoration and actual per-NIC traffic. Card/canvas identity and explicit NIC
choice survive refresh; 1512/768/390px layouts and console checks pass. The supported server roadmap is now 95%.
The preceding immutable v0.2.27 separately passed its full CI and anonymous downloads. The initial v0.2.26 Windows
candidate's 87 passes / 14 failures / 2 SQL skips, successful Docker job and explicitly cancelled test job remain
historical evidence; no failed tag was rewritten or described as green. Detailed identities and boundaries are in
the child ledger and private deployment receipts.

- Private 0.2.26 completed immutable native preparation, full Go tests, 169 frontend units/build, native account/token readiness, collector/archive/download checks and dependency audit with zero known advisories. Full source vet and six layout-browser cases passed separately. Exact-source runtime Docker/browser checks passed twice (204.782 s), including restart and offline restore with the original memory assertions; four real database/eight protocol fixture flows passed twice on the corrected transport source. Edge verified actual GitHub Dark tokens, all seven instances, formal filtering/IP search and the note persistence/restoration flow, plus real LAN/Linux NIC data and retained canvas/NIC selection across refresh. A reviewed existing-collector apply produced six real host panels without duplicate scraping or alerts; its versioned layout now has readable 200px instruments and full-width per-volume capacity. Desktop and 390px mobile renders passed, with mobile client/scroll width both 390px and no captured warnings/errors. Charts, racing gauges and threshold colors remain independent of console chrome. No game binaries, synthetic samples, high load or new Feishu messages were introduced for this unit. Detailed intermediate/final source attribution remains in the child status ledger and private deployment receipts.
- Private 0.2.24 passed the full immutable worker, 169 frontend units/build, native readiness, collector and archive/download checks, plus the patched dependency audit (zero known advisories). Deployment 439 succeeded and actual runtime health reports 0.2.24/database=ok. Edge verified seven real cards and explicit physical-host resources, category/environment/global ordering, Chinese multiline note save/search/reopen/restore, and separate service/NIC throughput with interface switching. LAN collector heartbeats expose 17 interfaces; the existing Linux exporter now exposes netdev. Card and canvas DOM identity, search drafts and chosen NIC survive same-scope refresh; 390px layout has no horizontal overflow. The GitHub Dark console palette stays independent from Grafana classic line and threshold-gauge rendering. The final concept/render comparison and intentional native-panel differences are documented in the child instance-directory contract. Producer aliases are pushed separately; this is not a claim of a new game binary rollout or gameplay login.
- Private 0.2.21 passed complete fixed-source worker tests/vet, 167 frontend units/build, native token/account readiness, cross-platform collector builds, archive and actual-download verification, then the exact production deployment. Edge verified the six actual reporting identities, the redesigned directory and physical-host/process/business layout, current CPU/memory/disk, decimal MB/GB, browser-local full timestamps/GMT clock, recent-hour trends and SQL multi-sort. Desktop 2514×1234 and 1586×992, plus mobile 390×844, passed the rendered flow and console checks. Concept-to-render fidelity and the explicit functional differences are documented in the child console-redesign contract.
- Private 0.2.17 cut over 16661384 real samples to embedded XOR/Zstd time series and local Badger/HNSW vectors with reopened exact float/count verification, including 40 normalized empty-label series. Independent control/identity/key files remained protected. Active native statistics initially occupied about 42 MB; the stopped legacy control file occupied 588 MB. Retained backups are separate from these active-storage figures.
- Private 0.2.19 completed the full fixed-source worker gates and exact target deployment. All six real game/gateway identities have explicit physical-host associations. Process CPU/RSS/uptime and the corresponding host CPU/memory/disk queries returned actual observations; five inherited business templates remained intact.
- Edge displayed the actual intranet instance resource gauges/capacity, last-hour curves and game process resources. The formal game SQL view sorted all 84 eligible rows before Top10; header primary sort, Shift-added secondary sort and the priority editor were exercised on the production page.
- Native-engine notification acceptance separately passed 24 transitions, one firing and one recovery provider ACK, second-cycle 1h cooldown suppression and owned-rule cleanup. The new readable signed card also passed a single explicit notification test with one HTTP 200 provider ACK. Temporary checks did not fabricate a production resource fault.
- Ingest-only credentials passed missing/wrong-token 401 and read/admin 403 boundaries. Account login, canonical source-IP policies and versioned 15-day retention remain independent controls.
- The failed 0.2.18 attempt stopped at an SSH handshake reset before any target mutation. It did not replace the healthy 0.2.17 service. Later 0.2.19 acceptance is recorded independently; no failed run is described as green.

## Client SDK evidence

- TypeScript: zero runtime dependencies, 10 local tests including a real native server, exact retry/partial ACK, finite bounds, redirect rejection, Retry-After and credential isolation. The official GitHub tgz was downloaded, SHA/provenance-checked, installed into a fresh cache/project, type-checked and successfully reported to an isolated real server.
- CSharp: netstandard2.0/net8.0/net10.0 build and NuGet pack, thread-safe cumulative counter/zero/ACK/retry/deadline tests and actual native-server ingestion/isolation. A fresh NuGet cache/project restored the package and reported successfully; the installed DLL hash matched the build. Official GitHub bytes matched that tested artifact. Unity/IL2CPP/device acceptance is not claimed.
- Rust: MSRV 1.88 tests and real-server correct/wrong-token checks; Clippy/doc/package checks. Both metrics233 0.1.0 and metrics233-client-sdk-rust 0.1.0 are officially published. A new Darwin arm64 project installed the alias through official cargo add, compiled and reported successfully; reopened embedded storage returned Counter 5 and Gauge 233, wrong/missing-token 401 and ingest-only management-read 403 passed. Official alias package SHA-256: 209401a867d0a0787e76eb36f6f481c96e24a43505743b45592ebf410b99eb2a. Windows fresh compilation hit OS error 1455 and is not counted as passing; the native consumer and Rust 1.88 tag CI are separate successful gates. See the child's docs/registry-v0.1.0.md for cache/source provenance.
- All three SDK tag workflows succeeded: [TypeScript](https://github.com/neko233-com/metrics233-client-sdk-typescript/actions/runs/39768659392), [CSharp](https://github.com/neko233-com/metrics233-client-sdk-csharp/actions/runs/39768665546), [Rust](https://github.com/neko233-com/metrics233-client-sdk-rust/actions/runs/39768672606). Hosted transport/package checks and local actual-server tests are distinct gates.

## Final follow-up gates

The current server pin adds authenticated Agent operation schemas for instance resources/host association/ranking, explicit stale-report labels and virtual-list scroll reset after sorting. Discovery/business tests and vet, 163 frontend units and production build passed. Its immutable 0.2.20 rollout passed all full-worker/readiness/archive gates and actual target deployment. Live discovery returned the four expected operations/roles; six instance resource associations and complete-set SQL sorting passed again (132 eligible rows at final readback). Aggregate composition ac55170e876781f561feb7c966f0cede0581b067 was pushed and independently cloned with all six submodules. Every pinned SHA matched, the new checkout was clean, and its six-module public-source/history gate passed. This subsequent receipt update changes documentation only.

The public-source checker now covers all six canonical children, CSharp/ESM source and lock files. Exact earlier two/three-module compositions are accepted only in history. Private deployment identities, addresses and receipts stay in the separate private repository. Overall server roadmap weighting remains 95%; no new game-account Login/Ready/Ping or nonzero player-lifecycle acceptance is claimed.

Earlier evidence is retained in [the historical ledger](history-20261022-before-native-cutover.md) and the server's own docs/status.md.
