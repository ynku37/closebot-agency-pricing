# ai appointment setting for agencies: what to run, what to charge, and what the stack really costs

Agencies search this phrase for two different reasons, and the confusion between them is where most of the bad pricing decisions come from.

Some are trying to sell AI appointment setting as a service — a done-for-you offer bolted onto an existing SMMA or marketing retainer. Others just want an agent answering and booking their own inbound leads so they stop paying a human setter to send "hey, just following up" texts at 9pm. Same keyword, two completely different budgets, two different answers.

CloseBot splits its own product along exactly that line: a business track for companies booking their own pipeline, and an agency track built around white-labeling and rebilling. That split is the single most useful thing to understand before you compare prices, because the tool is usually the smaller half of the bill.

## The bill is a stack, not a subscription

Every AI setter that plugs into a CRM inherits that CRM's cost, and that cost is not small.

CloseBot is CRM-native. It connects to HighLevel, HubSpot, LeadConnector, or a custom CRM, and then takes over the text-based channels inside that CRM — SMS, live chat, email, whichever conversations already land in the inbox. It does not connect to Instagram or WhatsApp directly. If your client's Instagram DMs route through a GoHighLevel Conversations inbox, CloseBot can answer them; if there's no CRM in the picture, there's nothing for the agent to plug into.

GoHighLevel itself runs $97/month for Starter, $297 for Unlimited, and $497 for Agency Pro — that's a third-party breakdown of GHL's pricing, not something CloseBot publishes, but any agency already selling to local businesses knows the number. So the honest per-client math looks like this:

- CRM subscription (HighLevel, HubSpot, whatever you already sell)
- AI setter platform fee
- Per-message usage, where the plan meters it
- AI provider token costs, where the platform passes them through

Two of those four lines are normally invisible in a vendor's headline price. CloseBot's business plans actually roll message costs into the base price rather than metering them on top, which is unusual in this category. The agency plans go the other direction: cheap messages, billed by usage, rebillable at your markup.

## What CloseBot is, in one paragraph

It builds "agents" — you give the agent an objective, knowledge, and tools, and it reasons through the conversation instead of walking a button tree. It ships with a drag-and-drop builder, a testing portal that lets you replay conversations before going live, human takeover on any thread, and a Smart FAQ that flags questions the agent couldn't answer confidently instead of inventing a discount you don't offer. There's native industry tooling for real estate and home services (property data, drive-time checks), Stripe payment collection inside the conversation, and unlimited custom connectors.

CloseBot's own site claims 1M+ booked appointments, 150,000 daily messages, 1,000+ agencies on the platform, and a 4.8 rating on G2 across 175+ reviews. Those are vendor-stated figures, not audited ones. In r/gohighlevel threads, the tone is broadly consistent with that: users rate conversation quality above GoHighLevel's native AI while a few flag the learning curve and occasional unreliability in demo links. Take both signals for what they are.

## Every plan CloseBot currently lists

The public plans page has a Free tier, a Core tier that branches into business and agency variants, and a custom-priced Growth tier. Business pricing scales with the monthly message ceiling you pick; agency pricing is flat with metered, rebillable usage on top.

| Plan | Who it's for | What's included | Price | Billing | Link |
| --- | --- | --- | --- | --- | --- |
| Free | Testing the platform, very low lead volume | 1 agent, 1 user seat, 100 monthly messages, 1 MB knowledge storage, unlimited account connections | $0 forever | — | [ Start on the free plan](https://app.closebot.com/a?fpr=li87) |
| Core (business) | Companies booking their own pipeline | 500 messages/month included, 15+ templates (50+ extra unlocked on annual), human support, add-on users at $5/seat, add-on storage and agents, no per-message charge within your ceiling | $64/mo; $53/mo billed as $640/yr on annual | Monthly or annual, month-to-month, cancel anytime | [ Check current business pricing](https://app.closebot.com/a?fpr=li87) |
| Core (agency) | Agencies selling AI setting to clients | Unlimited messages at $0.012/message, all costs rebillable, white-label client portal, client seats at $5 each, storage billed at $0.006/MB/day and rebillable | $397/mo (third-party reviews of the plans page list roughly $331/mo equivalent on annual billing) | Monthly or annual, includes a 7-day trial | [ See the agency plan and rebilling setup](https://app.closebot.com/a?fpr=li87) |
| Growth | Teams needing SLAs, compliance, or very high volume | 50+ templates, HIPAA compliance, quarterly audits, 99.99% priority uptime, priority support | Custom quote | Custom | [ Request Growth pricing](https://app.closebot.com/a?fpr=li87) |

Free plan overage runs $0.08 per message if you blow past 100 in a month. Business plans handle overage differently — you raise your ceiling for cheaper bulk rates, and anything above it is charged at a 2x overage rate drawn from a wallet.

### One pricing detail worth flagging

CloseBot's plans page FAQ states the agency rate is **$0.012 per message**. Older docs and blog posts on CloseBot's own site still quote **$0.006 per message**. That's a 2x difference on your largest variable cost, and it changes the margin on every client account. Confirm the current rate with their sales team in writing before you build a pricing model around it — don't assume the docs page is the source of truth.

There's a second ambiguity in the same area. CloseBot's V2 documentation says the platform requires you to use your own AI provider API keys and that message costs don't cover provider tokens. The plans page FAQ says the opposite: no "bring your own key," described as a security decision. Both statements are live on CloseBot properties right now. Whichever applies to your account determines whether you're buying tokens separately from OpenAI, Anthropic, DeepSeek, or nobody. Ask before you commit.

## Rebilling is the actual product here

If you're an agency, the rebilling mechanics matter more than the agent quality, because they decide whether this is a software expense or a revenue line.

On the agency plan you're billed for messages, storage, and seats, and you can re-bill all three to your clients at whatever markup you set. Client wallets top up via your own Stripe account, so client payments land with you and you settle with CloseBot. CloseBot's own page notes agencies bill anywhere from $100/month to $10,000+/month per client depending on positioning — which is a vendor framing, but it matches what the wider market does.

For context on the wider market: published breakdowns put appointment setting retainers at roughly $2,000–$4,500/month on subscription models, or $75–$500 per booked meeting, and AI automation agencies commonly run $500–$1,500/month for small business retainers. A human setter costs multiples of the software line. That gap is the entire business case, and it's why the per-message rate matters so much — it's the only cost in the stack that scales with the client's success.

[👉 Look at the agency plan's rebilling and white-label setup](https://app.closebot.com/a?fpr=li87)

## What CloseBot's own case studies actually cost

CloseBot published two real-world breakdowns on its blog. Worth reading carefully, because the message line in both was calculated at the older rate.

**Scaled agency:** 102 sub-accounts, ~108 conversational appointments/day, ~24,720 messages/month, 50 MB knowledge base, OpenAI as provider.

- $397 base plan
- $148 message costs at $0.006/message
- $9 knowledge base storage
- $255 token costs to OpenAI ($63 if routed to DeepSeek)
- **Total: $809/month**

At the current $0.012 rate, that message line becomes roughly $297, pushing the total north of $950 before tokens. Still cheap against 100+ booked appointments a day, but it's the difference between a comfortable margin and a thin one.

**Starting agency:** 4 sub-accounts, ~2 appointments/day, ~468 messages/month, 3 MB knowledge base, DeepSeek as provider.

- $397 base plan
- $3 message costs
- $0.50 storage
- $3 tokens
- **Total: $403.50/month**

A 4-client agency paying $403 to run AI setting across all four is fine if you're billing $500+/client. It's not fine if you're charging $150. The base plan is flat, which means low-volume accounts subsidize the platform rather than the other way around — and that's where a lot of agencies discover their pricing was too aggressive after they've signed the client.

## Business plan or agency plan?

Decide this before anything else.

Pick the **business track** if the agents work your own pipeline, you want message costs baked into a predictable monthly number, and you never need a client to log in and see anything. Real estate teams, home service companies, clinics, and coaches run here. The trade-off is that a business plan doesn't give you the rebilling view, white-labeling, or client portal.

Pick the **agency track** if clients pay you and you pay CloseBot. You'll pay more per month for the base plan and less per message, and you'll get the markup control that turns the whole thing into a service you can price. The 7-day trial applies to the agency plan too, so you can see the portal and rebilling config before you're billed.

## Limits, honestly

- **It needs a CRM.** No CRM, no agent. If a solo client's entire pipeline is Instagram DMs and they don't run a CRM, you're selling them two products.
- **Learning curve is real.** Several r/gohighlevel threads mention this, and there's a hiring market for CloseBot specialists, which tells you it isn't a 20-minute setup for anything complex.
- **No refunds.** CloseBot states this plainly. The free plan and the 7-day paid trial are your evaluation window, not a money-back period.
- **Message ≠ always one message.** One message equals one segment unless you enable the Agent Node's unlimited potential (many tools, unlimited instructions), where billing shifts to token costs. Heavy agents blow through ceilings faster than the plan name suggests.
- **Free plan caps are tight.** 100 messages, 1 seat, 1 agent, 1 MB storage, and you can't expand storage at all on free.

## A sane way to test it

Build one agent on the free plan and point it at real leads — not the demo, real ones. Give it your actual qualification criteria, your actual calendar, your actual FAQ. Run it for a couple of weeks at 100 messages/month, read the transcripts, and count booked appointments against what your current process produces.

If it books, spend the 7-day trial on the paid tier and test the thing that actually worries you: rebilling math at your real message volume, with your real markup. If a client's 3,000 monthly messages cost you $36 and you're billing $500, you have a business. If they cost you $36 and you're billing $150 on top of a CRM subscription you're also absorbing, you have a hobby.

[👉 Start free and build your first agent in CloseBot](https://app.closebot.com/a?fpr=li87)

## FAQ

**How much does it cost to run AI appointment setting for one client?**
On CloseBot's agency plan, $397/month base covers unlimited agents across unlimited accounts, then message usage at the published per-message rate, storage at $0.006/MB/day, and $5 per extra user seat. A client generating ~1,000 messages a month costs a few dollars in usage. The dominant cost is your base plan divided across your client count, not your usage.

**Can I resell it under my own brand?**
Yes — that's what the agency plan is for. White-labeled client portal, client seats so they can see their own dashboard and upload knowledge, and rebilling on messages, storage, and seats with markup you control.

**Do I need GoHighLevel?**
No. CloseBot integrates natively with HighLevel, HubSpot, LeadConnector, and custom CRMs, and the site lists standalone compatibility. But you do need some CRM for the agent to live inside — it isn't a channel-native tool.

**Is there a free plan?**
A free-forever tier capped at 100 messages a month, 1 agent, 1 seat, and 1 MB of storage. Paid plans come with a 7-day trial before billing starts.

**Will the AI close deals for me?**
No, and anything claiming otherwise is overselling. It qualifies, handles objections, follows up, and books. The close still happens on the call with a human. Treat it as the layer that keeps your calendar full.

## The short version

For agencies, the relevant question isn't whether CloseBot's agents are good — the conversation quality is the part people consistently praise, and the rebilling model is the most agency-shaped pricing in the category. The relevant question is whether your client pricing survives the real cost of the stack. Base plan, CRM subscription, message volume at whatever rate is actually current, plus tokens if they apply.

Run that math per client before you sign anything. Then decide whether the platform is the expense or the revenue line.
