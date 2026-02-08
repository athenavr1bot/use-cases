# Pillar 02: Variable Operations Master Document

**Pillar Code:** 02-VAROPS  
**Focus:** Sales & Finance/Insurance Optimization  
**Agent:** Agent-02 (to be created)  
**Last Updated:** 2026-02-08

---

## Overview

Variable Operations encompasses the vehicle sales department, typically the highest-profile but lowest-margin area of the dealership (5-10% gross). Success requires volume, process discipline, and strong F&I performance.

---

## Core Use Cases

### UC-01: Sales Team Structure Optimization
**Category:** PROCESS | SLS | STR  
**Priority:** HIGH

**Objective:** Design optimal sales team for dealership size

**Key Decisions:**
- Number of salespeople (formula: monthly unit target / 10-12)
- Floor vs. internet allocation
- BDC model vs. individual responsibility
- Sales manager span of control

**Related Documents:**
- `02-VAROPS-PROCESS-SLS-Team-Design-v1.md`
- `02-VAROPS-PLAYBOOK-Sales-Management-v1.md`

---

### UC-02: Lead Response Excellence
**Category:** WORKFLOW | INT | LDM  
**Priority:** CRITICAL

**Objective:** Maximize lead-to-appointment conversion

**Standards:**
- Response time: < 5 minutes
- Contact attempts: 8+ within 30 days
- Channels: Phone, SMS, Email, Video
- Documentation: Every touch logged

**Workflow:**
```
Lead Incoming
    ↓
< 5 minute response
    ↓
Qualification (5 questions)
    ↓
Appointment Setting
    ↓
Confirmation & Reminder
    ↓
Show Rate Follow-up
```

**Related Documents:**
- `02-VAROPS-WORKFLOW-INT-Lead-Response-v1.md`
- `02-VAROPS-PROCESS-INT-Qualification-v1.md`

---

### UC-03: F&I Penetration Program
**Category:** PROCESS | FNI | PEN  
**Priority:** HIGH

**Objective:** Maximize Finance & Insurance product sales

**Key Products:**
- Finance reserve (target: $2,000+)
- Extended warranties (60%+ penetration)
- Gap insurance (40%+)
- Maintenance contracts (30%+)
- Theft protection (20%+)

**F&I Stack:**
1. Finance Reserve (non-negotiable)
2. Gap (high margin, easy sale)
3. Warranty (highest dollar)
4. Maintenance (loyalty builder)
5. Theft/Etch (add-on)

**Related Documents:**
- `02-VAROPS-PROCESS-FNI-Penetration-v1.md`
- `02-VAROPS-STANDARD-FNI-Benchmarks-v1.md`

---

### UC-04: Desking Excellence
**Category:** PROCESS | DES | STR  
**Priority:** MEDIUM

**Objective:** Structure deals for maximum profitability

**Key Elements:**
- Vehicle pricing strategy
- Trade-in valuation
- Finance rate optimization
- Product presentation order
- Negotiation approach

**Related Documents:**
- `02-VAROPS-PROCESS-Desking-v1.md`
- `02-VAROPS-WORKFLOW-DES-Pricing-v1.md`

---

### UC-05: Inventory Turn Optimization
**Category:** PROCESS | INV | TURN  
**Priority:** HIGH

**Objective:** Minimize days in inventory while maintaining margins

**Target:** 45-60 days average

**Strategies:**
- Front-line vs. wholesale allocation
- Pricing adjustments based on age
- Market-based merchandising
- Auction vs. retail decisions

**Related Documents:**
- `02-VAROPS-PROCESS-INV-Management-v1.md`
- `02-VAROPS-STANDARD-INV-Benchmarks-v1.md`

---

## Key Performance Indicators

| KPI | Formula | Target | Top Performer |
|-----|---------|--------|---------------|
| Turn | Units/Month/Salesperson | 12+ | 18+ |
| Closing Rate | Units/Up % | 20-25% | 30%+ |
| Front Gross | Gross on vehicle | $800-1,500 | $2,000+ |
| Back Gross | F&I gross/unit | $1,500+ | $2,500+ |
| PVR | Total Gross / Units | $2,500+ | $4,000+ |
| Internet Closing | Leads/Appt/Close % | 8%/25%/15% | 12%/35%/22% |
| Days in Inventory | Avg days to sell | 45-60 | 30-45 |

---

## Sales Funnel Metrics

```
┌─────────────────────────────────────────────────────────┐
│                    SALES FUNNEL                          │
├─────────────────────────────────────────────────────────┤
│                                                         │
│  Website Traffic                                        │
│       ↓                                                 │
│  Leads Generated    [Target: 100+/month]              │
│       ↓                                                 │
│  Contacts Made       [Target: 90%+ contact rate]        │
│       ↓                                                 │
│  Appointments Set    [Target: 25%+ of contacts]         │
│       ↓                                                 │
│  Appointments Shown  [Target: 80%+ show rate]           │
│       ↓                                                 │
│  Vehicles Sold       [Target: 15%+ close on appt]        │
│       ↓                                                 │
│  F&I Products       [Target: $1,500+/vehicle]          │
│       ↓                                                 │
│  Customer Delivery   [Target: 100% with ceremony]       │
│       ↓                                                 │
│  Follow-up          [Target: 48-hour check-in]         │
│                                                         │
└─────────────────────────────────────────────────────────┘
```

---

## Common Problems & Solutions

| Problem | Root Cause | Solution |
|---------|------------|----------|
| Low closing rate | Poor qualification | BDC script training |
| Front gross bleed | Negotiation weakness | Desking training |
| Low F&I income | Advisor avoidance | Scripting + closing training |
| Old inventory | Pricing strategy | Market-based repricing |
| Low show rate | Reminder gaps | Multi-channel confirmation |
| Lead response slow | Process gaps | < 5 minute rule enforcement |

---

## Templates

| Template | Use |
|----------|-----|
| `02-VAROPS-TEMPLATE-Lead-Tracker-v1.xlsx` | Daily lead management |
| `02-VAROPS-TEMPLATE-Sales-Call-Sheet-v1.pdf` | Phone script |
| `02-VAROPS-TEMPLATE-Desking-Worksheet-v1.xlsx` | Deal structuring |
| `02-VAROPS-TEMPLATE-FNI-Menu-v1.pdf` | Product presentation |
| `02-VAROPS-TEMPLATE-Delivery-Checklist-v1.pdf` | Handover ceremony |

---

## Workflows

| Workflow | Trigger | Action |
|----------|---------|--------|
| VAR-WF-001 | New lead | Auto-response + SMS + assign |
| VAR-WF-002 | 5 min no contact | Escalation to manager |
| VAR-WF-003 | Appointment booked | Send confirmation + video |
| VAR-WF-004 | 1 day before | Reminder SMS + call |
| VAR-WF-005 | Customer arrives | Check-in + notify sales |
| VAR-WF-006 | Deal written | Notify F&I + delivery prep |
| VAR-WF-007 | Deal delivered | Send survey + 48hr follow-up |
| VAR-WF-008 | 7 days post-delivery | Satisfaction check |

---

## Case Studies

| Case | Dealer Type | Challenge | Result |
|------|-------------|-----------|--------|
| CASE-001 | High-line import | 12% closing rate | 24% in 90 days |
| CASE-002 | Domestic store | $1,800 F&I PVR | $3,200 in 6 months |
| CASE-003 | Internet-heavy | 5% lead-to-close | 11% with BDC |
| CASE-004 | Multi-store | 65-day inventory turns | 42 days avg |

---

## Agent-02 Configuration

**Role:** Variable Operations Specialist  
**Knowledge Base:** This folder and subdocuments  
**Tools Required:**
- DMS access
- CRM (Dealertrack, Tekion, etc.)
- Desking tools
- Inventory management
- Communication platforms

**Default Prompts:**
- "Analyze our sales funnel conversion"
- "Create a lead response improvement plan"
- "Design F&I training program"
- "Optimize our inventory pricing strategy"
- "Build a sales team compensation plan"

---

*Document Version: 1.0*
*Taxonomy Code: 02-VAROPS-MASTER-v1*
