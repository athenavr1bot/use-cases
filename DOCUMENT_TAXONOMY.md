# Document Taxonomy & Classification System

**Version:** 1.0  
**Date:** 2026-02-08  
**Purpose:** Define how documents are coded, sorted, and managed

---

## Document Coding System

### Format: `[PILLAR]-[TYPE]-[CATEGORY]-[NAME]`

**Example:** `01-FIXOPS-PROCESS-Service-Absorption-Analysis`

---

## Pillar Codes

| Code | Pillar | Color |
|------|--------|-------|
| **01** | Fixed Operations | 🔵 Blue |
| **02** | Variable Operations | 🟢 Green |
| **03** | Marketing Architecture | 🟣 Purple |
| **04** | API Configurations | 🟠 Orange |
| **05** | CRM Automation | 🔴 Red |
| **06** | Graphics Design | 🟡 Yellow |
| **07** | Attribution & Tracking | ⚫ Black |

---

## Document Types

| Code | Type | Description |
|------|------|-------------|
| **PROCESS** | Process Document | Step-by-step workflows |
| **WORKFLOW** | Workflow Definition | Automation sequences |
| **TEMPLATE** | Template | Reusable document templates |
| **CASE** | Case Study | Client success stories |
| **PLAYBOOK** | Playbook | Comprehensive action guides |
| **REFERENCE** | Reference Material | Background information |
| **STANDARD** | Standards Doc | Best practices & benchmarks |
| **TRAINING** | Training Material | Educational content |

---

## Category Codes

### Fixed Ops (01)

| Category | Code | Examples |
|----------|------|----------|
| Service | SVC | CSI, workflows, advisor training |
| Parts | PRT | Inventory, pricing, wholesale |
| Technician | TEC | Skills, certification, productivity |
| Absorption | ABS | Service absorption calculations |
| Scheduling | SCH | Appointment systems, capacity |
| Warranty | WAR | Claims, recall management |

---

### Variable Ops (02)

| Category | Code | Examples |
|----------|------|----------|
| Sales | SLS | Team structure, quotas, compensation |
| F&I | FNI | Finance, insurance, extended warranties |
| Inventory | INV | Stocking, pricing, turns |
| Internet | INT | Digital leads, BDC, online sales |
| Desking | DES | Finance structuring, deal sheets |
| Closing | CLS | Negotiation, objection handling |

---

### Marketing (03)

| Category | Code | Examples |
|----------|------|----------|
| Strategy | STR | Campaign planning, budgets |
| Content | CNT | Blogs, social, video |
| Channels | CHN | Paid, organic, email |
| Brand | BRD | Guidelines, identity, messaging |
| Campaigns | CMP | Specific marketing initiatives |
| Attribution | ATT | Tracking, ROI, measurement |

---

### API Config (04)

| Category | Code | Examples |
|----------|------|----------|
| Integration | INT | System connections |
| Data | DAT | ETL, migration, sync |
| Authentication | AUTH | OAuth, API keys |
| Webhooks | WHK | Event triggers |
| Documentation | DOC | API specs, endpoints |
| Security | SEC | Encryption, access control |

---

### CRM Automation (05)

| Category | Code | Examples |
|----------|------|----------|
| Lead Management | LDM | Scoring, routing, nurturing |
| Follow-up | FUP | Sequences, cadences, templates |
| Segmentation | SEG | Customer lists, targeting |
| Automation | AUT | Triggers, rules, workflows |
| Reporting | RPT | Dashboards, metrics, analytics |
| Integration | INT | CRM connections, data sync |

---

### Graphics (06)

| Category | Code | Examples |
|----------|------|----------|
| Brand Identity | BID | Logos, colors, typography |
| Digital | DIG | Web, social, email graphics |
| Print | PRT | Brochures, signage, materials |
| Video | VID | Commercials, testimonials |
| Guidelines | GLI | Brand usage, standards |
| Assets | AST | Image libraries, icon sets |

---

### Attribution (07)

| Category | Code | Examples |
|----------|------|----------|
| Tracking | TRK | Pixels, UTM, call tracking |
| Analytics | ANA | Reporting, dashboards, insights |
| Attribution | ATT | Models, touchpoints, channels |
| Performance | PRF | KPIs, benchmarks, ROI |
| Channels | CHN | Google, Facebook, dealer websites |
| Compliance | CMP | Privacy, data usage |

---

## Folder Structure

```
use-cases/
├── 01_fixed-ops/
│   ├── processes/
│   ├── workflows/
│   ├── templates/
│   ├── case-studies/
│   └── playbooks/
├── 02_variable-ops/
│   ├── processes/
│   ├── workflows/
│   ├── templates/
│   ├── case-studies/
│   └── playbooks/
├── 03_marketing/
│   ├── processes/
│   ├── workflows/
│   ├── templates/
│   ├── case-studies/
│   └── playbooks/
├── 04_api-config/
│   ├── processes/
│   ├── workflows/
│   ├── templates/
│   ├── case-studies/
│   └── playbooks/
├── 05_crm-automation/
│   ├── processes/
│   ├── workflows/
│   ├── templates/
│   ├── case-studies/
│   └── playbooks/
├── 06_graphics/
│   ├── processes/
│   ├── workflows/
│   ├── templates/
│   ├── case-studies/
│   └── playbooks/
└── 07_attribution/
    ├── processes/
    ├── workflows/
    ├── templates/
    ├── case-studies/
    └── playbooks/
```

---

## Document Naming Convention

```
[PILLAR]-[TYPE]-[CATEGORY]-[NAME]-[VERSION].[md/json/html]
```

**Examples:**

```
01-FIXOPS-PROCESS-SVC-Appointment-Scheduling-v1.md
02-VAROPS-WORKFLOW-FNI-Product-Upsell-Sequence-v1.md
03-MKTG-ATT-Model-MultiTouch-v1.md
05-CRM-AUT-LDM-Scoring-Rules-v1.json
07-ATTR-ANA-Dashboard-Setup-v1.md
```

---

## Metadata Header (Required)

Every document must include:

```yaml
---
title: Document Title
pillar: 01-Fixed Operations
type: PROCESS | WORKFLOW | TEMPLATE | CASE | PLAYBOOK | REFERENCE | STANDARD | TRAINING
category: SVC | PRT | SLS | FNI | etc.
author: Your Name
created: 2026-02-08
updated: 2026-02-08
version: 1.0
tags: [tag1, tag2, tag3]
related: [linked documents]
---
```

---

## GitHub Sync Instructions

### Initial Setup

```bash
cd /root/.openclaw/workspace/use-cases
git init
git remote add origin https://github.com/athenavr1bot/use-cases.git
git add .
git commit -m "Initial use case taxonomy and structure"
git push -u origin main
```

### Adding New Documents

```bash
# Create document with proper naming
touch 01-FIXOPS-PROCESS-SVC-New-Process-v1.md

# Add to GitHub
git add .
git commit -m "Add: [Document Name]"
git push origin main
```

---

## Agent Mapping

| Agent | Pillar | Focus | Document Types |
|-------|--------|-------|----------------|
| Agent-01 | Fixed Ops | Service/Parts optimization | Processes, playbooks |
| Agent-02 | Variable Ops | Sales/F&I performance | Workflows, case studies |
| Agent-03 | Marketing | Strategy/content/channels | Campaigns, content |
| Agent-04 | API Tech | Integrations/data | API docs, configs |
| Agent-05 | CRM | Lead management/automation | Sequences, templates |
| Agent-06 | Creative | Graphics/brand assets | Design specs, templates |
| Agent-07 | Attribution | Tracking/analytics/ROI | Dashboards, reports |

---

## Quick Reference

### Finding Documents

| Need | Search Pattern |
|------|----------------|
| All fixed ops | `01-FIXOPS-*` |
| All CRM workflows | `05-CRM-AUT-*` |
| All templates | `*-TEMPLATE-*` |
| All case studies | `*-CASE-*` |
| Service processes | `01-FIXOPS-PROCESS-SVC-*` |
| Marketing attribution | `03-MKTG-ATT-*` |

---

*This document controls how all knowledge is organized. Update when adding new categories or pillars.*
