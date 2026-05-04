# 해외살이, 나한테 맞을까? 🌏

A personality-based quiz web app built to explore **how organic traffic behaves through a quiz funnel** — and to demonstrate a full GA4 + GTM analytics implementation from scratch.

🔗 **Live:** [overseas-quiz.vercel.app](https://overseas-quiz.vercel.app)

---

## What This Project Is

This started as a content experiment targeting Korean-speaking audiences curious about living abroad. The real goal behind it was analytical: build a measurable funnel, instrument it properly, and see what the data says.

The quiz guides users through a series of questions and returns a personalised result type. Every step of that journey is tracked.

---

## Analytics Stack

| Layer | Tool |
|---|---|
| Tag Management | Google Tag Manager (`GTM-5M4CMZBX`) |
| Analytics | GA4 (`G-JBZJYJQBVW`) |
| Consent | Google Consent Mode v2 |
| Custom Dimensions | Quiz result type, question responses |
| Funnel Tracking | Step-by-step event tracking across all quiz stages |

**What's instrumented:**
- Quiz start, each question step, and result reveal — all as discrete GA4 events
- Custom dimensions capturing result category per user
- Consent Mode v2 with banner — compliant with UK/EU cookie requirements
- Funnel drop-off visibility across every question transition

---

## Results

- **1,000+ organic users** with no paid promotion
- Traffic sourced beyond initial Twitter seeding — validated organic reach within Korean-speaking communities
- Funnel data confirmed question-level drop-off patterns, informing content decisions

---

## Tech

- Vanilla HTML / CSS / JavaScript — zero dependencies, zero frameworks
- Deployed on Vercel
- Google Search Console verified (`google2bcd8133c0ac9ff7.html`)
- `sitemap.xml` submitted for indexing
- OG image configured for social sharing

---

## Key Decisions

**Why vanilla JS?**
The analytics layer is the point of this project, not the framework. Keeping the stack minimal meant the GTM/GA4 implementation is easy to inspect and learn from — no build step obscuring the tag firing logic.

**Why Consent Mode v2?**
UK GDPR compliance is non-negotiable for any real deployment. This project treats it as a requirement, not an afterthought.

---

## What I Learned

- Full GTM container setup from scratch: triggers, variables, tags, preview/debug
- GA4 custom event schema design before implementation (not after)
- Consent Mode v2 behaviour — how modelled conversions work when consent is denied
- Organic content distribution patterns in niche language communities

---

*Part of a broader portfolio of analytics and automation work. See [data-sj.vercel.app](https://data-sj.vercel.app)*
