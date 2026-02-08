# Pillar 05: CRM Automation Master Document

**Pillar Code:** 05-CRM  
**Focus:** Lead Management, Follow-up, Automation  
**Agent:** Agent-05 (to be created)  
**Last Updated:** 2026-02-08

---

## Overview

CRM Automation ensures no lead is forgotten, every customer receives timely follow-up, and long-term relationships are nurtured through systematic, personalized communication.

---

## Core Use Cases

### UC-01: Lead Scoring System
**Category:** PROCESS | LDM | SCR  
**Priority:** CRITICAL

**Objective:** Rank leads by likelihood to convert

**Scoring Model:**
```
LEAD SCORE = Intent Score + Engagement Score + Fit Score

INTENT SIGNALS (0-40 points)
├── Website visit to VDP (+5)
├── Multiple VDP views (+10)
├── Price check (+5)
├── Trade-in value check (+10)
├── Credit application (+15)
├── Video watched (+5)
└── Form completed (+10)

ENGAGEMENT SIGNALS (0-30 points)
├── Opened email (+2, max +10)
├── Clicked email link (+5)
├── Clicked SMS (+3)
├── Returned call within 15 min (+10)
├── Scheduled appointment (+15)
└── Visited dealership (+10)

FIT SIGNALS (0-30 points)
├── In-market timeframe (+10)
├── Trade-in available (+5)
├── Credit qualified (+10)
├── Match to inventory (+10)
└── Referred by customer (+5)

TOTAL: 0-100 points
```

**Related Documents:**
- `05-CRM-PROCESS-LDM-Scoring-v1.md`
- `05-CRM-WORKFLOW-LDM-Automation-v1.md`

---

### UC-02: Multi-Touch Follow-up Cadence
**Category:** WORKFLOW | FUP | SEQ  
**Priority:** CRITICAL

**Objective:** Systematic lead nurturing over 90+ days

**90-Day Nurture Sequence:**

```
DAY 0: INITIAL RESPONSE
├── Hour 0: Auto-acknowledgment
├── Hour 1: Personal follow-up
├── Hour 2: Send inventory match
└── Day 1: Value proposition email

DAY 3
├── Email: Customer testimonial
├── SMS: Quick check-in
└── Retargeting ad

DAY 7
├── Email: Market inventory update
├── Personal call attempt
└── Social connection

DAY 14
├── Email: Competitive comparison
├── SMS: Appointment availability
└── Retargeting

DAY 21
├── Email: Special offer
├── Personal call
└── Direct mail piece

DAY 30
├── Email: Monthly digest
├── Social engagement
└── Retargeting

DAY 45
├── Check-in call
├── Needs reassessment
└── Timeline update

DAY 60-90
├── Quarterly outreach
├── New model announcement
└── Milestone recognition
```

**Related Documents:**
- `05-CRM-WORKFLOW-FUP-90Day-v1.md`
- `05-CRM-TEMPLATE-Email-FollowUp-v1.docx`

---

### UC-03: Customer Segmentation
**Category:** PROCESS | SEG | DST  
**Priority:** HIGH

**Objective:** Group customers for targeted communication

**Segments:**
```
┌─────────────────────────────────────────────────────────┐
│                   CUSTOMER SEGMENTS                         │
├─────────────────────────────────────────────────────────┤
│                                                         │
│  PROSPECT SEGMENTS                                      │
│  ├── Active Shoppers (score 70+)                       │
│  ├── Warm Leads (score 40-69)                          │
│  ├── Cold Leads (score 0-39)                           │
│  └── Nurture Pool (no timeline)                        │
│                                                         │
│  CUSTOMER SEGMENTS                                     │
│  ├── Recent Buyers (0-6 months)                        │
│  ├── Loyal Customers (multiple purchases)               │
│  ├── Service-only Customers                            │
│  ├── At-Risk (no engagement 6+ months)                 │
│  └── Churned (defected to competitor)                   │
│                                                         │
│  SERVICE SEGMENTS                                      │
│  ├── High-Value Service (>$500/RO)                     │
│  ├── Maintenance Focused                               │
│  ├── Express/Lube Only                                 │
│  └── Warranty Work                                     │
│                                                         │
└─────────────────────────────────────────────────────────┘
```

**Related Documents:**
- `05-CRM-PROCESS-SEG-Segmentation-v1.md`

---

### UC-04: Service Reminder Automation
**Category:** WORKFLOW | AUT | SVC  
**Priority:** HIGH

**Objective:** Drive service retention through automation

**Trigger Points:**
```
MILESTONE-BASED
├── 30 days before expected service
├── 60 days since last visit
├── 5,000 miles over (based on odometer)
├── Manufacturer recall available
└── Seasonal (summer/winter prep)

BEHAVIOR-BASED
├── Vehicle page viewed (retargeting)
├── Competitor website visit
├── Expressed interest in service
└── Previous no-show (extra touch)
```

**Related Documents:**
- `05-CRM-WORKFLOW-AUT-ServiceReminders-v1.md`

---

### UC-05: Long-Term Follow-up System
**Category:** PROCESS | FUP | LTF  
**Priority:** MEDIUM

**Objective:** Maintain relationships with customers beyond transaction

**Annual Touch Calendar:**
```
MONTHLY
├── Birthday/anniversary email
├── Service reminder (if due)
└── Loyalty points summary

QUARTERLY
├── Vehicle care tips
├── New model update
└── Satisfaction check

ANNUALLY
├── Trade-in valuation offer
├── Warranty expiration reminder
└── Referral request

MILESTONE
├── 1-year ownership anniversary
├── 50,000 mile milestone
└── Lease return reminder
```

**Related Documents:**
- `05-CRM-PROCESS-FUP-AnnualCalendar-v1.md`

---

## Key Performance Indicators

| KPI | Target | Top Performer |
|-----|--------|---------------|
| Lead response time | < 5 min | < 2 min |
| Lead contact rate | 90%+ | 98%+ |
| Lead-to-appointment | 15%+ | 25%+ |
| Follow-up completion | 100% | 100% |
| Email open rate | 20%+ | 30%+ |
| SMS response rate | 15%+ | 25%+ |
| 30-day engagement | 60%+ | 80%+ |
| Lead-to-sale (90 day) | 8%+ | 15%+ |

---

## Templates

| Template | Use |
|----------|-----|
| `05-CRM-TEMPLATE-Scoring-Rules-v1.json` | Lead scoring config |
| `05-CRM-TEMPLATE-Email-FollowUp-v1.docx` | Follow-up emails |
| `05-CRM-TEMPLATE-SMS-Sequence-v1.xlsx` | SMS templates |
| `05-CRM-TEMPLATE-Segmentation-v1.xlsx` | Customer segments |
| `05-CRM-TEMPLATE-Service-Reminder-v1.docx` | Service emails |

---

## Workflows

| Workflow | Trigger | Action |
|----------|---------|--------|
| CRM-WF-001 | New lead | Score + assign + auto-respond |
| CRM-WF-002 | Score change (up) | Increase priority + notify |
| CRM-WF-003 | Score change (down) | Add to nurture pool |
| CRM-WF-004 | Appointment booked | Remove from follow-up sequence |
| CRM-WF-005 | Vehicle purchased | Add to customer journey |
| CRM-WF-006 | Service completed | Add to service retention |
| CRM-WF-007 | 30 days no engagement | Re-engagement campaign |
| CRM-WF-008 | Negative survey | Alert manager + recovery |

---

## Case Studies

| Case | Dealer Type | Challenge | Result |
|------|-------------|-----------|--------|
| CASE-001 | Multi-store | 3% lead-to-sale | 11% with 90-day nurture |
| CASE-002 | High-line | 40% lead contact | 95% with automation |
| CASE-003 | Import | Service retention 45% | 78% with reminders |
| CASE-004 | Domestic | 15% follow-up | 100% with CRM workflows |

---

## Agent-05 Configuration

**Role:** CRM & Automation Specialist  
**Knowledge Base:** This folder and subdocuments  
**Tools Required:**
- CRM platforms (Tekion, Dealertrack, VinSolutions)
- Email platforms (Klaviyo, Mailchimp)
- SMS platforms (Podium, Texting Edge)
- Analytics tools

**Default Prompts:**
- "Design lead scoring for [dealership]"
- "Create a 90-day follow-up sequence"
- "Build service reminder automation"
- "Segment our customer database"
- "Set up CRM workflows for [trigger]"

---

*Document Version: 1.0*
*Taxonomy Code: 05-CRM-MASTER-v1*
