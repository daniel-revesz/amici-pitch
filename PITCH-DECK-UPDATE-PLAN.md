# Pitch Deck Update Plan: Product Direction Overhaul

This document is a detailed handoff for updating the Amici investor pitch deck (index.html). It captures all strategic decisions, copy changes, and a new slide to build. Read this fully before making any changes.

---

## Strategic context: what changed and why

Through a product strategy session, we clarified how Amici actually works as a business. The deck currently uses language like "digital event agency," "orchestrate," and "the platform coordinates everything." These imply Amici does the coordination work. It doesn't. The updated model is clearer and more scalable:

**Amici is a supplier network and matching platform that makes simple events fully self-service and complex events manageable.**

The core insight for investors: **Agencies sell human hours. Amici sells software and network effects.** Every event an agency runs requires proportionally more staff time. Every event Amici facilitates runs on the same platform with near-zero marginal cost, because the coordination burden sits with the customer or with a coordinator supplier, never with Amici.

---

## The product model (how Amici actually works)

### Supplier matching flow
1. Customer describes their event on Amici
2. Amici matches the request with relevant suppliers from its network
3. Suppliers respond with offers to Amici (not directly to the customer)
4. Amici packages and presents the full event proposal to the customer as one coherent offering
5. Customer reviews, compares, and books

### Coordination responsibility
Amici never coordinates. Period. The responsibility sits with either:
- **The customer** (who self-coordinates when they decline a coordinator), or
- **A professional event coordinator** (booked as an add-on through Amici)

From each supplier's perspective, their point of contact is always the customer (or the coordinator if one is booked).

### The event coordinator add-on
For complex, multi-supplier events with dependencies (e.g., chef + external venue + transport), Amici's platform smartly recommends adding a professional event coordinator. This is not a marketplace of random coordinators. These are coordinators Amici collaborates with explicitly.

- **If the customer accepts the coordinator:** The coordinator manages logistics between suppliers. Amici can guarantee a coherent event experience.
- **If the customer declines the coordinator:** The customer becomes the point of contact for all suppliers and coordinates them directly. Amici does not guarantee a coherent event experience. Each supplier delivers their part independently.

### Three service tiers

**Tier 1: Single supplier (e.g., chef for a company dinner)**
Fully self-service. Customer books, supplier delivers. Supplier contacts customer directly for any questions. No coordination needed.
Amici's role: matching, offer presentation, payment.

**Tier 2: Multi-supplier, low dependency (e.g., chef + photographer at customer's own office)**
Self-service with platform-provided logistics info. Suppliers each contact the customer independently. The platform shares basic event details to all booked suppliers (date, time, location, guest count). The customer handles any alignment needed.
Amici's role: matching, offer presentation, payment, shared event brief.

**Tier 3: Multi-supplier, high dependency (e.g., chef + venue + transport + equipment)**
Platform recommends an event coordinator add-on. If the customer accepts: the coordinator becomes their logistics point of contact for all suppliers, and Amici guarantees a coherent event experience. If the customer declines: they take on coordination responsibility themselves, suppliers contact the customer directly, and Amici does not guarantee a coherent event experience.
Amici's role: matching, offer presentation, payment, smart coordinator recommendation, optional coordinator add-on.

### Competitive framing
Traditional agencies are the main competitor. The framing should position agencies as the incumbent that can't scale, and Amici as the platform that can. Agencies sell hours. Amici sells software. This is the key line for investors.

---

## Current deck structure (13 slides)

For reference, the current slides are:

| Slide # (UI) | data-slide | Section | Headline |
|---|---|---|---|
| 1 | 0 | Cover | Company events, without the chaos |
| 2 | 1 | Problem | "Can you organize something nice for 40 people?" |
| 3 | 2 | Why Now | Event spend is booming. The tools haven't caught up. |
| 4 | 3 | Traction | We ran events by hand. On purpose. |
| 5 | 4 | Insights | What running events taught us |
| 6 | 5 | Vision | One tool to orchestrate it all |
| 7 | 6 | Vision | A supplier engine agencies can plug into |
| 8 | 7 | Product | What takes hours today takes minutes with Amici |
| 9 | 8 | Market | Big market. Focused start. |
| 10 | 9 | Business Model | Commission today. Scale tomorrow. |
| 11 | 10 | Competitive Landscape | The sweet spot nobody owns |
| 12 | 11 | Team | We know this industry from the inside |
| 13 | 12 | The Ask | From side project to full-time company |

---

## Changes to make

### NEW SLIDE: Customer User Flow (insert after current slide 8/Product, as new slide 9)

This is the biggest addition. Create a new slide that shows the customer journey as a visual flow diagram using HTML/CSS boxes and arrows. It should follow the deck's existing design system (dark theme, blue accent #3B82F6, same fonts, card styles, stagger animations).

**The flow to visualize:**

```
[Customer describes event]
        ↓
[Amici matches suppliers from network]
        ↓
[Suppliers submit offers to Amici]
        ↓
[Amici presents packaged event proposal]
        ↓
[Customer reviews and books]
        ↓
    ◇ Decision point: Does this event need coordination?
   /                          \
  /                            \
[Path A: Simple]          [Path B: Complex]
Single supplier or         Multiple suppliers
low dependency             with dependencies
     ↓                         ↓
Supplier contacts         Platform recommends
customer directly         event coordinator add-on
     ↓                    /                    \
Event delivered     [Customer accepts]    [Customer declines]
                         ↓                      ↓
                   Coordinator manages     Customer self-coordinates
                   logistics between       with suppliers directly
                   all suppliers                ↓
                         ↓                 Event delivered
                   Amici guarantees        (no coherence guarantee)
                   coherent experience
                         ↓
                   Event delivered
```

**Design notes for this slide:**
- Section label: "How It Works" or "Customer Journey"
- Headline: Something like "One flow. Two paths." or "Simple events run themselves. Complex ones get a coordinator." (follow pitch-copy skill guidelines: assertion headline, no buzzwords, no em dashes)
- Use the existing card styling for boxes
- Use blue accent for the Amici-controlled steps
- Use a different visual treatment (perhaps green #22C55E or a subtle border change) for the coordinator path vs. the self-service path
- The decision point (diamond) should be visually distinct
- Keep it clean and readable. This is a pitch deck, not a technical spec. The diagram should be immediately understandable

**Important:** After inserting this new slide, all subsequent slide numbers shift by 1. Update the data-slide attributes accordingly and update the slide counter in the nav.

---

### SLIDE 1 (Cover, data-slide="0"): Update subtitle

**Current:** "The digital event agency for businesses without an event team. One tool to book chefs, venues, transport, and equipment."

**Change to:** Replace "digital event agency" with "event platform." The word "agency" implies Amici does the work. We want to position against agencies, not as one.

**New:** "The event platform for businesses without an event team. One tool to book chefs, venues, transport, and equipment."

---

### SLIDE 4 (Traction, data-slide="3"): Update timeline step 4

**Current text in timeline step 4:** "Expanding beyond chefs into a full digital event agency. This raise funds the transition from concierge to platform."

**Change to:** Remove "digital event agency" language. Reframe around the platform model. Something like: "Expanding beyond chefs into a multi-service event platform. This raise funds the transition from concierge to platform."

---

### SLIDE 5 (Insights, data-slide="4"): Update quote block

**Current quote:** "The real value isn't matching a single supplier to a client. It's coordinating the entire event."

**Current subtext:** "That's what nobody else is doing for the mid-market. This is why we're building a multi-service platform, not another single-vendor marketplace."

**Issue:** The quote says "coordinating the entire event" which implies Amici coordinates. The subtext is actually fine.

**Change to:** Adjust the quote to reflect that the value is in bringing all the pieces together in one place for the customer, not in Amici doing the coordination. Something like: "The real value isn't matching a single supplier. It's bringing the entire event together in one place." Keep the subtext as is.

---

### SLIDE 6 (Vision, data-slide="5"): Update headline and subheadline

**Current headline:** "One tool to orchestrate it all"
**Current subheadline:** "Describe your event. The platform identifies what you need, drafts requests to verified suppliers, and lets you compare offers, all in one place."

**Issues:**
- "Orchestrate" implies Amici does the coordination.
- "Drafts requests to verified suppliers" is okay but doesn't reflect that Amici packages and presents offers.

**Change headline to:** Something that conveys the matching and packaging value without implying coordination. E.g., "One tool to plan it all" or "Every supplier. One place." or "Describe your event. We handle the rest." (though that last one also implies doing the work, so be careful).

**Change subheadline to:** Reflect the actual flow: customer describes event, Amici matches suppliers, suppliers respond to Amici, Amici presents a packaged proposal. E.g., "Describe your event. We match you with verified suppliers, collect their offers, and present one clear proposal. You compare, book, and go."

---

### SLIDE 7 (Vision, data-slide="6"): Keep but make more open-ended

**Current headline:** "A supplier engine agencies can plug into"
**Current subheadline:** "As our supplier network grows, agencies and platforms can tap into it via API or embed our widget. The speed, quality, and coordination we build becomes infrastructure anyone can use."

**Decision:** Keep this slide. The idea that agencies and other platforms could eventually plug into Amici's supplier network is a valid long-term revenue stream and strengthens the network effects story. Agencies using your infrastructure would be a sign of platform dominance, not a contradiction with competing against them. Think Shopify powering competing stores.

**Changes needed:**
- Replace "coordination" with "matching" or "sourcing" to stay consistent with the rest of the deck.
- Make the framing more open-ended about who could plug in. Don't limit it to agencies. Other event platforms, corporate tools, HR platforms, etc. could all be consumers of the supplier network.
- Suggested subheadline direction: "As our supplier network grows, other platforms, agencies, and corporate tools can tap into it via API or embed. The matching and quality we build becomes infrastructure anyone can use."
- The headline could stay similar but broaden slightly. E.g., "A supplier engine anyone can plug into" or "A supplier network that becomes infrastructure."

---

### SLIDE 8 (Product, data-slide="7"): Update step 3 and bottom text

**Current step 3 title:** "Compare, book, done"
**Current step 3 description:** "Pick your favorites, confirm, and pay. The platform coordinates everything from there."

**Issue:** "The platform coordinates everything from there" is the single most problematic line in the deck. Amici does not coordinate.

**Change step 3 description to:** "Pick your favorites, confirm, and pay. For complex events, add a professional coordinator. For simple ones, you're good to go."

**Current bottom card text:** "You spend a few minutes describing your event. Suppliers respond with coordinated offers. No chasing quotes, no juggling vendors, no spreadsheet tracking."

**Issue:** "Coordinated offers" implies someone coordinated them.

**Change to:** "You spend a few minutes describing your event. We match you with the right suppliers and present their offers side by side. No chasing quotes, no juggling vendors, no spreadsheet tracking."

---

### SLIDE 10 (Business Model, data-slide="9"): Update "Later" card and add scalability framing

**Current "Later" card:** "Concierge tier: clients pay Amici to manage events end-to-end. Supplier SaaS: featured listings, analytics, priority matching. Plus supplier kickbacks on volume."

**Issue:** "Clients pay Amici to manage events end-to-end" contradicts the model where Amici never coordinates.

**Change "Later" card to:** Replace "Concierge tier" with the coordinator add-on and supplier tools. E.g.: "Event coordinator add-on: customers book professional coordinators through Amici for complex events (additional commission). Supplier SaaS: featured listings, analytics, priority matching. Plus supplier kickbacks on volume."

**Add the key investor line somewhere on this slide.** Consider adding it to the bottom card or as a new element: "Agencies sell human hours. Amici sells software and network effects." This is the single most important line for investors to understand the business model's scalability. It could replace or sit alongside the existing bottom metrics bar (CAC, Rev/event, 3-5x repeat).

---

### SLIDE 11 (Competitive Landscape, data-slide="10"): Update Amici box and bottom card

**Current Amici box text:** "Full orchestration, digital delivery. Agency power without the agency price tag."

**Issue:** "Full orchestration" implies Amici orchestrates. "Agency power" is closer to right but still implies agency-level service.

**Change Amici box to:** Something like "All your suppliers, one platform. With optional coordination for complex events." or "Multi-service matching with transparent pricing. Add a coordinator when you need one."

**Current bottom card:** "Why not just use a traditional agency? Agencies run on calls, emails, and enterprise budgets. Amici delivers the same orchestration through a modern digital flow, at a fraction of the cost."

**Change bottom card to:** This is where "Agencies sell human hours. Amici sells software and network effects." lands perfectly. Replace the current defensive framing with this offensive one. E.g.: "Why agencies can't compete: Agencies sell human hours. Every event they run costs more staff time. Amici sells software and network effects. Every event we facilitate runs on the same platform at near-zero marginal cost."

Alternatively, use this as the primary line and keep it punchy. The current framing ("Why not just use a traditional agency?") is a question the audience asks. The new framing ("Agencies sell hours. We sell software.") is the answer they remember.

---

### SLIDE 13 (The Ask, data-slide="12"): Update roadmap language

**Current Month 1-3:** "Go full-time. Expand booking flow to multi-service requests. Seal supplier deals. Build the digital event agency infrastructure. Stockholm focus."

**Change:** Replace "Build the digital event agency infrastructure" with "Build the multi-service matching platform." or "Build the supplier network and event coordinator partnerships."

**Current Month 4-6:** "Scale sales and marketing. Optimize multi-service orchestration. Build partnerships with large companies as their go-to digital event agency."

**Change:** Replace "multi-service orchestration" with "multi-service matching." Replace "as their go-to digital event agency" with "as their go-to event platform."

---

### SLIDE 3 (Why Now, data-slide="2"): Minor update to third card

**Current third card text:** "Single-service platforms digitized booking for venues or catering, one category at a time. Agencies coordinate the full event, but through calls and emails at a premium. No platform does both: multi-service orchestration, delivered digitally."

**Issue:** "Multi-service orchestration, delivered digitally" could imply Amici orchestrates.

**Change to:** "No platform does both: multi-service matching and coordination, delivered digitally." Or: "No platform brings all event suppliers into one digital flow." The nuance is that Amici's value is bringing suppliers together in one place and optionally providing coordination through the coordinator add-on, not orchestrating itself.

---

## What NOT to change

These slides are fine as-is and don't conflict with the new direction:

- **Slide 2 (Problem):** The problem framing is still accurate. Companies struggle with coordination, and that's exactly why Amici exists.
- **Slide 9 (Market):** Pure market data, no product claims.
- **Slide 12 (Team):** No changes needed.

---

## Summary of all changes

1. **New slide:** Customer user flow diagram (insert after slide 8, becomes new slide 9)
2. **Slide 1 (Cover):** "digital event agency" → "event platform"
3. **Slide 3 (Why Now):** "multi-service orchestration, delivered digitally" → softer language
4. **Slide 4 (Traction):** "full digital event agency" → "multi-service event platform"
5. **Slide 5 (Insights):** Update quote to not imply Amici coordinates
6. **Slide 6 (Vision):** "orchestrate" → different verb; update subheadline to reflect offer packaging flow
7. **Slide 7 (Vision/API):** Keep but broaden. Replace "coordination" with "matching/sourcing." Make the audience more open-ended (not just agencies: also other platforms, corporate tools, HR platforms)
8. **Slide 8 (Product):** "The platform coordinates everything" → reflect coordinator add-on model
9. **Slide 10 (Business Model):** "Concierge tier" → coordinator add-on; add "agencies sell hours, we sell software" line
10. **Slide 11 (Competitive):** "Full orchestration" → platform language; bottom card → "agencies sell hours" framing
11. **Slide 13 (The Ask):** "digital event agency" → "event platform" throughout roadmap

---

## Design system reference (for the new slide)

Use these existing CSS variables and patterns:
- Background: var(--bg-primary) #0A0A0B
- Card background: var(--bg-card) #131415
- Card hover: var(--bg-card-hover) #1a1b1d
- Border: rgba(255, 255, 255, 0.1)
- Blue accent: var(--accent) #3B82F6
- Green accent: var(--success) #22C55E
- Text primary: var(--text-primary) #F5F5F7
- Text secondary: rgba(255, 255, 255, 0.7)
- Text muted: var(--text-muted) #71717A
- Font display: var(--font-display) 'Quattrocento'
- Font body: var(--font-body) 'Quattrocento Sans'
- Font mono: var(--font-mono) 'Roboto Mono'
- Border radius: var(--radius) 24px, var(--radius-sm) 12px
- Slides use class="slide has-header" with .slide-header for section-label + headline + subheadline
- Content goes in .slide-inner
- Animations use class="stagger" for fade-up on slide entry
- The file is a single self-contained HTML file, all CSS/JS inline

---

## Decision log entries to add to CLAUDE.md

After making changes, append these to the decision log in CLAUDE.md:

- **2026-03-14:** Strategic overhaul of product positioning. Amici is a "supplier network and matching platform," not a "digital event agency." Amici never coordinates events. Coordination responsibility sits with the customer (self-service) or a professional event coordinator (add-on). Replaced all "digital event agency" and "orchestrate" language throughout the deck.
- **2026-03-14:** Added customer user flow slide showing the two paths: simple events (supplier contacts customer directly) and complex events (platform recommends event coordinator add-on). When coordinator is booked, Amici guarantees coherent experience. When declined, customer self-coordinates with no coherence guarantee from Amici.
- **2026-03-14:** Added "Agencies sell human hours. Amici sells software and network effects." as the key competitive framing on the business model and/or competitive landscape slides. This is the core scalability argument for investors.
- **2026-03-14:** Clarified supplier offer flow: suppliers respond to Amici, Amici packages and presents offers to customer. Customer does not interact with suppliers during the matching phase.
- **2026-03-14:** Event coordinators are not a marketplace. They are professionals Amici collaborates with explicitly. This is a curated relationship, not an open marketplace.
- **2026-03-14:** Traditional agencies are positioned as the main competitor. The competitive advantage is structural: platform economics vs. labor economics.
- **2026-03-14:** Kept the "supplier engine" vision slide (data-slide="6") but broadened it. The idea that agencies and other platforms could plug into Amici's supplier network is a valid long-term revenue stream that strengthens network effects. Changed "coordination" to "matching/sourcing" and made the potential audience more open-ended (agencies, other platforms, corporate tools, HR platforms).

---

## Open questions

None currently. All decisions have been made.
