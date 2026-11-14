---
author: Rikelvi Capellán
category: Artificial Intelligence
cover: /articles/covers/ai-2026-advances-problems.png
description: "What actually improved in AI this year —models, agents, science— and which risks are now structural: security, misinformation, energy, market concentration, and the EU AI Act's final stretch."
lang: en
pageTitle: ai-2026-advances-problems
tags:
  - artificial intelligence
  - agents
  - security
  - eu ai act
  - energy
  - "2026"
  - analysis
timestamp: 14/Nov/2026
title: "AI in 2026: real advances and the problems we can no longer ignore"
translationKey: ai-2026
---

For years, the conversation about artificial intelligence ran ahead of reality: promises of autonomous agents, models that would rewrite entire industries, and a race to show off the most impressive demo. November 2026 sounds different. AI is no longer on stage; it is in email, in calendars, in search and in the supply chain. And with that, failures stopped being theoretical too.

This is a review of what genuinely improved this year and of the cracks that are now structural. It is not a headline recap: it is an attempt to separate demonstrated capability from operational risk, with references so you can check it yourself.

## What actually improved

### Models that reason in parts

On November 12, Google introduced **Gemini 4 Hydrogen**, which the company calls its biggest Search upgrade yet. The interesting change is not a higher benchmark score but the kind of task it handles: questions with multiple parts, hard-to-interpret typos and highly specific requests. The model breaks the question down, queries several subtopics at once and returns more links, comparison tables, graphs and maps. It also adds an `xhigh` reasoning level for the cases that need it.

That a model like this is now the default in AI Mode and for the hardest AI Overviews questions says a lot about where search is going: fewer "ten blue links" and more of a constructed answer, with sources the user is expected to check. That is useful. It also puts a new responsibility on the reader: verifying whether the answer and its sources hold up.

### Agents that do work, not just conversation

The second real advance is agents moving into everyday tasks. **Claude Duet**, Anthropic's consumer agent, connects to email, calendar, Google Docs and Slack. In a week-long test, _The Verge_ described it as genuinely helpful for spotting contradictions between a meeting and a direct message, or for flagging a deadline that had been overlooked. It also described it as a slightly neurotic assistant: it misread the context of a deadline, missed the tone of a message, and even offered to review its own work.

That nuance matters. An agent's advantage is not that it "thinks" better than a chat model, but that it has access to more context and can act on it. The risk is not abstract either: the more context and the more permissions, the more damage a bad judgment call can do. The review's practical conclusion is the right one: an agent works as a backstop for your organizational systems, not as a replacement for them.

### Science: speeding up the search, not skipping validation

There are encouraging signals in science too. Google DeepMind introduced **AlphaGenome 2**, aimed at understanding genetic regulation and the cellular roots of disease. And a swarm of AI agents was presented as the discoverer of a Maya site from NASA LIDAR data. The second story is especially instructive: the site had already been published years earlier by an archaeologist, and the AI had rediscovered something already in the literature.

That is not an AI failure: it is exactly what AI does well, finding patterns at scale. The failure would be believing that an agent's output replaces fieldwork, peer review or a discipline's prior knowledge. AI accelerates the search; validation remains human.

## The cracks that are no longer theoretical

### 1. Security: the shared link as a hole

The clearest case of the year is **Grok Build**, SpaceXSI's coding agent. A researcher at security firm Claroc found 43,601 links to apps built with the tool. More than 35,000 — nearly 95% — opened the app and all of its data to anyone holding the link. The exposed data included medical exams for 3,784 workers, internal résumés, client proposals, sales plans and 24 apps built by SpaceXSI itself containing confidential material.

The technical cause is simple and embarrassing: the random identifier was in the subdomain, not the path. That makes the links enumerable through passive DNS services. Meta had a similar problem with Muse weeks earlier. And it is not unique to one tool: Lovable, Bolt and Replit also give each app its own web address, so the same pattern can repeat.

The lesson is not "don't use coding agents." It is that **sharing is an authorization decision**, not a UI detail. A "anyone with the link" URL is a credential. If your product generates links, it needs real authentication, per-resource permissions, expiry and access logs.

### 2. Trust: answers that recommend scams

Another problem that stopped being hypothetical is recommendation quality. A study by Podqi analyzed 6,795 answers from ChatGPT, Gemini and Perplexity to shopping questions about 151 brands. Up to 15% of Perplexity's answers surfaced "risky" sites: fake stores impersonating a brand, old domains re-registered by someone else, or dead sites anyone could buy. ChatGPT came in at 8% and Gemini at 4%.

The most uncomfortable detail is that the models sometimes invented regional websites for brands with no regional presence. For users, the risk is direct: entering payment details in a store that looks official because a chatbot cited it. For brands, it is a reputation and fraud problem. And for anyone building with AI, it is a reminder that answer quality is not only how convincing it sounds, but where its sources come from.

### 3. Economics: concentration and governance

The week of November 12 was a reminder of how much of the industry depends on a few pieces. Nvidia, the chip supplier underpinning much of the AI buildout, announced the resignation of CEO Jensen Huang after two extramarital relationships — one with a person described as an alleged Chinese spy — and a board investigation. CFO Colette Kress took over on an interim basis. The company also held an investment portfolio of roughly $99 billion across AI companies, from frontier labs to cloud providers.

That same week, Anthropic confirmed it plans to start trading on November 19, with a guide price of $70 to $78 per share and a valuation of up to $1.4 trillion.

You do not have to decide whether this is a bubble to see the risk: when the infrastructure supplier also invests in its customers, and customers are valued on what they can buy with that infrastructure, one company's governance becomes a systemic issue. The question is no longer only "which model is better?" but "who controls access, price and terms?"

### 4. Energy and territory

AI consumes electricity, and increasingly so. The IEA's _Energy and AI_ report estimated that data-center electricity consumption could more than double to around 945 TWh by 2030, from about 415 TWh in 2024. This is not only an emissions problem: it is a grid, price and land problem.

In the United States, data-center opposition became an election issue in the 2026 midterms. Voters favored limits in nearly every ballot measure, and advocacy groups are already pushing politicians to keep their promises. In practice, building a data center is no longer just a technical or financial decision; it is a local political one.

### 5. Regulation: the AI Act is no longer a draft

The **EU AI Act** completed its main rollout on August 2, 2026: most of its obligations now apply, with exceptions for high-risk systems, which arrive on December 2, 2027 (Annex III) and August 2, 2028 (Annex I). Systems that generate synthetic audio, image, video or text and were already on the market have until December 2, 2026 to comply with the transparency obligations in Article 50. The same day, bans on non-consensual intimate imagery and child sexual abuse material take effect.

For a small business, this translates into four concrete tasks: classify the system by risk, document the decisions, label synthetic content where required, and train the people who use it. This is not optional paperwork: it is the difference between being able to sell in Europe and not being able to.

### 6. Work and judgment

Generative AI keeps entering creative workflows. This year's GDC Festival of Gaming survey showed more game developers using it, against a backdrop of layoffs and pressure to ship faster. But the Grok Build case leaves a more uncomfortable lesson for the productivity narrative: if nobody reviews what the agent produces, the time saved is paid back later in incidents.

The pattern I see in teams that work is not "AI does the job." It is "AI produces the first draft and a person decides what stays." That requires judgment, and judgment is exactly what does not get delegated. As I wrote in [my notes on AI-assisted development](/articles/ai-assisted-development), the rule is still the same: if you cannot explain a line, do not merge it.

## What to do if you build with AI

If you are integrating models or agents into a product, these are the controls that separate a demo from a system:

- **Treat model output as untrusted input.** Never concatenate it directly into SQL, shell or HTML. Validate, escape and constrain.
- **Scope permissions by tool, not by agent.** An agent that can read email should not be able to send money. Use allowlists and human approval for irreversible actions.
- **Design link sharing as authentication.** Private links by default, per-resource permissions, expiry and audit logs. Entropy is not authorization.
- **Verify sources.** If your product recommends products, doctors or procedures, restrict answers to trusted domains and always show the citation. A link is not a guarantee.
- **Measure cost, latency and energy.** Not every problem needs the largest model. Routing simple tasks to smaller models is both a product and a sustainability decision.
- **Prepare for the regulatory calendar.** Risk classification, documentation, transparency and training. The AI Act is already here, not in a hypothetical future.
- **Have an incident plan.** What you do if an agent leaks data, a recommendation turns out to be fraudulent, or a model starts failing in production. Without that plan, you do not have a system: you have a bet.

## The uncomfortable conclusion

AI in 2026 is both more capable and more fragile than its marketing suggests. Models reason better, agents have more context, and science is moving. But failures no longer happen in a lab: they happen in a shared link, in a shopping recommendation, in a CEO's resignation or in a region's electricity bill.

The bottleneck is no longer model capability. It is trust, governance and accountability. And those three things are not fixed with a new set of weights: they are fixed with design, auditing and human decisions.

If a system recommends, buys or decides, it needs the same guarantees as any other system that does those things. That is the conversation the industry has been postponing for far too long.

## References

- [EU Artificial Intelligence Act — Implementation Timeline](https://artificialintelligenceact.eu/implementation-timeline/) (updated August 31, 2026).
- [IEA — Energy and AI](https://www.iea.org/reports/energy-and-ai) (April 10, 2025) and [Key Questions on Energy and AI](https://www.iea.org/reports/key-questions-on-energy-and-ai) (April 16, 2026).
- [The Verge — Google's new Gemini model is better at understanding complicated questions](https://www.theverge.com/ai-artificial-intelligence/1032505/google-search-ai-mode-gemini-4-hydrogen) (November 12, 2026).
- [The Verge — Claude's Duet agent is a little neurotic and surprisingly helpful](https://www.theverge.com/ai-artificial-intelligence/1032518/claude-duet-ai-agent-hands-on) (November 13, 2026).
- [Ars Technica — Grok Build coding agent leaks oodles of confidential info](https://arstechnica.com/security/2026/11/grok-build-coding-agent-leaks-oodles-of-confidential-info-some-belonging-to-spacexsi/) (November 10, 2026).
- [The Verge — AI chatbots are recommending fake retail websites, study finds](https://www.theverge.com/ai-artificial-intelligence/1032020/gemini-chatgpt-perplexity-shopping-test-risky-fake-websites-citations) (November 12, 2026).
- [The Verge — Nvidia CEO Jensen Huang resigns amid spy, affair scandals](https://www.theverge.com/ai-artificial-intelligence/1031689/jensen-huang-nvidia-ceo-resigns) (November 12, 2026).
- [The Verge — Anthropic confirms its IPO plans](https://www.theverge.com/ai-artificial-intelligence/1031894/anthropic-confirms-its-planning-for-its-shares-to-start-publicly-trading-on-november-19th) (November 12, 2026).
- [The Verge — Data center opponents are cheering midterm results](https://www.theverge.com/policy/1026365/data-centers-midterms-results) (November 11, 2026).
- [The Verge — Google's AlphaGenome 2 zooms in on the cellular roots of disease](https://www.theverge.com/ai-artificial-intelligence/1031524/google-deepmind-alphagenome-2-genetic-ai-model) (November 11, 2026).
- [The Verge — No, AI agents did not discover a previously unknown Maya site](https://www.theverge.com/ai-artificial-intelligence/1032125/ai-agents-maya-site-archeology-discovery) (November 12, 2026).
- [The Verge — More game developers are starting to use generative AI](https://www.theverge.com/games/1032085/gdc-festival-of-gaming-annual-survey-ai-layoffs) (November 12, 2026).
