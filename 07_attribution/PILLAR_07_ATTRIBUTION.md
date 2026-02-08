# Pillar 07: Attribution & Tracking Master Document

**Pillar Code:** 07-ATTR  
**Focus:** ROI Measurement, Channel Performance, Analytics  
**Agent:** Agent-07 (to be created)  
**Last Updated:** 2026-02-08

---

## Overview

Attribution & Tracking provides complete visibility into marketing performance, enabling data-driven budget allocation and proving marketing ROI across all channels and campaigns.

---

## Core Use Cases

### UC-01: Multi-Touch Attribution Model
**Category:** PROCESS | ATT | MTA  
**Priority:** CRITICAL

**Objective:** Understand which touchpoints drive conversions

**Attribution Models:**

```
┌─────────────────────────────────────────────────────────┐
│                 ATTRIBUTION MODELS                         │
├─────────────────────────────────────────────────────────┤
│                                                         │
│  FIRST TOUCH (100% to first)                            │
│  Best for: Brand awareness focus                        │
│  Pros: Simple, clear                                    │
│  Cons: Ignores nurturing                                │
│                                                         │
│  LAST TOUCH (100% to last)                              │
│  Best for: Direct response focus                        │
│  Pros: Clear ROI at conversion                          │
│  Cons: Undervalues awareness                            │
│                                                         │
│  LINEAR (equal split)                                   │
│  Best for: Balanced view                               │
│  Pros: All touches valued                               │
│  Cons: No differentiation                               │
│                                                         │
│  TIME DECAY (more recent touches)                       │
│  Best for: Consideration-focused                        │
│  Pros: Values nurturing                                 │
│  Cons: Complex calculation                              │
│                                                         │
│  POSITION BASED (40/40/20)                             │
│  Best for: Complex funnels                             │
│  Pros: Balances first/last                              │
│  Cons: Arbitrary percentages                           │
│                                                         │
│  DATA-DRIVEN (algorithmic)                              │
│  Best for: Mature marketing                            │
│  Pros: Evidence-based                                  │
│  Cons: Requires volume + tools                          │
│                                                         │
└─────────────────────────────────────────────────────────┘
```

**Related Documents:**
- `07-ATTR-PROCESS-ATT-Models-v1.md`
- `07-ATTR-REFERENCE-ATT-Comparison-v1.md`

---

### UC-02: UTM & Tracking Infrastructure
**Category:** PROCESS | TRK | UTM  
**Priority:** CRITICAL

**Objective:** Consistent tracking across all campaigns

**UTM Standard:**
```
UTM SCHEMA:
https://domain.com/path? 
  utm_source=[google|facebook|newsletter]
  utm_medium=[cpc|email|social]
  utm_campaign=[spring_sale_2026]
  utm_content=[video_variant_a]
  utm_term=[toyota+camry]

REQUIRED: source, medium, campaign
RECOMMENDED: term, content
```

**Tagging Workflow:**
```
1. Campaign creation
   └── Define UTM parameters

2. Asset generation
   └── Apply UTM to all links

3. Verification
   └── Test all links in QA

4. Documentation
   └── Log all UTMs in tracking sheet

5. Monitoring
   └── Verify data in analytics
```

**Related Documents:**
- `07-ATTR-PROCESS-TRK-UTM-v1.md`
- `07-ATTR-TEMPLATE-UTM-Sheet-v1.xlsx`

---

### UC-03: Call Tracking & Attribution
**Category:** PROCESS | TRK | CALL  
**Priority:** HIGH

**Objective:** Track phone call sources

**Setup:**
```
CALL TRACKING NUMBERS
├── Default number (all calls)
├── Source-specific numbers (Google, Facebook, etc.)
├── Campaign-specific (Spring Sale, etc.)
└── Duration: Minimum 90 days

DISPLAY
├── Dynamic number insertion (website)
├── Vanity numbers (optional)
└── Ring-to-tracking number

DATA CAPTURE
├── Call duration
├── Call recording (with consent)
├── Call outcome (connected, voicemail)
└── Source attribution
```

**Related Documents:**
- `07-ATTR-PROCESS-TRK-Calls-v1.md`

---

### UC-04: Marketing ROI Dashboard
**Category:** REFERENCE | ANA | DSH  
**Priority:** CRITICAL

**Objective:** Centralized view of marketing performance

**Dashboard Components:**
```
┌─────────────────────────────────────────────────────────┐
│              MARKETING ATTRIBUTION DASHBOARD                │
├─────────────────────────────────────────────────────────┤
│                                                         │
│  SPEND & PERFORMANCE                                    │
│  ├── Total spend by channel                            │
│  ├── Cost per lead (CPL)                              │
│  ├── Cost per acquisition (CPA)                        │
│  ├── ROAS by channel                                   │
│  └── Budget vs actual                                  │
│                                                         │
│  LEAD FLOW                                             │
│  ├── Leads by source                                   │
│  ├── Lead-to-appointment rate                         │
│  ├── Appointment-to-sale rate                         │
│  └── Time to first contact                            │
│                                                         │
│  CHANNEL PERFORMANCE                                   │
│  ├── Google Ads (search, display, YouTube)             │
│  ├── Facebook/Instagram                               │
│  ├── SEO/organic                                      │
│  ├── Email                                             │
│  └── Offline (print, radio)                            │
│                                                         │
│  ATTRIBUTION RESULTS                                   │
│  ├── Touchpoints per conversion                        │
│  ├── Assisted conversions                              │
│  ├── Revenue by channel                               │
│  └── Winning combinations                              │
│                                                         │
└─────────────────────────────────────────────────────────┘
```

**Related Documents:**
- `07-ATTR-REFERENCE-ANA-Dashboard-v1.md`

---

### UC-05: Conversion Tracking Setup
**Category:** PROCESS | TRK | CVT  
**Priority:** CRITICAL

**Objective:** Track all conversion actions

**Conversion Events:**
```
WEBSITE CONVERSIONS
├── Form submissions (lead, parts, service)
├── Phone clicks (call tracking)
├── Text message clicks
├── Chat initiations
├── Video completions
├── Directions requests
└── Vehicle detail page views

OFFLINE CONVERSIONS
├── Phone calls (tracked separately)
├── In-store visits
├── Test drives booked
├── Vehicle purchases (matched back)
└── Service appointments booked

MICRO-CONVERSIONS
├── Video starts
├── Photo gallery views
├── Compare vehicle views
├── Trade-in value requests
└── Credit application starts
```

**Tracking Implementation:**
```
TRACKING TOOLS
├── Google Analytics 4
├── Google Ads conversion tracking
├── Facebook Pixel
├── LinkedIn Insight Tag
├── Call tracking platform
└── Heat mapping (Hotjar)

VERIFICATION
├── Test conversions in QA
├── Google Tag Assistant
├── Facebook Pixel Helper
└── Regular data audits
```

**Related Documents:**
- `07-ATTR-PROCESS-TRK-Conversions-v1.md`

---

## Key Performance Indicators

| KPI | Definition | Target | Top Performer |
|-----|------------|--------|---------------|
| CAC | Cost to acquire customer | <$500 | <$300 |
| ROAS | Revenue / Ad spend | 3:1 minimum | 5:1 |
| CPL | Cost per lead | <$50 | <$30 |
| CPA | Cost per appointment | <$75 | <$50 |
| Lead-to-Sale | % leads that buy | 8%+ | 15%+ |
| Attribution Rate | % leads tracked | 95%+ | 100% |
| Data Freshness | Time to insights | <24 hours | Real-time |

---

## Tracking Infrastructure Map

```
┌─────────────────────────────────────────────────────────┐
│              TRACKING INFRASTRUCTURE                       │
├─────────────────────────────────────────────────────────┤
│                                                         │
│  TRACKING TOOLS                                          │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐   │
│  │  GA4       │  │  Google Ads │  │  FB Pixel  │   │
│  └──────┬──────┘  └──────┬──────┘  └──────┬──────┘   │
│         │                │                │          │
│         └────────────────┼────────────────┘          │
│                          ▼                           │
│                  ┌─────────────┐                    │
│                  │  CDP/       │                    │
│                  │  Data Layer  │                    │
│                  └──────┬──────┘                    │
│                         │                            │
│         ┌───────────────┼───────────────┐            │
│         ▼               ▼               ▼            │
│   ┌───────────┐  ┌───────────┐  ┌───────────┐      │
│   │ Analytics │  │  CRM     │  │  Dashboards│      │
│   └───────────┘  └───────────┘  └───────────┘      │
│                                                         │
│  ATTRIBUTION LAYER                                      │
│  ┌─────────────────────────────────────────────────┐ │
│  │              Attribution Model                    │ │
│  │  (First Touch, Last Touch, MTA, etc.)          │ │
│  └─────────────────────────────────────────────────┘ │
│                                                         │
└─────────────────────────────────────────────────────────┘
```

---

## Templates

| Template | Use |
|----------|-----|
| `07-ATTR-TEMPLATE-UTM-Master-v1.xlsx` | UTM tracking sheet |
| `07-ATTR-TEMPLATE-Campaign-Tags-v1.xlsx` | Campaign parameter |
| `07-ATTR-TEMPLATE-Conversion-Map-v1.xlsx` | Conversion tracking |
| `07-ATTR-TEMPLATE-ROI-Report-v1.xlsx` | Monthly ROI report |
| `07-ATTR-TEMPLATE-Call-Tracking-v1.xlsx` | Call attribution |

---

## Workflows

| Workflow | Trigger | Action |
|----------|---------|--------|
| ATT-WF-001 | New campaign | Generate UTM + configure tracking |
| ATT-WF-002 | New lead | Log source in CRM |
| ATT-WF-003 | Vehicle sale | Match back to marketing source |
| ATT-WF-004 | Monthly | Generate attribution report |
| ATT-WF-005 | Weekly | Update dashboard with fresh data |
| ATT-WF-006 | Anomaly detected | Alert + investigate |

---

## Case Studies

| Case | Dealer Type | Challenge | Result |
|------|-------------|-----------|--------|
| CASE-001 | Multi-store | Can't track offline | 100% attribution with call tracking |
| CASE-002 | Single store | Google vs Facebook ROI | Data-driven budget shift, +40% ROAS |
| CASE-003 | High-line | No attribution model | Implemented MTA, identified winning channels |
| CASE-004 | Import | $125 CPL | $38 CPL with optimization |

---

## Agent-07 Configuration

**Role:** Analytics & Attribution Specialist  
**Knowledge Base:** This folder and subdocuments  
**Tools Required:**
- Google Analytics 4
- Google Tag Manager
- Attribution platforms (Bizible, Marketo)
- Call tracking (CallRail, Marchex)
- Data visualization (Data Studio, Tableau)
- CRM analytics

**Default Prompts:**
- "Set up multi-touch attribution for [dealership]"
- "Configure UTM tracking for [campaign]"
- "Build a marketing ROI dashboard"
- "Analyze channel performance and recommend budget"
- "Troubleshoot tracking issues with [channel]"

---

*Document Version: 1.0*
*Taxonomy Code: 07-ATTR-MASTER-v1*
