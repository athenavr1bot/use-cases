# CLAWChat Gateway PRD Summary

**Quick reference for the ClawChat Gateway mobile application**

---

## At a Glance

| Aspect | Details |
|--------|---------|
| **Product** | Mobile-first chat gateway for OpenClaw |
| **Platforms** | iOS 15+ / Android 8+ |
| **Design Inspiration** | iMessage, Slack, Discord, ChatGPT |
| **Core Philosophy** | Chat is the only interface |
| **Primary Users** | Automotive consultants, operators, executives |

---

## The 4 Pillars (v1)

| Pillar | Focus | Use Cases |
|--------|-------|-----------|
| **1. Sales Operations** | Lead response, BDC, CRM | "What's my closing rate?" |
| **2. Marketing & Attribution** | Lead sources, ROI, vendors | "Show CPL by channel" |
| **3. Fixed Ops** | 🔒 Placeholder for v2 | Service, CSI, capacity |
| **4. Team Performance** | KPIs, coaching, accountability | "Create coaching plan" |

---

## What v1 INCLUDES

✅ Real-time chat (WebSocket)  
✅ Typing indicators  
✅ Message reactions  
✅ Quick reply suggestions  
✅ Pillar-aware context  
✅ Role-based access (Consultant/Operator/Executive)  
✅ Offline caching  
✅ Structured AI responses (KPIs, cards, actions)  
✅ Local language: Automotive native  

---

## What v1 EXCLUDES

❌ Dashboards  
❌ CRM UI  
❌ Settings screens  
❌ Voice/video calls  
❌ Workflow builder  
❌ Complex integrations  

---

## Chat Features

### Message Types
```
👤 USER        → Plain text, voice, attachments
🤖 AI          → Text, structured cards, action buttons
📢 SYSTEM     → Context hints, suggestions, transitions
🔔 NOTIFY     → Alerts, completions, mentions
```

### Interactions
- Typing indicators
- Quick reply chips
- Swipe actions (archive, star, delete)
- Long-press reactions
- Thread support

---

## User Flow

```
Open App → Start Typing → Send → AI Response → Complete Task
    │            │           │          │
    ▼            ▼           ▼          ▼
[New Session]  [Context]  [Thinking] [Result]
```

---

## Technical Stack

```
Mobile (v1)          Gateway Layer        OpenClaw
─────────────         ──────────────        ──────────
iOS: SwiftUI         Auth + Session       7 Agents
Android: Compose     Context Manager       Tools + Memory
Chat SDK             Pillar Router        Knowledge Base
WebSocket            Rate Limiter
```

---

## Success Metrics

| Metric | Target |
|--------|--------|
| DAU / MAU | 80%+ |
| Session Duration | < 2 min avg |
| Messages / Session | 3-5 |
| Task Completion | 70%+ |
| Time to First Response | < 1s |
| App Launch | < 2s |

---

## Timeline

| Phase | Weeks | Deliverables |
|-------|-------|--------------|
| Foundation | 1-4 | App scaffold, basic chat |
| Core Chat | 5-8 | Real-time, caching, offline |
| Automotive Context | 9-12 | Pillars, routing, roles |
| Polish | 13-16 | Performance, launch prep |

---

## Design System

```
Colors:
  Primary: #6366F1 (Indigo)
  Secondary: #10B981 (Emerald)
  Accent: #F59E0B (Amber)

Typography:
  Headlines: SF Pro / Roboto
  Body: SF Pro Text / Roboto
  Data: SF Mono / Roboto Mono

Spacing:
  Screen padding: 16pt
  Message padding: 12pt
  Message gap: 4pt
```

---

## Key Files

| Document | Purpose |
|----------|---------|
| `CLAWCHAT_GATEWAY_PRD.md` | Full PRD with all details |
| `CLAWCHAT_QUICKSTART.md` | This summary |
| `use-cases/03_marketing/` | Marketing pillar context |
| `use-cases/05_crm-automation/` | CRM automation context |

---

*Version: 1.0 | 2026-02-08*
