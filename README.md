<p align="center"><img src="assets/banner.svg" alt="Ops Health Dashboard" width="100%"></p>

<p align="center">
<img src="https://img.shields.io/badge/stack-Apps_Script_·_HTML_Service_·_Sheets-5B3A3A?style=flat-square">
<img src="https://img.shields.io/badge/data-fictional-FBE3EC?style=flat-square">
<a href="https://sider.ai/agents/web-creator/share/695ea81100a621619985fdfb"><img src="https://img.shields.io/badge/Portfolio-Nae_Kitakado-F4B4CD?style=flat-square"></a>
</p>

<p align="center"><a href="https://naekitakadoportfolio.github.io/ops-health-dashboard/"><img src="https://img.shields.io/badge/%E2%96%B6%20Try%20the%20live%20demo-5B3A3A?style=for-the-badge" alt="Live demo"></a></p>

# Ops Health Dashboard

An operations monitor for work items that sync between two systems. It flags stuck, desynced and flapping cards, explains why, and fixes them. Click a card, simulate incidents, and try Full Auto-Fix.

> **Portfolio rebuild.** This is a from-scratch recreation of a production system I designed and run, rebuilt with **fictional data** and no client names, code or branding. The live demo runs entirely in the browser.

## The problem
Ad cards moved between an internal project tool and an external ad platform through several automations. When one misfired, cards got stuck, subtasks desynced or statuses flapped. Coordinators found out days later and had to escalate every time.

## Impact in production
Gave coordinators one dashboard that detects stuck, desynced and flapping cards, explains the root cause and fixes them in one click. Several recurring incidents (race conditions, silent duplicate-send guards, overwrites) were traced and fixed at the source.

## What it demonstrates
| Capability | How |
|---|---|
| Anomaly detection | Stuck-time thresholds, desync scanner, flapping detector |
| Root-cause investigator | Side-by-side internal vs platform state |
| Guided recovery | Validate → Preview → Apply, plus Full Auto-Fix |
| Health scorecard | Single operations health KPI |
| UX | Responsive glassmorphic UI with light/dark theme in production |

## Production architecture
Apps Script web app (HTML Service) · time-driven watchdog trigger · Sheets as daily sync log · REST calls to both systems · Slack alerts on stuck cards

## Try it
Open the **[live demo](https://naekitakadoportfolio.github.io/ops-health-dashboard/)** or run `index.html` locally. No install needed.

---
<p align="center"><sub>Built by <b>Nae Kitakado</b>, AI Automation Consultant · <a href="https://www.linkedin.com/in/nae-k-203194265">LinkedIn</a> · <a href="https://sider.ai/agents/web-creator/share/695ea81100a621619985fdfb">Portfolio</a> · open to retainer &amp; part-time consulting</sub></p>
