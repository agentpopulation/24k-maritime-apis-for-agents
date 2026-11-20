## Maritime API endpoints, snapshot 15 Nov 2026

- 24,827 endpoints passed a keyless data call, tested 10–15 Nov 2026 (IST)
- 3,457 services · 73 country codes · 14,548 keyless JSON rows

### Download

- `Maritime_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz`: the full list, 24,827 rows, 1.2 MB gzipped (7.4 MB as CSV), SHA-256 `7f065f7df693543e8b5533d6d0141028a30405162b9be23b36fef1c6b3b9b4f4`
- `SHA256SUMS.txt`: the checksum of that file

Check the download in the folder that holds both files:

```bash
sha256sum -c SHA256SUMS.txt          # Linux
shasum -a 256 -c SHA256SUMS.txt      # macOS
certutil -hashfile Maritime_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz SHA256   # Windows: compare with SHA256SUMS.txt
```

Then `gunzip Maritime_API_Endpoints_AgentPopulation_Snapshot_2026-11-15.csv.gz` and pass the CSV path to the examples or to `node tools/test-endpoints.mjs`. The repository itself holds a 1,000-row sample and the services list.

### What's in it for you

- 🤖 Agent tools: 5,035 · Wrap the port-call URL as a get_port_calls tool: pass a UN/LOCODE port code (FIHEL), return the ships with arrival and departure times; add a timeout.
- 📱 App features: 5,056 · Show ports, ferry piers, moorings and harbour limits on a coastal map card, with the layer name and the date it passed.
- 🧠 Grounding and data pipelines: 1,390 · Load freight, port-call and ship-count tables on a schedule into your own store, so answers about port traffic cite a dated table.
- 🧪 Evals and testing: 24,827 · Run your maritime tool against a fixed set of URLs across formats; check that port code, ship name, time or feature geometry parse, and keep last_tested as the baseline for your own re-tests.

### Changes

- First release
- Left out: 236 ArcGIS Survey123 layers (they can hold people's form answers).
- Left out: 1 layer marked editable in the title (it can hold entries that people added).
- Left out: 23 ArcGIS layers that keep a form's default service name (they can hold people's form answers).
- Left out: 118 ArcGIS class or coursework layers (lab, assignment, exam, quiz, lesson, exercise, tutorial and final-project layers, copies of class layers, layers named for a person or a person's home, and layers whose name ends in a person's name or holds a student number).
- Left out: 16 ArcGIS layers that hold reports, comments, submissions or form responses sent in by the public.
- Overlap: 468 of these URLs are also in 190k-weather-apis-for-agents.
- Overlap: 1,949 of these URLs are also in 270k-transit-apis-for-agents.
- Overlap: 3,104 of these URLs are also in 270k-water-apis-for-agents.
- Overlap: 66 of these URLs are also in 130k-finance-economy-apis-for-agents.
- Overlap: 18 of these URLs are also in 130k-india-apis-for-agents.
- Overlap: 2,484 of these URLs are also in 86k-oceans-apis-for-agents.
- Overlap: 123 of these URLs are also in 20k-air-quality-apis-for-agents.
- Overlap: 14,548 of these URLs are also in 2.5m-agent-ready-apis.
- Overlap: 4 of these URLs are also in 6.5k-wildfire-apis-for-agents.
- Overlap: 1,307 of these URLs are also in 24k-traffic-apis-for-agents.
- Overlap: 60 of these URLs are also in 12k-parking-apis-for-agents.
- Overlap: 115 of these URLs are also in 10k-earthquake-apis-for-agents.
- Overlap: 27 of these URLs are also in 5.2k-volcano-tsunami-apis-for-agents.

On the date in last_tested (IST), one GET to the URL, sent with no key, returned HTTP 2xx and a non-empty data body. HTML pages and empty results did not pass. The format column records what came back. This is a test result for that date, not a promise that the URL answers today. Licences, terms, rate limits, accuracy and freshness were not reviewed. Endpoints are URLs, not separate APIs; many share one service. This pack was tested 10–15 Nov 2026; snapshot 15 Nov 2026.

For the latest tested endpoints, search agentpopulation.com/apis. This pack is a snapshot from 15 Nov 2026.

Credit: Maritime API endpoints by AgentPopulation (https://agentpopulation.com), CC BY 4.0, snapshot 15 Nov 2026.

Compiled by [AgentPopulation](https://agentpopulation.com) with [AP Desk](https://github.com/agentpopulation/apdesk) · corrections: [@agentpopulation](https://x.com/agentpopulation) on X
