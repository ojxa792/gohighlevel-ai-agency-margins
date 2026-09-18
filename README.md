# gohighlevel ai for agencies: what to resell, what it costs, and how to keep margin on every sub-account

Search "GoHighLevel AI for agencies" and you get two very different questions mixed into one box. Half the people typing it want to know which AI to switch on inside their own sub-accounts. The other half are trying to figure out what they can package, price, and rebill to clients without the margin evaporating the moment usage spikes.

Both questions land in the same place: the math. Native AI inside GoHighLevel is priced per location. Third-party conversational AI is usually priced per message. Those two models behave very differently once you pass your fourth client, and that difference decides whether AI becomes a revenue line or an expense you apologise for.

## What agencies are actually selling when they sell "GoHighLevel AI"

Strip the branding away and there are three distinct things agencies hand to clients and call "AI":

1. **Conversation AI** — the text layer. SMS, web chat, and the other text channels inside a sub-account's Conversations inbox. It replies, qualifies, and in good setups books straight to a calendar.
2. **Voice AI** — inbound and outbound call handling, receptionist duty, call routing.
3. **Agent tooling** — reply drafts, review responses, content generation, workflow assistants. Useful, but rarely the thing the client is actually paying a retainer for.

Only one of these is the reason clients sign. Clients don't renew because an AI wrote their review reply. They renew because leads that used to go cold at 9pm got answered and booked. So the decision that matters is which conversation layer sits under your offer, and what it costs you per location and per message.

## The native route: what HighLevel's own AI costs per location

HighLevel's AI products sit under three billing modes, and the current published numbers are the ones worth quoting to clients.

| Native AI plan | Price | What's included |
| --- | --- | --- |
| Pay-as-you-go | Token cost only, no monthly fee | Conversation AI, Voice AI, Reviews AI, Content AI billed per token, minute, review or image |
| AI Employee Growth | $50/month per enabled location | 1,000 Conversation AI responses, 100 Voice AI minutes, unlimited Reviews AI and Content AI, 100 Voice AI Prompt Optimizer minutes |
| AI Employee Unlimited | $97/month per enabled location | Unlimited Conversation AI, Voice AI, Reviews AI, Content AI and Prompt Optimizer usage, subject to fair use |

Two details in that table are easy to miss and expensive to miss.

**Agent Studio is not included in any plan.** It stays pay-per-use across Pay-as-you-go, Growth, and Unlimited. If your offer depends on agent workflows rather than conversation, the subscription doesn't cover it.

**Rebilling AI Employee usage requires the $497/month agency plan.** Agencies below that tier can still use the AI, but the billing plumbing for passing AI costs to clients in a structured way isn't there.

The per-location model is clean, predictable, and completely reasonable for an agency running AI on its own pipeline. It gets awkward when you're the one holding the invoice. Ten sub-accounts on AI Employee Unlimited is $970 a month before a single SMS charge, and that number doesn't shrink when a client goes quiet for three months. Your wholesale cost is tied to the number of locations you manage, not to how much value the AI actually delivered.

## The bolt-on route: a dedicated conversational AI layer on top of GHL

This is where most "GoHighLevel AI for agencies" searches end up, because the native option stalls somewhere between "good enough for a demo" and "this is my whole product".

CloseBot is the layer agencies most often put on top of a sub-account. It connects natively to HighLevel through an OAuth flow — open Sources, add a source, choose HighLevel Sub-Account, approve the app permissions, pick the sub-account. No developers, no webhook wiring by hand. HubSpot and custom CRMs are supported the same way.

What you actually get on top of the native text AI:

- **Objective-driven job flows on a drag-and-drop canvas.** Instead of one large prompt, you build a flow with nodes — qualify, branch, answer, book. Branching matters: a med spa asking about Botox and one asking about laser hair removal shouldn't run through the same five sentences.
- **Personas that are separate from the agent.** Tone, timing, message splitting, even a deliberate typo can live in the persona and be reused across every client, with variables like `{industry}` or `{company_name}` swapped per sub-account. Build it once, redeploy it for a plumber and a realtor.
- **Text channels beyond SMS**, including email, plus the ability to read images a lead sends.
- **Multiple AI providers with automatic fallback.** If your primary model degrades, the agent routes to your next preference instead of going dark.
- **Smart FAQ.** When the agent hits a question it can't answer confidently, it flags it instead of inventing one. You answer once and CloseBot follows up with every lead who asked.
- **Testing portal and rollback.** Test conversations in-flow before going live, pause the AI on a single conversation for human takeover.

That last group is the unglamorous half of the product, and it's the half that keeps clients from firing you over a hallucinated discount.

> Worth being blunt about the limits: CloseBot itself does not connect to Instagram or WhatsApp. It answers whatever text channels your CRM already has connected, which for GoHighLevel means Instagram DMs and WhatsApp work only if they're already flowing into the Conversations inbox. Comment-to-DM triggers and story-reply funnels stay in your CRM or a separate flow tool.

## CloseBot pricing, plan by plan

Straight from the current plans page, at the time of writing:

| Plan | Price | Billing cycle | What it includes | Get it |
| --- | --- | --- | --- | --- |
| Free | $0 | Always free | 100 messages/month, 1 agent, 1 user seat, 1 MB storage, unlimited account connections | [Start on the free plan](https://app.closebot.com/a?fpr=li87) |
| Core — Business | $64/month ($53/month equivalent billed annually as $640/year) | Monthly or annual, cancel anytime | 500 messages/month included with message costs inside the base price, 15+ templates (50+ extra on annual), human support, extra users at $5/seat, add-on storage and agents | [See the business plans](https://app.closebot.com/a?fpr=li87) |
| Core — Agency | $397/month ($331/month equivalent on annual billing) | Monthly or annual, cancel anytime | Unlimited messages at $0.012/message, all of it rebillable, white-label client portal, re-bill seats and storage, 15+ templates, extra users at $5/seat | [Open the agency plan](https://app.closebot.com/a?fpr=li87) |
| Growth | Custom | Quoted | HIPAA compliance, quarterly audits, 99.99% priority uptime, priority support, 50+ templates, high volume | [Request a Growth quote](https://app.closebot.com/a?fpr=li87) |

Every paid plan carries a 7-day trial, and there are no refunds — which is exactly why the free plan and the trial exist. Test there, not on a support ticket afterwards.

There's one published coupon: `CLOSEBOT100OFF`. CloseBot lists it on its own blog as the only code the company maintains, and says it takes $100 off your first payment on Business and Agency plans. Third-party coupon sites advertising 60% off or "$350 off" are aggregator noise; the vendor explicitly says codes from outside that page can't be guaranteed at checkout.

One more structural note on the message counter: on the business track you can raise the monthly message ceiling, and the price rises with it — the slider runs from 500 up past 100,000, with better bulk rates the higher you go. That's the tier where "just start at $64" turns into a real forecasting exercise.

## The margin math: what rebilling actually returns

Here's the part that decides whether the Agency plan pays for itself, using plainly stated assumptions.

Say you run 10 clients, each generating 300 AI-handled messages a month.

- CloseBot wholesale message cost: 3,000 × $0.012 = **$36**
- Agency plan base: **$397**
- Total wholesale: **$433/month**

Now the revenue side. CloseBot's own plans page states that, based on its polled agencies, the average billing is around $500 per client per month. Ten clients at that average is **$5,000/month** in agency revenue against roughly $433 in wholesale AI cost. Even at a fifth of that billing — $100 per client, which CloseBot itself cites as the low end — you're at $1,000 against $433.

GoHighLevel's native AI Employee model produces a different shape. Ten locations on AI Employee Unlimited is $970/month in wholesale cost before SMS, and that cost is fixed regardless of how much conversation each client actually had.

The Agency plan also lets you markup far more than messages. Seats are billed to you at $5/month per user and can be rebilled at whatever you set — CloseBot's own documentation shows an example of rebilling a seat at $100. Storage is billed at $0.006 per MB per day and rebillable, which means the client uploading their own knowledge base files increases your revenue rather than eating it. Payment runs through Stripe Connect, so your clients top up their wallets and that money pays you directly.

Read the numbers honestly, though: the spread only exists if you actually sell the service. A software subscription doesn't create the offer for you.

## What agencies are packaging and charging

The offer shapes that show up repeatedly in case studies are boring in a good way:

- **Speed to lead.** Answer in seconds, qualify, book. The pitch is lost leads, not AI.
- **After-hours coverage.** Nights, weekends, holidays. Easy to quantify for home services and healthcare.
- **Dead lead reactivation.** Cheapest to sell because the leads already exist and nobody has to spend on ads. CloseBot's published case study has Eric McAvoy adding roughly $1,000 in MRR in 10 days off $1 of ad spend reactivating dormant leads.
- **Done-for-you agent builds.** Nick Tan's agency sells CloseBot V2 builds at $5,000 for setup and $500/month ongoing — that's the purest form of "the AI is the product".

Vertical matters more than feature count here. Real estate, home services, dental and med spa, coaching, and gyms all behave differently enough that a generic "AI chatbot" pitch reads as a commodity. A build that knows to check drive time before proposing an appointment slot does not.

## Where GoHighLevel AI projects go wrong

Three failure modes come up again and again in agency discussions, and none of them are about model quality.

**Thin margins from metered billing.** Native Conversation AI on pay-as-you-go is token-billed, which means you can't quote a client a fixed price per conversation without either padding it heavily or eating the variance. A flat per-message cost is easier to explain and easier to mark up.

**Knowledge bases nobody updates.** Every independent review of AI setters lands on the same point: inaccurate knowledge produces wrong answers, and wrong answers cost clients money. Smart FAQ exists precisely because the alternative — an agent confidently inventing a discount — is the fastest way to lose an account.

**Overselling what AI closes.** It qualifies, follows up, and books. It does not negotiate a six-figure deal or draft a custom proposal. An agency that implies otherwise gets blamed when the calendar fills with calls that never close.

And it's fair to note that sentiment isn't unanimous. In r/gohighlevel threads comparing the two, one two-year user described the tool as great when it works but unreliable enough that they were shopping for alternatives, and another reported the agent inventing details. CloseBot's own CEO replies in those threads, which is more engagement than most vendors manage. Meanwhile the public review picture is favourable: 4.8 stars from 191 reviews on G2. Vendors quote their best numbers; review platforms quote everyone's. Weigh both.

One structural limitation also worth knowing before you build a business on it: CloseBot doesn't offer bring-your-own API keys, which the company frames as a security decision. You can't swap in a cheaper model key to cut your own costs.

## How to pick a lane

If you're running AI on your **own** pipeline and your costs are predictable, native HighLevel AI is genuinely fine. Start on Pay-as-you-go, watch actual token spend for a month, then move to Growth or Unlimited if the numbers justify it.

If AI is the **product** you sell — multiple clients, white-label, rebilling, margin you control — the native per-location model starts working against you around client four. That's the point where a dedicated conversational layer with a flat, rebillable per-message cost stops being a nice-to-have.

A practical sequence that doesn't require committing blind:

1. Sign up free and connect one real sub-account. 100 messages a month is enough to run an agent against live leads and see whether it books.
2. Build the flow for your highest-volume niche, not a hypothetical one.
3. Watch where the agent asks for help. Those transcripts are your knowledge base gaps and your sales demo.
4. Only then decide between a business plan and the Agency plan — the 7-day trial on either covers the decision.

👉 [Open a free CloseBot account and test it against a live sub-account](https://app.closebot.com/a?fpr=li87)

## FAQ

**Is GoHighLevel's built-in AI enough for an agency?**
For your own pipeline, often yes. For rebilling AI as a product to multiple clients, the per-location pricing ($50 or $97/month per enabled location) plus the $497/month plan requirement for rebilling tends to hurt margin as you scale.

**How much does CloseBot cost for an agency?**
$397/month monthly or $331/month equivalent on annual billing, with unlimited messages rebilled at $0.012 each. Seats are $5 to you and rebillable at your own rate; storage is $0.006 per MB per day.

**Does CloseBot work with GoHighLevel without developers?**
Yes. Connection is an OAuth flow from the Sources page. Independent reviews put initial configuration at around 5–10 hours for knowledge bases and flows; CloseBot claims most teams get a first agent live the same day.

**Can I use CloseBot for Instagram DMs?**
Only through your CRM. If Instagram is already connected to your GoHighLevel Conversations inbox, the agent can answer those DMs. CloseBot has no native Instagram or WhatsApp connection of its own.

**Is there a real CloseBot discount code?**
Yes — `CLOSEBOT100OFF`, listed on CloseBot's own site as the only code the company maintains, taking $100 off the first payment on Business and Agency plans. Codes on coupon aggregators aren't guaranteed.

**Can I get a refund if it doesn't work out?**
No. CloseBot doesn't issue refunds. The free plan and the 7-day trial on paid plans are the risk-free window — use them for the actual decision.
