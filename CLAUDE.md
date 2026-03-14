# Amici Pitch Deck — Context for Claude

## What is Amici

Amici is a Swedish pre-seed startup building an event platform for mid-market companies (20-500 employees) that don't have dedicated event staff. The platform lets companies describe an event, get matched with verified suppliers (chefs, venues, transport, equipment), and receive coordinated offers in one place.

## Current stage

- Part-time founding team of 4: Carol (CEO), Anders (Chef/Co-founder), Daniel (Product & Design), Edin (Engineering)
- ~20 events delivered through manual concierge operations (chef bookings for Hermès, Prada, Sail Racing, Chimi)
- V2 platform live with user accounts, event management, transaction messaging
- Raising 5M SEK pre-seed to go full-time and build the multi-service marketplace

## Business model

- Amici charges suppliers a 20% commission (supplier-side, not customer-side)
- The customer sees transparent, direct pricing with no markup
- This is a key differentiator from agencies who charge the customer 15-20% on total cost
- Future revenue streams: concierge services (white-glove add-on), supplier SaaS tools, supplier kickbacks on volume

## Key narrative decisions

- Traction is framed as "we ran events by hand on purpose" — deliberate customer discovery, not a pivot
- The manual concierge phase validated demand, buyer profile, and founder-market fit
- Amici targets companies that would never hire an agency — a different tier of the market, not competing with agencies directly
- The competitive advantage is multi-service orchestration (coordinating the whole event), not just matching a single supplier

## Market data sources

- 9.1% CAGR: Sweden's event market, fastest-growing in Europe. Source: Allied Market Research, Europe Events Industry Forecast 2021-2030
- 8.7% CAGR: European corporate events market overall. Same source
- 7.2B SEK TAM: Bottom-up math — 30K companies × 4 events/year × 60K SEK avg. spend
- 30K+ companies: SCB (Statistics Sweden) company registry, companies with 20-500 employees

## Technical notes for the deck

- Single self-contained HTML file — all CSS, JS, and content in one file
- Dark theme, blue accent (#3B82F6), green for market/business model slides (#22C55E)
- Slide navigation via keyboard arrows, click dots, or swipe
- Responsive with breakpoints at 1280px, 900px, and 600px
- Staggered fade-up animations on slide transitions
- Two product mockups on the Vision slide: mobile phone frame (event organizer view) and desktop browser frame (supplier dashboard)

## When editing this deck

- Always ask before making changes to files
- Preserve the existing visual design system (colors, typography, spacing, animations)
- Follow pitch-copy best practices: no em dashes, no buzzwords, assertion headlines, human tone
- Source any market claims with credible data
- The deck is deployed to Vercel via GitHub — changes to main auto-deploy
- After every decision or direction change agreed with the user, update the "Decision log" section below with what was decided and why

## Decision log

- **2026-03-09:** Replaced the duplicate "15-20% agency markup" card on the Why Now slide with a digitization gap card. Stat: #3 from bottom in digitization. Source: McKinsey Global Institute, Industry Digitization Index. Reason: the agency markup was already shown on the Problem slide.
- **2026-03-09:** Refined the third Why Now card from "0 platforms that do this" to "0 digital alternatives to agencies." Reframed to acknowledge single-service platforms and agencies exist, but highlight the gap: no platform combines multi-service orchestration with digital delivery. Positions Amici as the "digital event agency" without using that phrase.
- **2026-03-09:** Added decision log rule to CLAUDE.md. Every decision or direction change agreed with the user must be appended here so future sessions inherit full context.
- **2026-03-09:** Repositioned Amici as a "digital event agency" throughout the deck. Updated cover subtitle, insights quote, business model headline ("Commission today. Scale tomorrow."), competitive landscape, Ask roadmap, and traction step 4 to use "digital event agency" language consistently.
- **2026-03-09:** Removed exact revenue/income numbers from the deck. Removed ~50K SEK/month booking value from traction stats and business model slide. Changed "Revenue growing" to "Demand growing" on the Ask slide. Kept 20% commission rate on business model slide (describes the model, not revenue).
- **2026-03-09:** Overhauled traction slide timeline to tell the founder journey: (1) consumer app for chef bookings, (2) pivot to B2B with V2 platform, (3) crossroads — become supplier or build the orchestrator customers keep asking for, (4) next steps. Moved brand names (Hermès, Prada, Sail Racing, Chimi) to the right side panel as a subtle "Trusted by" list, replacing the old stats. Kept ~20 events delivered as the one remaining metric.
- **2026-03-09:** Removed EventLogic from competitive landscape slide. Simplified to 4 columns: DIY → Single platforms → Amici → Traditional agencies. Reframed Amici as the more accessible, powerful digital alternative to traditional event firms. Updated moat text to explain why Amici beats traditional agencies.
- **2026-03-13:** Removed Airbnb reference, customer service fee, and ~50K SEK/month booking volume from Business Model slide (slide 10, data-slide="9"). Kept only the 20% supplier commission. Customer service fee may be added in the future but isn't live yet. Note: slide numbers in this log refer to the UI indicator at the bottom of the deck, not the data-slide attribute.
- **2026-03-13:** Trimmed Competitive Landscape slide (slide 11) boxes to max ~3 lines each, focusing on market positioning not pricing. Reframed Amici box from "built for companies that would never hire an agency" to "agency power without the agency price tag" — Amici pulls from both ends of the spectrum (DIY/single-platform users moving up, and potential agency customers moving down).
- **2026-03-14:** Strategic overhaul of product positioning. Amici is a "supplier network and matching platform," not a "digital event agency." Amici never coordinates events. Coordination responsibility sits with the customer (self-service) or a professional event coordinator (add-on). Replaced all "digital event agency" and "orchestrate" language throughout the deck.
- **2026-03-14:** Added customer user flow slide (slide 9) showing the two paths: simple events (supplier contacts customer directly) and complex events (platform recommends event coordinator add-on). When coordinator is booked, Amici guarantees coherent experience. When declined, customer self-coordinates with no coherence guarantee from Amici.
- **2026-03-14:** Added "Agencies sell human hours. Amici sells software and network effects." as the key competitive framing on the business model and competitive landscape slides. This is the core scalability argument for investors.
- **2026-03-14:** Clarified supplier offer flow: suppliers respond to Amici, Amici packages and presents offers to customer. Customer does not interact with suppliers during the matching phase.
- **2026-03-14:** Event coordinators are not a marketplace. They are professionals Amici collaborates with explicitly. This is a curated relationship, not an open marketplace.
- **2026-03-14:** Traditional agencies are positioned as the main competitor. The competitive advantage is structural: platform economics vs. labor economics.
- **2026-03-14:** Kept the "supplier engine" vision slide (now slide 7, data-slide="6") but broadened it. Changed "agencies can plug into" to "anyone can plug into." Changed "coordination" to "matching" and made the potential audience more open-ended (agencies, other platforms, corporate tools).
- **2026-03-14:** Merged Why Now cards #2 (digitization gap) and #3 (zero digital alternatives) into one card. They made the same point. Added new third card: "The tech to match suppliers at scale finally exists" (10x cheaper to build today). Stat-label: CHEAPER TO BUILD TODAY.
- **2026-03-14:** Shortened traction slide timeline titles: "Started with chef bookings", "Pivoted to B2B", "Supplier or platform?", "Now: concierge to platform". Design rule: no title should have exactly one word on the second line (must be 0 or 2+ words wrapping).
- **2026-03-14:** Changed "Most events need more than one supplier" to "Many events" on the Insights slide. Too bold a claim without data.
- **2026-03-14:** Removed standalone How It Works slide (was too complex). Integrated a 5-step flow into the Product slide instead: (1) Describe your event, (2) We match suppliers, (3) Review offers, (4) Book and pay, (5) Want coordination? Step 5 uses amber styling as a decision point. The split is about whether the user wants coordination, not about event complexity.
- **2026-03-14:** Reordered slides. New order: Cover, Problem, Why Now, Traction, Insights, Product, Competitive Landscape, Vision (mockups), Vision (supplier engine), Market, Business Model, Team, The Ask. Rationale: product and competitive positioning right after insights (concrete before visionary). Vision slides expand on where the company is going after establishing what it does and how it's different. Deck is now 13 slides.
