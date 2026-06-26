# ScraperAPI Pricing Explained: How Much Does Each Plan Really Cost, Which Tier Should You Pick, and How Do API Credits Actually Work? (Plus the Real Cost-Per-Request Math Most Reviews Skip)

So you've landed on the ScraperAPI pricing page, you're staring at numbers like "100,000 credits" and "$49/month," and you're trying to figure out one simple thing: how many actual web pages does that get you? You're not alone. ScraperAPI's pricing looks straightforward on the surface — a handful of monthly tiers, a free trial, an annual discount — but the credit system underneath it has a way of surprising people on their first invoice.

This guide breaks down every single plan ScraperAPI currently offers, explains how the credit math actually works (this is the part that trips people up), and walks through which tier fits which kind of project. No fluff, no inflated claims — just the numbers as they currently stand, plus some practical guidance on getting the most out of your subscription.

## What ScraperAPI Actually Does (Quick Context Before the Numbers)

ScraperAPI is a web scraping API: you send it a URL, and it sends back the HTML — handling proxy rotation, CAPTCHA solving, JavaScript rendering, and anti-bot bypassing behind the scenes so you don't have to build and maintain that infrastructure yourself. It supports integrations across Python, Node.js, PHP, Ruby, and Java, plus a no-code scheduler called DataPipeline for people who'd rather not write scraping scripts at all.

Every plan, from the smallest to the largest, includes the same core feature set: JS rendering, premium proxies, automatic JSON parsing, rotating proxy pools, CAPTCHA and anti-bot detection, custom headers and sessions, automatic retries, unlimited bandwidth, and a 99.9% uptime guarantee. What changes between tiers isn't the feature list — it's the **credit allowance, concurrency limit, and geotargeting scope**. That's the whole game when it comes to ScraperAPI pricing.

## How ScraperAPI's Credit-Based Pricing Actually Works

This is the single most important thing to understand before picking a plan, because it's also the part that catches people off guard. ScraperAPI doesn't charge per "request" in a simple 1-to-1 sense — it charges in **credits**, and not every request costs the same number of credits.

Here's the breakdown straight from ScraperAPI's own cost structure:

- A standard, unprotected page costs **1 credit**
- Scraping Amazon costs **5 credits**
- Scraping Google or Bing (including subdomains) costs **25 credits**
- Scraping LinkedIn costs **30 credits**
- Any site sitting behind bot protection like Cloudflare, Datadome, or PerimeterX adds **+10 credits** on top, when ScraperAPI has to bypass that protection
- Enabling JavaScript rendering or premium/ultra-premium proxies multiplies the credit cost further, depending on the target site

> In practice, this means a plan advertising "100,000 credits" might give you 100,000 simple page scrapes — or it might give you closer to 6,000–7,000 requests if you're hitting Amazon listings with JS rendering turned on. The advertised credit number and your real, usable request volume are two different things, and it depends entirely on what you're scraping.

Before committing to a paid plan, it's worth using the Domain Cost Estimator inside the ScraperAPI dashboard (available once you sign up) to check exactly how many credits your specific target sites will consume per request. That single step will tell you more about real-world ScraperAPI pricing for your use case than any plan comparison chart.

## ScraperAPI Pricing: Full Plan Breakdown (Free to Enterprise)

ScraperAPI currently runs eight tiers in total — one free plan and seven paid tiers, topping out at a custom Enterprise plan. Annual billing knocks roughly 10% off every paid tier. Here's the complete, current lineup:

| Plan | Monthly Price | Annual Price (per mo) | API Credits / mo | Concurrent Threads | Geotargeting | Get Started |
|---|---|---|---|---|---|---|
| **Free** | $0 | — | 1,000 | 5 | US & EU | [ Start free, no card required](https://www.scraperapi.com/signup/?fp_ref=coupons) |
| **Hobby** | $49 | $44.10 | 100,000 | 20 | US & EU only | [ Get the Hobby plan](https://www.scraperapi.com/pricing/?fp_ref=coupons) |
| **Startup** | $149 | $134.10 | 1,000,000 | 50 | US & EU only | [ Get the Startup plan](https://www.scraperapi.com/pricing/?fp_ref=coupons) |
| **Business** | $299 | $269.10 | 3,000,000 | 100 | Global (country-level) | [ Get the Business plan](https://www.scraperapi.com/pricing/?fp_ref=coupons) |
| **Scaling** ⭐ Most popular | $475 | $427.50 | 5,000,000 | 200 | Global (country-level) | [ Get the Scaling plan](https://www.scraperapi.com/pricing/?fp_ref=coupons) |
| **Professional** | $975 | $877.50 | 10,500,000 | 300 | Global (country-level) | [ Get the Professional plan](https://www.scraperapi.com/pricing/?fp_ref=coupons) |
| **Advanced** | $1,975 | $1,777.50 | 21,500,000 | 500 | Global (country-level) | [ Get the Advanced plan](https://www.scraperapi.com/pricing/?fp_ref=coupons) |
| **Enterprise** | Custom | Custom | 22,000,000+ | 500+ | Global (country-level) | [ Talk to sales](https://www.scraperapi.com/contact-sales/?fp_ref=coupons) |

A few things worth flagging in that table:

- **Geotargeting is a real differentiator.** Hobby and Startup are locked to US and EU locations only. If your project needs to scrape from other regions, you'll need at least the Business plan.
- **Business and above unlock unlimited analytics history** in the dashboard, versus a rolling 30-day window on Hobby and Startup.
- **Scaling, Professional, Advanced, and Enterprise all include Pay-As-You-Go**, meaning if you blow through your monthly credits, you can keep scraping at a fixed per-credit overage rate instead of getting cut off — Hobby, Startup, and Business plans instead prompt you to upgrade tiers or contact support once you hit 100%.
- **Credits do not roll over.** Whatever you don't use resets at renewal, so it's worth sizing your plan to your actual monthly volume rather than overbuying "just in case."

## Monthly vs. Annual Billing: Is the 10% Worth Committing For?

ScraperAPI applies a flat ~10% discount across every paid tier when you pay annually instead of month-to-month. On the Hobby plan, that's the difference between $588/year (monthly) and $529.20/year (annual) — a $58.80 saving. On the Business plan, annual billing saves roughly $358.80 over the year. The discount scales proportionally as you move up tiers, so the higher your usage, the more absolute dollars the annual commitment saves you.

The trade-off is flexibility: annual plans lock you in for 12 months. If your scraping volume is genuinely predictable — say, a recurring e-commerce price-monitoring job or an ongoing SEO tracking pipeline — annual billing is close to free money. If you're still validating a new project or your volume swings a lot month to month, staying monthly until you have a few stable billing cycles under your belt is the safer move.

## Free Trial and Free Plan: Testing Before You Pay

ScraperAPI gives you two separate ways to try the service without committing money upfront:

1. **7-day trial** — new signups get 5,000 free API credits and access to test the platform at a larger scale than the permanent free tier, with no credit card required.
2. **Permanent free plan** — after the trial, accounts default to 1,000 free credits per month with a maximum of 5 concurrent connections, available indefinitely for small, low-volume projects.

This is genuinely the most useful first step in evaluating ScraperAPI pricing for your situation: sign up, run your actual target URLs through the Domain Cost Estimator, and see exactly what your real credit burn rate looks like before picking a paid tier.

👉 [Start your free ScraperAPI trial here](https://www.scraperapi.com/signup/?fp_ref=coupons)

## What About ScraperAPI Coupon Codes?

If you've searched around, you've probably seen a long list of supposed ScraperAPI promo codes floating around coupon aggregator sites — most claiming 20–60% off. Worth being skeptical here: a lot of these list outdated price points that don't match ScraperAPI's current official pricing, which is a strong sign they're stale or simply unverified.

What's actually confirmed directly from ScraperAPI's official pricing page:

- **Annual billing discount** — roughly 10% off any paid plan, automatically applied when you switch the billing toggle to yearly
- **7-day free trial with 5,000 credits** — no credit card required, the closest thing to a "discount" for anyone still deciding

If ScraperAPI is running a seasonal promotion (Black Friday, Cyber Monday, etc.), it will show up directly on the official pricing page rather than through third-party codes of uncertain validity. The safest way to check what's currently active is to look there directly:

👉 [Check current ScraperAPI pricing and active offers](https://www.scraperapi.com/pricing/?fp_ref=coupons)

## Which ScraperAPI Plan Should You Actually Choose?

Plan selection really comes down to two questions: how many requests per month do you realistically need, and what are you scraping? Here's a rough breakdown by use case:

- **Solo developers, students, side projects** → Start on the **Free plan** (1,000 credits/mo). It's enough to build and test a scraper before you're paying anything.
- **Small businesses, freelancers, personal SaaS tools** → **Hobby** ($49/mo) covers light, steady scraping of standard pages, as long as you don't need geotargeting outside the US/EU.
- **Growing startups with moderate, recurring scraping jobs** → **Startup** ($149/mo) is the jump to 1M credits, useful once a single project outgrows Hobby's 100K ceiling.
- **Agencies and production workloads needing global data** → **Business** ($299/mo) is the first tier with global geotargeting and unlimited analytics history — important if you're scraping region-specific search results or e-commerce listings.
- **Larger ongoing operations** → **Scaling** ($475/mo) is ScraperAPI's flagged "most popular" tier, adding Pay-As-You-Go so you're never hard-blocked mid-month.
- **High-volume, recurring data pipelines** → **Professional** and **Advanced** add priority support/routing on top of much larger credit pools, suited to teams running continuous scraping jobs across multiple sources.
- **Enterprise-scale data acquisition** → The **Enterprise** plan is fully custom — 22M+ credits, a dedicated support team, and Slack-based support, built for organizations with unpredictable or massive volume needs.

## ScraperAPI Pricing vs. the Alternatives

It's worth knowing where ScraperAPI sits relative to other scraping APIs when you're evaluating the price tag. Competing tools in a similar category — services like ScrapingBee and ScrapingDog — tend to start in a comparable $49/month range for their entry tier, while infrastructure-heavy providers like Bright Data often price by data volume rather than flat monthly credit pools. ScraperAPI's entry point is competitive for small projects, but because of the credit-multiplier system described above, your effective cost per request can climb quickly once you're scraping JavaScript-heavy or bot-protected sites — so it's worth comparing based on your actual target domains, not just the sticker price.

## Pros and Cons of ScraperAPI's Pricing Model

**What works in ScraperAPI's favor:**
- Low entry price point relative to building your own proxy infrastructure
- Free trial and permanent free tier make it easy to test before paying
- Annual billing offers a real, transparent discount
- Pay-As-You-Go on higher tiers avoids hard service interruptions
- All core features (JS rendering, CAPTCHA handling, parsing) are included on every plan — no feature-gating between tiers

**Where it gets more complicated:**
- The credit-multiplier system (1x for simple pages up to 75x for the most protected targets) makes it genuinely hard to estimate your real monthly cost in advance
- Geotargeting is restricted to US/EU on the two cheapest paid tiers
- Credits don't roll over between billing cycles
- Heavy JS-rendering or anti-bot-protected workloads can burn through a plan's credit pool far faster than the headline number suggests

## Frequently Asked Questions About ScraperAPI Pricing

**Does ScraperAPI have a free plan?**
Yes — after the 7-day, 5,000-credit trial, accounts default to a permanent free tier of 1,000 API credits per month with up to 5 concurrent connections. No credit card is required to sign up.

**What happens if I run out of credits?**
On Hobby, Startup, or Business, you can either upgrade to the next tier (usually at a better price-per-credit) or contact support about a custom plan. On Scaling, Professional, Advanced, or Enterprise, Pay-As-You-Go lets you keep scraping past your limit at a fixed overage rate, with an optional monthly spending cap.

**Do unused credits roll over to the next month?**
No. Your credit balance resets at renewal regardless of plan tier.

**Can I cancel my ScraperAPI subscription anytime?**
Yes, cancellation is available anytime from the dashboard or by contacting support, with no cancellation fee.

**Is there a refund policy?**
ScraperAPI offers a 7-day, no-questions-asked refund window if you're not satisfied with the service.

**Does one request always equal one credit?**
No — credit cost depends on the target domain and the parameters used (JS rendering, premium proxies, etc.). Use the Domain Cost Estimator in the dashboard to check exact costs before scraping at scale.

## Bottom Line

ScraperAPI's pricing is straightforward at the headline level — eight tiers from free to custom Enterprise, a clean 10% annual discount, and a generous trial to test things out. The part that actually determines whether a plan is "worth it" for you is the credit-multiplier system underneath: what you're scraping matters just as much as which plan you pick. The smartest move is to start free, run your real target URLs through the cost estimator, and size your plan around your actual usage pattern rather than the advertised credit number alone.

👉 [Compare all ScraperAPI plans and start your free trial](https://www.scraperapi.com/pricing/?fp_ref=coupons)
