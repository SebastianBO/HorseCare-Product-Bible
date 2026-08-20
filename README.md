# HorseCare Product Bible

**The complete operating system for horse owners — Cal AI ease for equine health.**

*Living document | Updated August 20, 2026 | Team: Grok, Harper, Lucas, Benjamin*

## Vision

HorseCare is the oldest and best iOS equestrian app, with millions of community posts (Facebook for horses). We now deliver the Cal AI moment for every horse: snap a photo → instant weight, BCS, hay quality, conformation and hoof intelligence → clear daily actions.

**Core:** Daily management of *your* horse(s). Marketplace and Community amplify the flywheel.

## Market Capture

- Global horse software market $1.8B (2025) → $3.9B (2034)
- ~12M private owners; US 7.2M horses
- Per-horse spend $3.5k–$10k+/yr

**Path to own the market:**
1. Viral individual habit (first scan magic)
2. Multi-horse barns (higher ARPU + team)
3. Professionals (leads + advocacy)
4. Marketplace liquidity from real needs
5. Data moat (best equine vision model)

## Pricing (Willingness to Pay)

**Free:** 3 AI scans/mo, basic dashboard, community view.

**Premium Individual:** $4.99/mo or **$39.99–$59.99/yr** (Best Value)
- Unlimited AI, full nutrition plans, multi-horse (≤5), reports, streaks.

**Barn/Pro:** $14.99–$49.99/mo
- Unlimited horses, staff seats, marketplace boosts, advanced analytics.

ROI: Prevents expensive issues; feed optimization alone pays for itself.

## Design System (Locked – AAA)

- Pure white background
- Deep forest green #0A7A4B primary / #22C55E accent
- Soft 20px radius white cards with subtle shadows
- SF Pro typography, bold large metrics
- Generous whitespace, large touch targets, progressive disclosure, one primary CTA per screen
- Trust signals: Confidence %, ± ranges, “AI estimate – always consult your vet”
- Animations: count-up numbers, sequential card reveals, streak confetti

### Exact Tab Bar (NON-NEGOTIABLE – identical on every screen)

Five tabs + elevated center FAB. Pixel-identical on ALL screens (only active state changes):

1. **Home** – house icon
2. **Progress** – bar chart icon
3. **Community** – people icon
4. **Marketplace** – shopping bag / storefront icon
5. **Profile** – person icon

- Active: filled #0A7A4B icon + bold green label
- Inactive: gray outline icons + gray labels (#8E8E93)
- Elevated circular green FAB (white + or horse silhouette) floating above the bar, centered
- Same height (~49pt + home indicator), same icon size, same label size (SF Pro ~10pt), same padding, same subtle top shadow on every single screen
- Never change order, labels, icons, or hide (except pure full-screen onboarding / paywall / camera AR flows)

**Prompt lock text (paste into every image generation):**
“Perfect identical bottom tab bar on every screen: Home (house), Progress (chart), Community (people), Marketplace (bag), Profile (person). Active tab filled deep green #0A7A4B with bold label. Inactive gray. Elevated circular green FAB with white + floating centered above the bar. Exact same height, spacing, icon size, font on all screens.”

## AI Possible vs Not

**Strong:** Weight/BCS from photo, hay type + approx protein, conformation overlays, hoof visual condition, trends over time, risk flags, confidence scoring.

**Limited / Never claim:** Exact lab-grade nutrition, medical diagnosis, absolute weight without scale reference, clinical lameness diagnosis from still photos.

Always show confidence and disclaimer.

## The Gauntlet Flywheel (Daily Habit Engine)

Trigger (smart notification or open app) → Morning Briefing (Home) → Zero-friction Scan or Log (FAB) → Instant AI reward + streak → Auto-updated Nutrition / Care suggestions → Data investment (Profile Timeline) → Shareable win (Community) → Contextual Marketplace when needed.

Amplifiers: Streaks, before/after transformations, barn team contributions, network-improved AI.

## Onboarding (Conversion Machine)

Personalized long flow (Cal AI style):
Welcome → Value props → Goals → Number of horses → Horse basics → Workload/conditions → Guided first scan (AR overlays magic) → Results aha moment → Personalized plan → Notification permission → Soft review ask → Paywall (personalized headline, annual default, trial, social proof, restore).

## Screen Inventory – Deep Analysis (Why / Useful / Can we simplify?)

### 1. Home / Morning Briefing (Primary daily screen)
**Why:** The single most important screen. Answers “How is my horse today and what do I need to do?”
**Useful?** Extremely – highest frequency. Health Index + next actions + upcoming care.
**Simplify:** Absorb “This Week’s Care” list here so full Calendar is demoted. Adaptive: single horse = full briefing; multi = status cards + needs-attention.
**Real text example:** “Good morning, Sarah. Bella’s Health Index is 92 — up 3 pts this week. Farrier due in 4 days. Ready for a quick scan?”

### 2. Scan Results (AI magic)
**Why:** The core product moment (Cal AI photo → intelligence).
**Useful?** Essential. Delivers the wow and the actionable data.
**Simplify:** Progressive disclosure. Nutrition recommendation and Share live as sections or sheets inside Results, not separate full screens.
**Real text:** “Weight estimated 1,142 lbs (±3%). BCS 5.2 — ideal range. Confidence 94%. AI estimate – consult your vet for medical decisions.”

### 3. Progress (Graphs, streaks, motivation)
**Why:** Retention engine. Shows investment paying off.
**Useful?** High for engaged users. Shareable transformations drive virality.
**Simplify:** Keep dedicated because mindset is different from deep records. Cross-link to Profile Timeline.
**Real text:** “12-day scan streak — you’re in the top 8% of owners. BCS improved 1.3 points in 6 weeks.”

### 4. Horse Profile (Deep timeline + records)
**Why:** Long-term data moat and single source of truth. Enables team sharing with vet/trainer.
**Useful?** Critical for history, documents (Coggins, insurance), multi-user access.
**Simplify:** Timeline is the hero. Documents, Team, Goals as secondary segments. No need to duplicate graphs (link to Progress).
**Real text:** “Aug 18 • AI Scan • BCS 5.2 • 94% confidence • Weight est. 1,120 lbs”

### 5. Community (Feed)
**Why:** Existing millions of posts + viral flywheel. Network effects.
**Useful?** Retention + acquisition via shares.
**Simplify:** Create Post is always a modal/composer (pre-filled from scan for maximum virality). Never replace the feed.

### 6. Marketplace
**Why:** Utility (find farrier/vet when the app tells you it’s due) + side revenue.
**Useful?** Yes, especially soft-entry from Home alerts. Less critical as pure browsing.
**Simplify:** Start lean (list + detail). Deep booking can come later.
**Real text soft entry:** “Farrier due in 4 days — 3 highly rated professionals within 8 miles.”

### 7. Profile Tab container
Holds: Horse list / switcher, Settings, Subscription management, Notification preferences, Account.

### Demoted / Modal / Combined (Cal AI reduction)
- **Full Care Calendar** → Demoted. “Upcoming Care” cards live on Home. Full month view optional secondary inside Profile if needed. Most owners prefer smart lists + notifications over calendar grids.
- **Daily Observation / Quick Log** → Bottom sheet / modal from FAB only. Chips + voice + optional photo. <10 seconds. Never a full tab.
- **Nutrition Plan** → Section inside Scan Results or Profile. One-tap “Log as fed” is the high-value action.
- **Vet Share Report** → Generated share sheet / PDF, not persistent screen.
- **Multi-Horse Dashboard** → Adaptive state of Home when user has >1 horse.
- **Soft Upgrade Gate** → Overlay or full-screen card at the exact moment free scans are exhausted.
- **Guided Scan / Onboarding / Paywall** → Full-screen flows (tab bar intentionally hidden).

## Resulting Structure
5 tabs stay rock solid. Home does more work. FAB is the universal Scan/Log entry. Profile holds depth + settings. Far fewer full screens = higher speed perception and AAA polish.

## Next Steps
1. Regenerate every key mockup with the exact locked Tab Bar text above.
2. Use only real horse-owner language in all UI text.
3. A/B the paywall and onboarding hard.
4. Ship the core loop first: Home → FAB Scan → Results → Streak → Share.

All decisions flow from: Cal AI ease + real horse owner needs + honest AI + perfect visual consistency.
