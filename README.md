<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>GitHub README Preview — Pratish Ninawe</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&family=JetBrains+Mono:wght@400;500&display=swap');

  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

  body {
    background: #0d1117;
    color: #e6edf3;
    font-family: 'Inter', -apple-system, sans-serif;
    font-size: 14px;
    line-height: 1.7;
    padding: 32px 16px 64px;
  }

  .readme {
    max-width: 780px;
    margin: 0 auto;
    background: #0d1117;
  }

  /* ── NAME BLOCK ── */
  .name-block {
    border-bottom: 1px solid #21262d;
    padding-bottom: 24px;
    margin-bottom: 28px;
  }

  .name {
    font-size: 28px;
    font-weight: 700;
    color: #f0f6fc;
    letter-spacing: -0.5px;
    margin-bottom: 4px;
    font-family: 'JetBrains Mono', monospace;
  }

  .tagline {
    font-size: 14px;
    color: #58a6ff;
    font-weight: 500;
    margin-bottom: 6px;
  }

  .motto {
    font-size: 13px;
    color: #8b949e;
    font-style: italic;
    margin-bottom: 14px;
  }

  .contact-bar {
    display: flex;
    flex-wrap: wrap;
    gap: 6px;
    align-items: center;
    font-size: 13px;
  }

  .contact-bar a {
    color: #58a6ff;
    text-decoration: none;
    padding: 3px 10px;
    border: 1px solid #30363d;
    border-radius: 20px;
    transition: border-color .15s, background .15s;
  }

  .contact-bar a:hover { border-color: #58a6ff; background: #161b22; }
  .contact-bar .sep { color: #30363d; }

  /* ── SECTION ── */
  h2 {
    font-size: 14px;
    font-weight: 600;
    color: #f0f6fc;
    text-transform: uppercase;
    letter-spacing: .08em;
    margin: 32px 0 14px;
    padding-bottom: 6px;
    border-bottom: 1px solid #21262d;
    font-family: 'JetBrains Mono', monospace;
  }

  /* ── JOB BLOCK ── */
  .job { margin-bottom: 22px; }

  .job-title {
    font-size: 14px;
    font-weight: 600;
    color: #f0f6fc;
    margin-bottom: 2px;
  }

  .job-title a { color: #58a6ff; text-decoration: none; }

  .job-period {
    font-size: 12px;
    color: #8b949e;
    font-family: 'JetBrains Mono', monospace;
    margin-bottom: 8px;
  }

  .job ul { padding-left: 0; list-style: none; }

  .job li {
    position: relative;
    padding-left: 18px;
    margin-bottom: 6px;
    font-size: 13px;
    color: #c9d1d9;
    line-height: 1.65;
  }

  .job li::before {
    content: '▸';
    position: absolute;
    left: 0;
    color: #58a6ff;
    font-size: 11px;
    top: 2px;
  }

  .job li b { color: #f0f6fc; font-weight: 600; }
  .job li .num { color: #79c0ff; font-weight: 600; font-family: 'JetBrains Mono', monospace; }

  /* ── TABLE ── */
  table { width: 100%; border-collapse: collapse; margin-bottom: 8px; font-size: 13px; }
  th {
    text-align: left;
    padding: 8px 12px;
    font-size: 11px;
    font-weight: 600;
    text-transform: uppercase;
    letter-spacing: .06em;
    color: #8b949e;
    border-bottom: 1px solid #21262d;
    font-family: 'JetBrains Mono', monospace;
  }
  td { padding: 9px 12px; border-bottom: 1px solid #161b22; color: #c9d1d9; vertical-align: top; }
  tr:last-child td { border-bottom: none; }
  td:first-child {
    font-family: 'JetBrains Mono', monospace;
    font-size: 12px;
    color: #58a6ff;
    white-space: nowrap;
    width: 220px;
  }
  tr:hover td { background: #161b22; }

  /* ── CODE BLOCK ── */
  .code-block {
    background: #161b22;
    border: 1px solid #21262d;
    border-radius: 8px;
    padding: 16px 20px;
    font-family: 'JetBrains Mono', monospace;
    font-size: 12px;
    line-height: 1.8;
    color: #c9d1d9;
    overflow-x: auto;
    margin-bottom: 4px;
  }

  .code-block .label { color: #58a6ff; font-weight: 500; }
  .code-block .val { color: #a5d6ff; }
  .code-block .comment { color: #8b949e; }

  /* ── CERT BLOCK ── */
  .cert {
    display: flex;
    align-items: center;
    gap: 10px;
    padding: 8px 12px;
    background: #161b22;
    border: 1px solid #21262d;
    border-radius: 8px;
    margin-bottom: 8px;
    font-size: 13px;
    color: #c9d1d9;
  }
  .cert-badge {
    background: #1f6feb;
    color: white;
    font-size: 10px;
    font-weight: 600;
    padding: 2px 8px;
    border-radius: 10px;
    white-space: nowrap;
    font-family: 'JetBrains Mono', monospace;
  }
  .cert-badge.wip { background: #388bfd33; color: #79c0ff; border: 1px solid #1f6feb44; }

  /* ── BUILDING ── */
  .building-item {
    display: flex;
    align-items: flex-start;
    gap: 8px;
    padding: 6px 0;
    font-size: 13px;
    color: #c9d1d9;
    border-bottom: 1px solid #161b22;
  }
  .building-item:last-child { border-bottom: none; }
  .building-item .dot { color: #58a6ff; margin-top: 1px; flex-shrink: 0; font-size: 10px; }

  /* ── FOOTER NOTE ── */
  .footer-note {
    margin-top: 32px;
    padding: 14px 18px;
    background: #161b22;
    border: 1px solid #21262d;
    border-left: 3px solid #58a6ff;
    border-radius: 4px;
    font-size: 12px;
    color: #8b949e;
    font-style: italic;
    line-height: 1.6;
  }

  .tip {
    margin-top: 6px;
    font-size: 12px;
    color: #8b949e;
    line-height: 1.6;
  }
  .tip b { color: #c9d1d9; }

  .divider {
    height: 1px;
    background: linear-gradient(90deg, #58a6ff22, #58a6ff88, #58a6ff22);
    margin: 28px 0;
  }
</style>
</head>
<body>
<div class="readme">

  <!-- NAME BLOCK -->
  <div class="name-block">
    <div class="name">PRATISH NINAWE</div>
    <div class="tagline">Backend Engineer · Azure Integration · .NET C# · Python · Fintech Systems</div>
    <div class="motto">If the data isn't moving reliably, redesign the pipeline.</div>
    <div class="contact-bar">
      <a href="#">📄 Résumé</a>
      <a href="https://www.linkedin.com/in/pratish-ninawe-6199b2220/" target="_blank">💼 LinkedIn</a>
      <a href="https://leetcode.com/pratish10/" target="_blank">🧩 LeetCode</a>
      <a href="mailto:pratish@email.com">✉ Email</a>
      <span style="font-size:12px;color:#8b949e;margin-left:4px">📍 Pune, India</span>
    </div>
  </div>

  <!-- WHAT I'M DOING NOW -->
  <h2>What I'm doing now</h2>

  <div class="job">
    <div class="job-title">Full Stack Engineer → Backend & Azure Integration · Qwalton Private Limited</div>
    <div class="job-period">Sept 2025 — Present</div>
    <ul>
      <li>Maintaining a <b>live AI-powered trading platform</b> integrating <span class="num">4 brokers</span>, serving <span class="num">80–100 daily active users</span> with sub-100ms latency SLAs across real-money financial workflows.</li>
      <li>Architected a full backend rebuild from Node.js → <b>.NET Core (C#) Clean Architecture</b> — MongoDB indexing, one-to-many relational restructure, async patterns, inbuilt caching, and <b>multi-threaded order execution</b> supporting <span class="num">500+ concurrent users</span> — delivering <span class="num">10× throughput improvement</span>, API response <span class="num">10s → 300ms</span>.</li>
      <li>Designed complete auth system from scratch — access + refresh token architecture, RBAC, broker-level session isolation.</li>
      <li>Cut trading UI page load <span class="num">10s → 1s</span> — React render optimisation, Redux normalisation, TypeScript API batching, broker market data caching.</li>
    </ul>
  </div>

  <div class="job">
    <div class="job-title">Azure Integration Engineer · <span style="color:#58a6ff">ByBar — Netherlands Fashion Brand</span> <span style="color:#8b949e;font-weight:400;font-size:12px">(client project via Qwalton)</span></div>
    <div class="job-period">2024 — 2025 · Logic Apps · Service Bus · Blob Storage · XSLT · CDM · Bicep · Azure DevOps</div>
    <ul>
      <li>Designed an <b>end-to-end Azure integration pipeline</b> for a live Netherlands fashion brand — <span class="num">10–20 million product records per sync</span>: recurrence-triggered → <b>XSLT transformation</b> → <b>Canonical Data Model</b> → Azure Blob Storage → Azure Service Bus → downstream system — latency <span class="num">under 4 seconds</span>.</li>
      <li>Entire infrastructure deployed as code via <b>Azure Bicep</b> + <b>Azure DevOps Pipelines</b> — repeatable across Logic Apps · APIM · Event Grid · Service Bus.</li>
    </ul>
  </div>

  <div class="job">
    <div class="job-title">Software Engineer · Celstream Technologies</div>
    <div class="job-period">Nov 2023 — Sept 2025 · React · Node.js · Python · WebSockets · Go.js</div>
    <ul>
      <li>Proposed and delivered a <b>complete UI architecture overhaul</b> — redesigned a broken nested-data interface; built a <b>Go.js canvas node-flipping feature</b> in JavaScript — recognised company-wide.</li>
      <li>Reduced frontend bundle <span class="num">2.4MB → 1.8MB</span>, improved responsiveness <span class="num">40%</span> with React + WebSockets.</li>
      <li>Mentored <span class="num">3 junior engineers</span> to production readiness in <span class="num">4 weeks</span>.</li>
    </ul>
  </div>

  <div class="divider"></div>

  <!-- RECENT WORK -->
  <h2>Recent / active work</h2>
  <table>
    <tr>
      <th>Repo</th>
      <th>What it is</th>
    </tr>
    <tr>
      <td>myalgoai</td>
      <td>Live multi-broker trading platform — real-time order execution, WebSocket data feeds, .NET C# backend serving 80–100 daily users</td>
    </tr>
    <tr>
      <td>data-monitor-dashboard</td>
      <td>Real-time streaming dashboard for distributed service metrics — 90% backend latency reduction through API redesign + PostgreSQL</td>
    </tr>
    <tr>
      <td>qr-dine</td>
      <td>Multi-tenant SaaS for restaurant management — React + Next.js + Node.js, JWT auth, RBAC, high-concurrency API handling</td>
    </tr>
    <tr>
      <td>rsvp.kim (OSS contrib)</td>
      <td>Card/email customisation, step validation, mobile previews shipped to Team Shiksha's production event creation flow</td>
    </tr>
  </table>

  <div class="divider"></div>

  <!-- CURRENTLY BUILDING -->
  <h2>Currently building toward</h2>
  <div class="building-item"><span class="dot">▸</span><span><b>AI-integrated backends on Azure</b> — RAG pipelines, Azure OpenAI, vector search with pgvector + LangChain (Python)</span></div>
  <div class="building-item"><span class="dot">▸</span><span><b>AI-200 certification</b> — Microsoft Azure AI Developer Associate · target: late 2026</span></div>
  <div class="building-item"><span class="dot">▸</span><span><b>AZ-400</b> — Azure DevOps Engineer Expert · target: early 2027</span></div>
  <div class="building-item"><span class="dot">▸</span><span><b>System Design depth</b> — Designing Data-Intensive Applications · ByteByteGo · 2 practice problems/week</span></div>
  <div class="building-item"><span class="dot">▸</span><span><b>DSA</b> — LeetCode 1 medium/day · target: 150 mediums by mid-2027</span></div>

  <div class="divider"></div>

  <!-- STACK -->
  <h2>Stack I actually ship</h2>
  <div class="code-block">
<span class="label">Backend:     </span><span class="val">.NET Core (C#) · ASP.NET Core · Python (FastAPI · Flask) · Node.js (Express) · Go</span>
<span class="label">Azure:       </span><span class="val">Logic Apps · Service Bus · Blob Storage · APIM · Event Grid · Container Apps</span>
<span class="val">             Bicep (IaC) · Azure DevOps Pipelines · AZ-900 Certified</span>
<span class="label">Frontend:    </span><span class="val">React · Next.js · TypeScript · Redux · WebSockets · Go.js canvas</span>
<span class="label">Data:        </span><span class="val">PostgreSQL · MongoDB (indexing · relational restructure) · MySQL · Redis</span>
<span class="label">DevOps:      </span><span class="val">Docker · GitHub Actions · Azure DevOps Pipelines · CI/CD</span>
<span class="label">Architecture:</span><span class="val">Clean Architecture · CQRS · event-driven pipelines · XSLT transformation</span>
<span class="val">             Canonical Data Model · multi-tenant SaaS · JWT + RBAC · multi-threaded execution</span>
<span class="label">AI / WIP:    </span><span class="val">Azure OpenAI · RAG pipelines · LangChain · pgvector <span class="comment">← actively building</span></span>
<span class="label">Languages:   </span><span class="val">C# · Python · TypeScript · JavaScript · Go · SQL</span>
  </div>

  <div class="divider"></div>

  <!-- CERTIFICATIONS -->
  <h2>Certifications</h2>
  <div class="cert">
    <span class="cert-badge">AZ-900</span>
    <span><b>Microsoft Certified: Azure Fundamentals</b> — May 2026</span>
  </div>
  <div class="cert">
    <span class="cert-badge wip">AI-200 · IN PROGRESS</span>
    <span><b>Microsoft Azure AI Developer Associate</b> — Target: late 2026</span>
  </div>

  <div class="divider"></div>

  <!-- HOW TO READ -->
  <h2>How to read this profile</h2>
  <div class="tip">Most of the older repos here are learning projects and coursework from when I was starting out. The work I'd actually point at is the trading platform at Qwalton and the ByBar Netherlands Azure integration project.</div>
  <br>
  <div class="tip"><b>→ Start at the Résumé</b> for the full story with numbers.</div>
  <div class="tip"><b>→ Reach out on LinkedIn</b> — I respond to interesting engineering conversations.</div>

  <div class="footer-note">
    Currently targeting Senior Backend · Azure Integration · AI Engineering roles — open to GCC, product companies, and international opportunities (NL · SG · CA · DE).
  </div>

</div>
</body>
</html>
