Defensive security analyst in Australia. My day job is mostly Splunk,
Sysmon and incident write-ups. The write-ups are the part nobody enjoys, so I've
been building tools that do the boring half for me.

I work around air-gapped networks, so everything here runs fully offline. No
cloud, no telemetry, nothing phones home.

## [IntelScribe](https://github.com/xGhst0/intelscribe)

Desktop report writer for incident response and pentest reports, written in Rust
(Tauri for the shell, Typst for rendering). You enter the facts once, then the
hosts, detections, IoCs and timeline feed every section: exec summary, IoC
tables, kill-chain timeline, mitigations, CVSS scoring. The full MITRE ATT&CK
matrix and the ACSC ISM are compiled into the binary, so citing a control quotes
the real text with the cable unplugged. It's all deterministic too, the same
input always produces the same report.

<img src="assets/intelscribe-app.png" width="100%" alt="IntelScribe desktop app">

It draws the attack path and ATT&CK coverage straight from the timeline:

<p>
<img src="assets/intelscribe-attack-path.png" width="49%" alt="attack path">
<img src="assets/intelscribe-attack-matrix.png" width="49%" alt="ATT&CK coverage matrix">
</p>

Report covers are generated procedurally, 18 palettes by 6 art styles. Stock
photography in an incident report never felt right:

<p>
<img src="assets/intelscribe-cover-1.png" width="32%" alt="Harbour Teal cover">
<img src="assets/intelscribe-cover-2.png" width="32%" alt="Midnight Slate cover">
<img src="assets/intelscribe-cover-3.png" width="32%" alt="Crimson Vector cover">
</p>

## [SKYHAWK](https://github.com/xGhst0/skyhawk)

Case management for analyst teams on closed networks. Plain Node.js, zero
dependencies, state in a single JSON file. Analysts log findings with evidence,
leads review, a manager signs. The technical report regenerates as findings
change; the formal report gets frozen and signed when the case closes. There's
a bundler that packs the app plus the Node runtime into one tarball for boxes
that have never seen the internet.

<img src="assets/skyhawk-dashboard.png" width="100%" alt="SKYHAWK dashboard">

<p>
<img src="assets/skyhawk-case.png" width="49%" alt="case workspace">
<img src="assets/skyhawk-report-technical.png" width="49%" alt="live technical report">
</p>

## Day to day

Splunk, Elastic, Sysmon, Volatility, KAPE. Frameworks-wise: MITRE ATT&CK, the
ACSC ISM and Essential Eight, CVSS when I have to.

Reach me at benjamin.sokimi@gmail.com
