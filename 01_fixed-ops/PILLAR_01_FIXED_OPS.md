# Pillar 01: Fixed Operations Master Document

**Pillar Code:** 01-FIXOPS  
**Focus:** Service & Parts Department Optimization  
**Agent:** Agent-01 (to be created)  
**Last Updated:** 2026-02-08

---

## Overview

Fixed Operations is the backbone of dealership profitability, typically generating 40-60% of total dealership profit with significantly less volatility than sales.

---

## Core Use Cases

### UC-01: Service Absorption Analysis
**Category:** PROCESS | SVC | ABS  
**Priority:** HIGH

**Objective:** Calculate and improve service absorption rate

**Formula:**
```
Service Absorption = (Service Gross + Parts Gross) / Total Dealership Expenses
                    excluding floorplan interest
```

**Target:** 80%+ minimum, 100%+ optimal

**Process:**
1. Extract financial data from DMS
2. Calculate absorption for last 12 months
3. Identify trends and gaps
4. Benchmark against top performers
5. Develop improvement plan

**Related Documents:**
- `01-FIXOPS-PROCESS-ABS-Calculation-v1.md`
- `01-FIXOPS-PLAYBOOK-Absorption-Improvement-v1.md`

---

### UC-02: CSI Improvement Program
**Category:** PROCESS | SVC | CSI  
**Priority:** HIGH

**Objective:** Improve Customer Satisfaction Index scores

**Key Metrics:**
- Overall satisfaction
- Service advisor performance
- Service write-up clarity
- Repair quality perception
- Vehicle return rate

**Process:**
1. Analyze last 12 months CSI data
2. Identify root causes of low scores
3. Implement service advisor training
4. Create feedback loops
5. Monitor and adjust

**Related Documents:**
- `01-FIXOPS-PROCESS-CSI-Analysis-v1.md`
- `01-FIXOPS-WORKFLOW-CSI-Feedback-v1.md`

---

### UC-03: Technician Productivity Optimization
**Category:** PROCESS | SVC | TEC  
**Priority:** HIGH

**Objective:** Maximize technician efficiency and output

**Key Metrics:**
- Efficiency % (hours sold / hours worked)
- Labor gross per technician
- Repair order count
- Flag hours vs. actual hours

**Target:** 85%+ efficiency minimum

**Related Documents:**
- `01-FIXOPS-PROCESS-TEC-Productivity-v1.md`
- `01-FIXOPS-STANDARD-TEC-Benchmarks-v1.md`

---

### UC-04: Parts Inventory Optimization
**Category:** PROCESS | PRT | INV  
**Priority:** MEDIUM

**Objective:** Right-size parts inventory for maximum turns

**Key Metrics:**
- Inventory turns (target: 4-6 annually)
- Stock-out rate
- Obsolescence percentage
- Gross margin percentage

**Related Documents:**
- `01-FIXOPS-PROCESS-PRT-Inventory-v1.md`

---

### UC-05: Appointment Scheduling System
**Category:** WORKFLOW | SVC | SCH  
**Priority:** HIGH

**Objective:** Maximize capacity utilization and customer convenience

**Components:**
- Online booking integration
- Confirmation SMS/email
- Reminder sequences
- Capacity planning
- No-show reduction

**Related Documents:**
- `01-FIXOPS-WORKFLOW-SCH-Appointment-v1.md`

---

## Key Performance Indicators

| KPI | Formula | Target | Top Performer |
|-----|---------|--------|---------------|
| Service Absorption | (Svc+Parts Gross)/Expenses | 80%+ | 100%+ |
| RO Average | Total Svc Gross / # ROs | $350-400 | $500+ |
| Service CSI | Manufacturer score | 900+ | 960+ |
| Parts Turns | COGS / Avg Inventory | 4-6 | 8+ |
| Tech Efficiency | Hours Sold / Hours Worked | 85%+ | 95%+ |
| Appointment Show Rate | Showed / Appointments | 85% | 95%+ |

---

## Common Problems & Solutions

| Problem | Root Cause | Solution |
|---------|------------|----------|
| Low absorption | Poor sales training | F&I product training |
| Low CSI | Advisor performance | Coaching program |
| Tech inefficiency | Supervision gaps | Real-time monitoring |
| Parts obsolescence | Poor buying | Demand-based ordering |
| No-shows | Poor communication | Multi-channel reminders |

---

## Templates

| Template | Use |
|----------|-----|
| `01-FIXOPS-TEMPLATE-SVC-Roaster-v1.xlsx` | Weekly tech schedule |
| `01-FIXOPS-TEMPLATE-ABS-Tracker-v1.xlsx` | Absorption dashboard |
| `01-FIXOPS-TEMPLATE-CSI-Analysis-v1.xlsx` | CSI trending |
| `01-FIXOPS-TEMPLATE-PRT-Inventory-v1.xlsx` | Parts optimization |

---

## Workflows

| Workflow | Trigger | Action |
|----------|---------|--------|
| SVC-WF-001 | Customer books online | Send confirmation SMS |
| SVC-WF-002 | 24 hours before | Send reminder SMS/email |
| SVC-WF-003 | Customer arrives | Check-in automation |
| SVC-WF-004 | RO completed | Send satisfaction survey |
| SVC-WF-005 | Low CSI score | Alert manager, trigger coaching |

---

## Case Studies

| Case | Dealer Type | Challenge | Result |
|------|-------------|-----------|--------|
| CASE-001 | Multi-store group | 65% absorption | +25% points in 6 months |
| CASE-002 | Single store | 820 CSI | 955 CSI in 4 months |
| CASE-003 | High-line | Tech efficiency 72% | 91% in 90 days |

---

## Agent-01 Configuration

**Role:** Fixed Operations Specialist  
**Knowledge Base:** This folder and subdocuments  
**Tools Required:**
- DMS access (Tekion, CDK, Reynolds)
- Spreadsheet tools
- CRM access
- Communication platforms

**Default Prompts:**
- "Analyze our service absorption"
- "Create a CSI improvement plan"
- "Optimize technician scheduling"
- "Design parts inventory strategy"

---

*Document Version: 1.0*
*Taxonomy Code: 01-FIXOPS-MASTER-v1*
