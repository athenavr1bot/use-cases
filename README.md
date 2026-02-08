# Use Cases & Agents Index

**Central reference for all documents and agents**

---

## Document Repository Structure

```
use-cases/
├── DOCUMENT_TAXONOMY.md          ← Start here for organization
├── agents/                        ← Agent configurations
│   ├── agent-01-fixedops.json
│   ├── agent-02-variableops.json
│   ├── agent-03-marketing.json
│   ├── agent-04-api.json
│   ├── agent-05-crm.json
│   ├── agent-06-graphics.json
│   └── agent-07-attribution.json
├── 01_fixed-ops/                 ← Pillar 1
│   └── PILLAR_01_FIXED_OPS.md
├── 02_variable-ops/              ← Pillar 2
│   └── PILLAR_02_VARIABLE_OPS.md
├── 03_marketing/                 ← Pillar 3
│   └── PILLAR_03_MARKETING.md
├── 04_api-config/                ← Pillar 4
│   └── PILLAR_04_API.md
├── 05_crm-automation/            ← Pillar 5
│   └── PILLAR_05_CRM.md
├── 06_graphics/                 ← Pillar 6
│   └── PILLAR_06_GRAPHICS.md
└── 07_attribution/               ← Pillar 7
    └── PILLAR_07_ATTRIBUTION.md
```

---

## Quick Reference

| Pillar | Agent | Focus | Master Doc |
|--------|-------|-------|------------|
| 01-Fixed Ops | Agent-01 | Service/Parts | PILLAR_01_FIXED_OPS.md |
| 02-Variable Ops | Agent-02 | Sales/F&I | PILLAR_02_VARIABLE_OPS.md |
| 03-Marketing | Agent-03 | Strategy/Channels | PILLAR_03_MARKETING.md |
| 04-API | Agent-04 | Integrations | PILLAR_04_API.md |
| 05-CRM | Agent-05 | Lead/Automation | PILLAR_05_CRM.md |
| 06-Graphics | Agent-06 | Design/Brand | PILLAR_06_GRAPHICS.md |
| 07-Attribution | Agent-07 | Analytics/ROI | PILLAR_07_ATTRIBUTION.md |

---

## Document Coding System

Format: `[PILLAR]-[TYPE]-[CATEGORY]-[NAME]`

**Example:** `01-FIXOPS-PROCESS-SVC-Appointment-Scheduling-v1.md`

### Pillar Codes

| Code | Pillar |
|------|--------|
| 01 | Fixed Operations |
| 02 | Variable Operations |
| 03 | Marketing |
| 04 | API Config |
| 05 | CRM Automation |
| 06 | Graphics |
| 07 | Attribution |

### Type Codes

| Code | Type |
|------|------|
| PROCESS | Process Document |
| WORKFLOW | Workflow Definition |
| TEMPLATE | Template |
| CASE | Case Study |
| PLAYBOOK | Playbook |
| REFERENCE | Reference Material |
| STANDARD | Standards Doc |
| TRAINING | Training Material |

---

## Using This System

### Finding Documents

| Need | Search |
|------|--------|
| All fixed ops documents | `01-FIXOPS-*` |
| All CRM workflows | `05-CRM-WORKFLOW-*` |
| All templates | `*-TEMPLATE-*` |
| All case studies | `*-CASE-*` |

### Adding New Documents

1. Follow naming convention
2. Add required metadata header
3. Place in correct pillar folder
4. Update related documents (Master Doc)
5. Commit to GitHub

### Activating an Agent

Reference the agent by Pillar:

| Say This... | Activates... |
|-------------|--------------|
| "Agent-01, analyze our absorption" | Fixed Ops Specialist |
| "Agent-02, improve our closing rate" | Variable Ops Specialist |
| "Agent-03, build a marketing plan" | Marketing Specialist |
| "Agent-04, configure API integration" | API Specialist |
| "Agent-05, create follow-up sequence" | CRM Specialist |
| "Agent-06, design brand guidelines" | Creative Specialist |
| "Agent-07, set up attribution" | Analytics Specialist |

---

## GitHub Sync

**Repository:** https://github.com/athenavr1bot/use-cases

```bash
# Pull latest changes
git pull origin main

# Add new document
git add [filename]
git commit -m "Add: [Document Name]"
git push origin main
```

---

*Last Updated: 2026-02-08*
*Version: 1.0*
