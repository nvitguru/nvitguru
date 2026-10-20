# Jessie Martin

**Project manager at Social Points Media.** I plan, direct and ship a portfolio of small-business SaaS products, and I run the business itself with a team of coordinated AI agents.

My focus is **applied AI that is useful, safe and cheap to run**: grounding models in real business data, putting guardrails where mistakes would cost money or trust, keeping a human in the loop for anything that matters, and measuring cost per task.

---

## AI inside the products

| Product | What the AI does | How it's kept safe and affordable |
|---|---|---|
| [**Chattiv**](https://github.com/nvitguru/chattiv-casestudy): website live chat | **Ava**, an opt-in AI agent (Claude) that answers visitors from each business's own knowledge: an always-on business brief plus retrieval over its FAQ and crawled website | Human-first design with hand-off to a person; refuses to invent prices or policies; metered per chat. Businesses pay about **$0.07 to $0.10 per extra AI chat**, versus about $0.99 at LiveChat and Intercom (checked October 2026) |
| [**Texttive**](https://github.com/nvitguru/texttive-casestudy): business texting | **Smart Replies**: drafted replies and automatic answers to customer texts, plus an **AI Compliance Check** that screens messages against carrier rules | Consent and opt-out rules the AI can never override; automatic pause and hand-off to a human; usage-based pricing ($19/month + $0.02 per reply) |
| [**RepComet**](https://github.com/nvitguru/repcomet-casestudy): review and reputation management | **AI reply drafts** for Google reviews and AI insights from customer feedback | The owner always reviews and posts replies; built around a strict "no review gating" rule (every customer gets the same choice, as Google and the FTC require) |

## AI that runs the business

Behind the products, Social Points Media operates as a set of specialist AI "departments" (Claude), each in its own workspace, coordinated by a central hub:

- **Command Center:** a single point of contact that routes work to about 20 project and department agents, tracks every open item and sends a daily briefing. Approvals that matter (deploys, customer emails, publishing, money) always come back to a human.
- **Customer support assistant:** watches 13 support and assistant inboxes every hour. Plain rules filter junk for free, so the AI is only used when real mail arrives: a small, fast model sorts each message, and a stronger model drafts a reply grounded in each product's facts. Refunds, legal questions, angry customers and phishing attempts (including forged "from the owner" emails, caught by checking mail headers) are flagged for a human instead of answered. Every reply is a draft a person approves. Typical cost: a few cents per real email and nothing on quiet hours.
- **System monitor:** uptime and health checks plus hourly server digests; rules do the watching, and AI is called only to diagnose new problems, with a daily cap on AI investigations.
- **Specialist agents** for SEO, social media, billing, client acquisition and R&D, each producing proposals that a human approves before anything goes out.

## How I work

- **Ground the model, then constrain it:** answers come from the business's own data, with explicit rules for what the AI must never say or do.
- **Human in the loop where it counts:** AI drafts, people approve anything public, financial or irreversible.
- **Measure cost per task:** cheap filters and small models first, larger models only when needed.
- **Ship with tests:** automated test suites and CI on every product (RepComet alone has 700+ tests running on GitHub Actions).

**Stack:** Laravel / PHP, MySQL, Redis, Stripe, Twilio, Mailgun, the Anthropic API (Claude), GitHub Actions, DigitalOcean.

## Case studies

- [Chattiv](https://github.com/nvitguru/chattiv-casestudy): live chat with an opt-in AI agent
- [Texttive](https://github.com/nvitguru/texttive-casestudy): business texting with AI Smart Replies
- [ToroDocs](https://github.com/nvitguru/torodocs-casestudy): e-signatures
- [CrexiPay](https://github.com/nvitguru/crexipay-casestudy): invoicing and payments on Stripe
- [RepComet](https://github.com/nvitguru/repcomet-casestudy): reviews and reputation, with AI reply drafts

📫 Social Points Media: [socialpointsmedia.com](https://www.socialpointsmedia.com)
