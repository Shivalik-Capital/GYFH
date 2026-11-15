# GYFH Discord Server Setup Guide

> **Architecture Purpose**:  
> A professional, low-maintenance, and 100% async Discord server engineered for 200–300 student participants, adult judges/mentors, and staff. Built to minimize DM spam and enforce child safety.

---

## 👥 Role Hierarchy & Color Scheme

Create these roles in Discord (`Server Settings > Roles`) from top to bottom:

| Role Name | Color | Permissions | Purpose |
| :--- | :--- | :--- | :--- |
| **Organizer / Staff** | Red / Gold | Administrator | You and your co-leads. |
| **Advisor / Judge** | Purple | Mentionable, Embed Links, Manage Messages in Stage | Industry professionals & evaluators. |
| **Mentor** | Blue | Mentionable, Embed Links, Attach Files | Office hours and technical guides. |
| **Ambassador** | Orange | Mentionable, Embed Links | Student club leads promoting GYFH. |
| **Participant** | Green | Send Messages, Read Message History | Verified student hackers who accepted rules. |
| **Unverified** | Gray | Read-only in `#welcome` & `#rules` | New joins before completing onboarding. |

---

## 📁 Category & Channel Structure

```text
📢 INFORMATION & RULES
├── 📌 #welcome               (Read-only: Event summary, dates: March 26–28, 2027)
├── 📜 #rules-and-conduct     (Read-only: Anti-harassment, safety, reaction-role to unlock server)
├── 📣 #announcements         (Read-only: Official news and milestones)
├── ❓ #faq                   (Read-only: Tracks, team sizes, sandbox rules)
└── 🗓️ #schedule               (Read-only: Timetable, workshop links, Apollo bot countdowns)

💬 COMMUNITY HUB
├── 💬 #general               (Open discussion, introductions)
├── 🛠️ #tech-stack-talk       (Languages, APIs, sandbox questions)
├── 💡 #project-ideas         (Brainstorming, feedback on concepts)
└── 🤖 #bot-commands          (Checking timezone conversions, level checks)

🤝 TEAM FORMATION
├── 🔎 #find-a-team           (Solo builders posting skills and timezone)
├── 👥 #teams-seeking-members (Teams looking for frontend/backend/designers)
└── 🏆 #team-registration     (Link to official team submission form)

🎓 TRACK BREAKOUTS (Forum or Text Channels)
├── 📚 #track-1-money-education
├── 💰 #track-2-smart-saving
└── 🌐 #track-3-social-finance

🆘 SUPPORT & MENTORSHIP
├── 🎟️ #get-help               (Ticket Tool bot: Opens private staff ticket for questions)
├── 🙋 #mentor-queue          (Public forum: post a question, mentor replies in thread)
└── 🚨 #report-incident       (Direct private ticket to Organizers for safety issues)

🔒 STAFF ONLY (Hidden from everyone else)
├── 💬 #core-chat             (Day-to-day organizer coordination)
├── 📋 #task-board            (Links to CRM, Notion, sheets)
└── 📝 #decision-log          (Documenting all major decisions async)
```

---

## 🤖 Recommended Bot Stack (100% Free Tiers)

### 1. Carl-bot (Reaction Roles & Moderation)
- **Role Verification**: Put a message in `#rules-and-conduct`:  
  *"Click the ✅ reaction to agree to the Code of Conduct and unlock all participant channels."*
- **Auto-Mod**:
  - Filter invite links (`discord.gg/*`) to prevent spam raids.
  - Filter profanity and slurs.

### 2. Ticket Tool (Zero-DM Support System)
- **Why it matters**: You don't want 300 students DMing your personal Discord account at 3:00 AM.
- **Setup**:
  - Place a panel in `#get-help`: *"Need help? Click 'Open Ticket' to talk to GYFH staff."*
  - Automatically creates a private channel `#ticket-001` visible only to the student and staff.
  - Automatically archives the transcript when closed.

### 3. Apollo / Sesh (Timezone & Event Bot)
- **Why it matters**: Students will be in UTC+8 (Singapore), UTC+5:30 (India), UTC-5 (New York), UTC+0 (London).
- **Setup**:
  - Post events in `#schedule` using `/event create`.
  - Apollo displays the start time in each user's exact local timezone automatically.

---

## 🛡️ Critical Safety & Minor Protection Setup

1. **Explicit DM Protection**:
   - Post an explicit notice in `#rules-and-conduct`:  
     > *"GYFH organizers, mentors, and judges will NEVER direct message (DM) you privately. All mentorship and troubleshooting occurs in public channels or official `#get-help` tickets. Never share real banking credentials or passwords."*
2. **Mentorship Channel Rule**:
   - Mentors do not conduct 1-on-1 private voice calls with minors.
   - All questions are asked in `#mentor-queue` or open Discord Stages where other participants/staff are present.
