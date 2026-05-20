<div align="center">

<img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=20&pause=1000&color=00D4FF&center=true&vCenter=true&width=700&lines=Analytics+Engineer;6+years+in+software.+Now+building+BI+systems.;From+back-end+events+to+Power+BI+decisions.;I+turn+messy+tracking+into+trusted+metrics." alt="Typing SVG" />

</div>

---

Six years building software. Now focused on Business Intelligence, analytics engineering, and data quality for SaaS products. The transition was natural — I always cared more about what the data was saying than the screen displaying it.

I follow the data from source to decision: backend events, GA4 exports, tracking pipelines, BigQuery models, scheduled SQL transforms, Power BI semantic layers, and stakeholder-ready diagnostics.

**Currently:** building and maintaining the NoPing BI platform — raw backend/GA4 sources, `noping_web` analytical tables, dependency-ordered scheduled queries, a versioned Power BI semantic model, dashboards, funnel analysis, revenue/client cohorts, marketing performance, software usage, and CRM automation datasets.

---

## Wins that matter

| Impact | What I did |
|---|---|
| **BI platform ownership** | Maintain the NoPing analytics stack from raw backend/GA4 sources to BigQuery `tbl_*` tables, scheduled SQL, Power BI TMDL semantic model, and report pages |
| **19 active analytical tables** | Organized the warehouse into domain tables for trials, sales, revenue, clients/churn, marketing, software performance, access type, page views, and devices |
| **6-page Power BI report** | Built and documented a version-controlled `.pbip` report with Revenue, Trials, Sales, Clients, Software, and Marketing pages, backed by TMDL, JSON visuals, DAX measures, relationships, parameters, and bookmarks |
| **Data warehouse cleanup** | Migrated analytics tables from `noping_analytics` to `noping_web`, removed 20 orphaned `tbl_*` tables, deleted an unused latency schedule/table, and documented destructive BigQuery actions in changelog |
| **CRM automation datasets** | Built incremental email-segmentation tables for expired trials and monthly-plan users: played, logged but did not play, never opened the app, and did not renew |
| **Visit → Register root cause** | Proved a reported funnel collapse was a BI artifact, not a product regression — GA4 trial tracking stopped, the visits denominator moved to backend tracking, and real trials stayed stable at ~800-900/day |
| **GA4 visibility gap** | Cross-checked GA4 with backend events and found that traffic in GCC/Asia was still arriving while GA4 was being filtered or blocked; recommended backend as the source of truth |
| **215x backend/GA4 gap** | Found China was almost invisible in GA4 (3 GA4 visits vs 645 backend visits/week), revealing real traffic hidden from dashboards |
| **China conversion diagnosis** | Investigated low CN registration conversion with BigQuery, VPN tests, backend review, and temporal analysis; identified Cloudflare Turnstile friction plus residential bot/proxy traffic as the main drivers |
| **Tracking data quality** | Mapped backend visit dedup (`md5(ip+userAgent)`, 24h TTL), validated it empirically, and documented where bots, race conditions, prefetch, and missing user/session IDs still distort metrics |
| **Timezone bug found** | Discovered `trial_page_visits.inserted_at` was saved as BRT but interpreted as UTC by BigQuery, affecting temporal analysis and monitoring |
| **33x** | Found a bug silently inflating core business metrics by 33x |
| **83 GB → incremental** | Rewrote full-scan queries to incremental loads |
| **19h → 1h19min** | Reduced BigQuery slot time by ~93% |
| **Dependency-ordered ETL** | Scheduled BigQuery refreshes across business domains with explicit dependencies, including revenue before clients/LTV and software overview before cross-usage |
| **61-month cohort retention** | Built cohort curves tracking user retention from month 0 to month 60, segmented by acquisition plan and top game |
| **End-to-end attribution** | Last-touch model with 30-day window covering CAC, LTV, ROAS, CPT, CPC, CTR, CPM — from Google Ads spend to subscription revenue |
| **Full ELT from desktop to cloud** | Designed the entire pipeline: Electron app (TypeScript) → sandboxed IPC → main process enrichment → secured Cloud Run endpoint (Go) → BigQuery streaming insert. Events enriched in real-time with geolocation, OS fingerprinting, and hardware telemetry |
| **Per-session hardware telemetry** | Each gaming session records RTT, packet loss, bridge routing, CPU/GPU usage, CPU/GPU temps, and RAM — correlated with ping improvement and ISP data |
| **12-phase user funnel** | Instrumented the full user journey across 9 BigQuery tables: boot → auth → connection → 8 feature screens, with session stitching via hardware fingerprint |

---

## Stack

<div align="center">

`Data` &nbsp; ![BigQuery](https://img.shields.io/badge/BigQuery-4285F4?style=flat-square&logo=google-cloud&logoColor=white) ![Dataform](https://img.shields.io/badge/Dataform-4285F4?style=flat-square&logo=google-cloud&logoColor=white) ![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat-square&logo=powerbi&logoColor=black) ![GA4](https://img.shields.io/badge/GA4-E37400?style=flat-square&logo=google-analytics&logoColor=white) ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)

`Cloud` &nbsp; ![GCP](https://img.shields.io/badge/GCP-4285F4?style=flat-square&logo=google-cloud&logoColor=white) ![Cloud Run](https://img.shields.io/badge/Cloud%20Run-4285F4?style=flat-square&logo=google-cloud&logoColor=white)

`Dev` &nbsp; ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white) ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white) ![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black) ![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=next.js&logoColor=white) ![Electron](https://img.shields.io/badge/Electron-47848F?style=flat-square&logo=electron&logoColor=white) ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

</div>

---

<div align="center">

[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/fisaarpelesjo/)
[![Kaggle](https://img.shields.io/badge/-Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)](https://www.kaggle.com/fisaar)
[![Email](https://img.shields.io/badge/-Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:filipesalesaraujo@gmail.com)

</div>
