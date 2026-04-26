# Presentation Script — Daniel

Slides 4–9 and 13 | Practice version | English

---

## Slide 4: Traction

Before we built anything, we ran events by hand. On purpose.

Carol and Anders were already connected to some of the best chefs in Sweden. So we started there: matching companies with chefs through their existing network. No marketing spend, zero paid acquisition. Every booking came through word of mouth.

And the clients were not small. Hermès, Prada, Sail Racing, Chimi. These are companies with high standards. They chose us because we delivered.

But what we kept hearing was: "Can you do more than just the chef?" Every single client wanted a venue. Then transport. Then something else. They didn't want a chef booking. They wanted their whole event taken care of.

That told us what to build. So we built it. A platform with the first three supplier categories in one digital flow: chef, venue, rentals. Authentication, admin tools, payments included.

And now we're at the next step: building the tool customers have been asking for. A full-time team lets us run the product, the partnerships, and the sales effort in parallel.

---

## Slide 5: Insights

Every event we ran taught us the same thing about the buyer.

They're not event professionals. They're the office manager, the HR lead, the assistant who got handed this. No supplier network. No reference point for pricing. They Google, ask around, and hope for the best.

And when they came to us for a chef, they always wanted more. First the chef, then the venue, then transport. Every time, the need expanded beyond a single service. That's not a coincidence. That's the shape of the market.

The third thing is the one that actually makes this a business: they come back. And when they do, they start from zero again. No institutional memory. No sense of whether the price is fair. The next event resets completely.

That's why a platform matters. Not just to make the first booking easier. But to capture the repeat cycle, build the supplier relationships, and give buyers a reference frame they can trust.

One customer said it best: not "can you find a chef?" but "can you handle the whole thing?" That's what we built Amici to answer.

---

## Slide 6: Product Vision — The Flow

So here's how Amici works.

You describe your event. Number of guests, format, date. The platform matches you against verified suppliers and shows you prices right away. Not in 24 hours. Not after a round of quote requests. Right away.

You adjust inputs, and the total updates live. More guests, different date, different format: the price updates as you go. When you're ready, you book.

After booking, you have a choice. If you want someone to handle the supplier logistics for you, you add a coordinator. That's a professional who manages everything. If you'd rather handle it yourself, you do that through the platform directly.

And here's something we built that investors consistently react to: once you've run an event, you can recreate it. Book from the same suppliers, keep what worked, swap out what didn't. The platform remembers, even when you don't.

What used to take 7 to 14 days of active work, spread across weeks of waiting, now takes minutes.

---

## Slide 7: Product Vision — All Suppliers, One Place

This is what the customer sees.

You describe the event. The platform pulls from our verified supplier network and shows you pre-negotiated prices right away. You're not waiting for suppliers to respond. We've done that work in advance.

The left side is the customer view on mobile. The right side is what the supplier sees in their dashboard.

No back-and-forth. No emailing five venues and hoping someone replies. The pricing is there. You adjust, you book.

---

## Slide 8: Product Vision — The Supplier Engine

Here's where this gets interesting for investors.

As the supplier network grows, it becomes infrastructure. Any platform, any agency, any corporate tool that needs to connect people with event suppliers can plug into Amici through an API or an embed.

The chef network, the venues, the transport providers, the equipment rental, the staff: all of it accessible through one integration.

We're not just building a booking tool. We're building the layer that sits underneath the event industry's supply side. That's a very different company.

---

## Slide 9: Competitive Landscape

The market has two ends. On the left, you do it yourself: Google, phone calls, spreadsheets, hours of coordination. It's free but it's painful.

On the right, you hire a traditional agency. Full service, professionally managed, and priced accordingly. Built for companies with big event budgets and dedicated procurement teams.

In the middle there are single-service platforms. You can book a venue on one, a caterer on another. But you're still juggling four different vendors and no one is accountable for the whole thing.

Amici sits between single platforms and traditional agencies. All your suppliers, one platform. Add a coordinator if you need one.

The reason agencies can't respond to this: they sell hours. Every event they run costs more staff time. Amici sells software and network effects. Every event we facilitate runs on the same platform at near-zero marginal cost. That's why the unit economics look completely different.

---

## Slide 13: The Platform

I want to give you a concrete sense of what Edin built, because it directly affects how capital-efficient we are.

The platform is a monorepo. One codebase. Four separate applications: the customer platform, the supplier portal, the admin dashboard, and the marketing site. They share code, configuration, and types.

84 shared components across those four apps. Change a button in one place, it updates everywhere. New supplier categories plug in without rebuilding the core.

39 versioned database migrations. An automated deployment pipeline. Type-safe from the database all the way up to the UI.

Most startups accumulate technical debt from day one. Edin architected this from the ground up to avoid it. That means faster iteration, lower burn, and lower risk for you as an investor. Four people built this. Imagine what a funded team does with it.

---

## Notes for practice

- **Slide 5 (Insights):** the customer quote is your landing moment. Pause before it.
- **Slide 6 (Flow):** walk through the steps slowly, investors need to visualize the UX.
- **Slide 9 (Competitive):** the "agencies sell hours / Amici sells software" line is your sharpest point. Deliver it cleanly and let it land before moving on.
- **Slide 13 (Platform):** if Edin is in the room, you can hand him this slide. If not, lead with the business implication ("capital-efficient") not the technical architecture.
