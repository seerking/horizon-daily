---
layout: default
title: "Horizon Summary: 2026-11-10 (EN)"
date: 2026-11-10
lang: en
---

> From 19 items, 7 important content pieces were selected

---

**Technology News**
1. [DeepMind Introduces AlphaProof Code for Verified Lean/Rocq Code](#item-tech-news-1) ⭐️ 8.0/10
2. [Anthropic Announces Fable 5.2 and Mythos 5.2 Models](#item-tech-news-2) ⭐️ 8.0/10
3. [Fireworks AI breach exposes Notion AI chat transcripts](#item-tech-news-3) ⭐️ 7.0/10
4. [Project Uses TV Signals to Sense Objects Through Walls](#item-tech-news-4) ⭐️ 7.0/10
5. [Meta launches Muse Ember, a small model for agent workloads](#item-tech-news-5) ⭐️ 7.0/10
6. [XGBoost outage forecast beats NWS/SPC baselines 2.4× on PR-AUC](#item-tech-news-6) ⭐️ 7.0/10
7. [JEPA-style tactile pretraining outperforms reconstruction baselines](#item-tech-news-7) ⭐️ 7.0/10

---

## Technology News

<a id="item-tech-news-1"></a>
### [DeepMind Introduces AlphaProof Code for Verified Lean/Rocq Code](https://deepmind.google/blog/introducing-alphaproof-code/) ⭐️ 8.0/10

DeepMind announced AlphaProof Code, an agent that writes formally verified code in Lean and Rocq. The supplied item provides no technical details on versions, availability, or measured results, so the announcement&\#x27;s scope and novelty remain unconfirmed. Hacker News commenters questioned how the agent differs from a classic coding agent that iterates over a codebase while writing and running Lean or Rocq code, and one noted that it appears to address implementation rather than the specification itself.

hackernews · ilreb · Nov 10, 12:11 · [Discussion](https://news.ycombinator.com/item?id=50439193)

**「Background」** DeepMind&\#x27;s AlphaProof Code is a multi-agent AI framework for formal software specification and verification, and the company says it used it to prove key security properties of libsignal, the Signal protocol&\#x27;s reference implementation, at the machine-code level. The framework splits verification work between human experts, who decide what to prove, and a group of AI agents that carry out the proofs.

**「Practical impact」** The community discussion points to a concrete limitation for anyone adopting such an agent: because the AI writes the Lean/Rocq proofs itself, a commenter \(r0ze-at-hn\) reports that AI-generated Lean can &quot;easily cheat,&quot; and recommends running a separate adversarial review prompt over the generated proofs. A commenter also notes the agent appears to target implementations rather than specifications, which bounds what a passing proof actually guarantees.

**「Community Discussion」** Commenter r0ze-at-hn reported experimenting with AI-generated Lean and warned that AI can &quot;easily cheat&quot; when writing proofs, recommending a separate adversarial review prompt; they also said the paper reintroduced some bugs to test detection but did not find bugs it located. Another commenter asked how the approach compares with Theorem and Anthropic&\#x27;s work on formally proving nixpkgs, while thibsrn questioned whether the agent is meaningfully different from a standard coding agent.

<details><summary>References</summary>
<ul>
<li><a href="https://deepmind.google/blog/introducing-alphaproof-code/">Formal Verification of Signal’s Protocol with... — Google DeepMind</a></li>
<li><a href="https://storage.googleapis.com/gdm-deepmind-com-prod-public/media/documents/Formal_Verification_of_Signal_4.pdf">AlphaProof Code : Verifying Signal’s Security at</a></li>

</ul>
</details>

**Tags**: `#formal verification`, `#AI coding agents`, `#Lean`, `#DeepMind`, `#software correctness`

---

<a id="item-tech-news-2"></a>
### [Anthropic Announces Fable 5.2 and Mythos 5.2 Models](https://www.anthropic.com/claude-fable-and-mythos-5-2) ⭐️ 8.0/10

Anthropic announced two new models, Fable 5.2 and Mythos 5.2, according to a Hacker News post linking to Anthropic&\#x27;s site; no source text was available, so the announcement&\#x27;s specific capabilities and availability conditions could not be verified. The post&\#x27;s analysis summary describes vendor claims about multi-agent OS prototyping and other engineering feats, which are prerelease claims rather than independently measured results. Community commenters report early hands-on use of Fable 5.2, with one saying it is hard to distinguish from Opus 5.5 on ordinary coding tasks unless prompts are pushed toward higher ambition.

hackernews · lairv · Nov 9, 18:01 · [Discussion](https://news.ycombinator.com/item?id=50429068)

**「Background」** Anthropic&\#x27;s Fable line has an immediate predecessor: OpenRouter&\#x27;s listing describes Fable 5.2 as gaining over Fable 5.1 in coding, reasoning, and vision, and a commenter compares the new release with the earlier Fable 5/5.1 versus Opus 4.8/5 pairing. The release also pairs Fable 5.2 with a second model, Mythos 5.2, and the vendor&\#x27;s own account describes a prerelease experiment in which Fable 5.2 coordinated over 1,000 subagents for eight days to build a prototype operating system from an empty folder.

**「Impact」** For developers choosing among Anthropic models, one early tester&\#x27;s report suggests Fable 5.2&\#x27;s advantage over Opus 5.5 may only appear on ambitious tasks, so routine coding work may not justify switching. The vendor&\#x27;s more dramatic claims, such as an engineer directing over 1,000 subagents for eight days to build a bootable prototype OS, remain unverified and should not be treated as measured capability.

**「Community Discussion」** Commenters split between hands-on impressions and skepticism: postalcoder said Anthropic&\#x27;s lineup now feels balanced and that Fable 5.2 is hard to tell apart from Opus 5.5 for ordinary coding, while endriju questioned the extraordinary prerelease claims, including solving black-hole physics problems and formalizing Fermat&\#x27;s Last Theorem in 30 hours. breakwaterlabs pressed on benchmark methodology, asking why Fable xHigh was compared against Carbon Med and why the cyber-focused Carbon model was omitted from the cyber benchmark comparison.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/claude-fable-and-mythos-5-2">Introducing Claude Fable 5 . 2 and Claude Mythos 5 . 2 \ Anthropic</a></li>
<li><a href="https://openrouter.ai/anthropic/claude-fable-5.2">Claude Fable 5 . 2 - API Pricing &amp; Benchmarks | OpenRouter</a></li>

</ul>
</details>

**Tags**: `#AI models`, `#Anthropic`, `#multi-agent systems`, `#software engineering`, `#model release`

---

<a id="item-tech-news-3"></a>
### [Fireworks AI breach exposes Notion AI chat transcripts](https://www.notion.com/help/security-incident-involving-a-third-party-ai-vendor) ⭐️ 7.0/10

Notion disclosed a security incident involving third-party AI vendor Fireworks AI, stating that newly analyzed data included unattributable Notion AI chat transcripts used for its Insights feature. According to Notion&\#x27;s notice, the transcripts were not labeled with author or workspace, contained no tool call results, and carried no information beyond the chat text that could identify a workspace, user, or company; Notion recommended customers treat the data as compromised as a precaution. The supplied material does not establish how the data was retained or leaked, and community commenters point to Fireworks AI&\#x27;s security bulletins, which they say also mention leaked customer model weights and training datasets.

hackernews · werrett · Nov 10, 07:19 · [Discussion](https://news.ycombinator.com/item?id=50437106)

**「Background」** Fireworks AI disclosed an October 2026 security incident in which an unauthorized third party used internal credentials to access environment variables in evaluation jobs across a limited number of customer accounts. Notion&\#x27;s advisory states that Fireworks notified it on November 6, 2026, and that the incident affected fewer than 1% of Notion workspaces. Fireworks has since published an update describing the data involved and hardening measures.

**「Impact」** Notion customers who used the Insights feature should treat their AI chat content as potentially exposed, since Notion says the transcripts cannot be tied back to a specific workspace or user and therefore cannot be individually scoped. The incident also puts vendor risk on organizations relying on third-party inference providers, particularly where data-retention settings differ from a provider&\#x27;s default posture.

**「Community discussion」** Commenters questioned how data could leak if Fireworks AI is labeled as zero-data-retention on OpenRouter, with one asking whether Notion configured Fireworks to retain data. Another commenter cited Fireworks&\#x27; breach page as also reporting leaked customer model weights and training datasets, while a third linked the vendor&\#x27;s official bulletins.

<details><summary>References</summary>
<ul>
<li><a href="https://fireworks.ai/security/bulletins/october-2026-security-incident-update">Update on October 2026 security incident | Fireworks AI</a></li>
<li><a href="https://fireworks.ai/security/bulletins/october-2026-security-incident">Fireworks October 2026 security incident | Fireworks AI</a></li>
<li><a href="https://www.notion.com/security/advisories/security-incident-involving-a-third-party-ai-vendor">Fireworks AI incident - notion.com</a></li>

</ul>
</details>

**Tags**: `#security`, `#AI infrastructure`, `#data privacy`, `#vendor risk`, `#Notion`

---

<a id="item-tech-news-4"></a>
### [Project Uses TV Signals to Sense Objects Through Walls](https://maurycyz.com/projects/fading/) ⭐️ 7.0/10

A project write-up explores using TV broadcast signals to sense objects through walls, relying on the way bodies and objects perturb RF propagation. The author frames it as an experiment in passive RF sensing rather than a product, and no source content was supplied to confirm measured range, accuracy, or hardware specifics. Commenters connect the technique to related work, including LTE-based traffic counting that estimated vehicle direction and type.

hackernews · Curiositry · Nov 10, 05:24 · [Discussion](https://news.ycombinator.com/item?id=50436410)

**「Background」** Passive RF sensing works by processing reflections of existing broadcast signals rather than transmitting its own radar pulses; earlier work demonstrated the concept with Wi-Fi, using software-defined radios and cross-ambiguity processing to detect motion through walls. A related application used standardized LTE/4G radio performance counters and machine learning to estimate road traffic flow, including direction and vehicle type, by sensing obstacles in the environment rather than tracking phones. The project discussed here extends the same passive-sensing idea to TV broadcast signals.

**「Impact」** The discussion suggests the same passive-sensing principle is already practical with commodity radio infrastructure: one commenter reports using LTE/4G signals to count road traffic and classify pedestrians, small vehicles, and large vehicles, claiming better accuracy than Google Maps because the sensing is independent of moving phones. That implies ambient-signal sensing can work without dedicated radar hardware, though the claim is a commenter&\#x27;s reported experience rather than an independently verified result.

**「Community Discussion」** Commenters treated the idea as an extension of familiar RF behavior, noting that analog TV reception visibly changed with where people stood, and one linked low-cost \(under $10\) ESP-SDR setups for observing WiFi and some LTE spectra. Others raised privacy concerns, pointing to fiber-optic cables as another medium where acoustic vibrations can be measured, though that claim was not substantiated in the thread.

<details><summary>References</summary>
<ul>
<li><a href="https://micrologics.org/blog/passive-wifi-radar-engineering-thru-wall-rf-sensing-with-sdrs-and-python">Passive WiFi Radar: Engineering Thru-Wall RF Sensing with ...</a></li>
<li><a href="https://forums.ni.com/t5/Real-World-Applications/Tracking-WiFi-Signals-to-Passively-See-Through-Walls-UK/ta-p/3762174">Tracking WiFi Signals to Passively See Through Walls (UK)</a></li>
<li><a href="https://www.researchgate.net/publication/348739408_Traffic_Flow_Estimation_using_LTE_Radio_Frequency_Counters_and_Machine_Learning">(PDF) Traffic Flow Estimation using LTE Radio Frequency ...</a></li>

</ul>
</details>

**Tags**: `#RF sensing`, `#signal processing`, `#wireless`, `#privacy`, `#hardware`

---

<a id="item-tech-news-5"></a>
### [Meta launches Muse Ember, a small model for agent workloads](https://simonwillison.net/2026/Nov/10/muse-ember/) ⭐️ 7.0/10

Meta AI released Muse Ember 1.0, which it describes as its smallest and most efficient model, aimed at repeated agent work such as tool calls, coding subtasks, routing, extraction, and long document parsing. For prompts up to 200k tokens it costs $0.10 per million input tokens and $0.50 per million output tokens, matching the short-prompt rates of GPT-6 Luna and Claude Haiku 5.5; above 200k tokens the rates rise to $0.30 input and $1.50 output. Simon Willison notes that Ember&\#x27;s long-prompt pricing falls between Luna&\#x27;s and Haiku&\#x27;s, and that Artificial Analysis places Ember&\#x27;s xhigh and max configurations on its cost-per-task Pareto frontier. The model offers six reasoning levels \(minimal, low, medium, high, xhigh, max\), though Willison reports that the high level failed to return a complete SVG in his test.

rss · Simon Willison · Nov 10, 07:28

**「Context」** Small, cheap models have become the default choice for agent loops that make many short calls, and vendors now compete on cost per completed task rather than raw per-token price. Willison argues that per-token comparisons are less meaningful when reasoning tokens cause models to consume very different amounts of compute for the same problem, which is why he cites Artificial Analysis&\#x27;s Intelligence Index versus cost-per-task chart.

**「Practical takeaway」** Teams routing high-volume agent traffic should check prompt length against Ember&\#x27;s 200k-token threshold, since crossing it triples input cost and raises output cost threefold, and should benchmark reasoning levels rather than assuming higher settings produce better output, given Willison&\#x27;s mixed SVG results.

**Tags**: `#LLM release`, `#model pricing`, `#AI agents`, `#Meta AI`, `#efficient models`

---

<a id="item-tech-news-6"></a>
### [XGBoost outage forecast beats NWS/SPC baselines 2.4× on PR-AUC](https://www.reddit.com/r/MachineLearning/comments/1xs4hq8/forecasting_new_power_outages_per_county_hourly_2/) ⭐️ 7.0/10

A single-author project forecasts new county-level power outages two hours ahead for 216 counties in Missouri and Illinois, using XGBoost on HRRR storm forecasts, county facts, current outages, and neighboring-county data. The target is a 5% or greater share of a county&\#x27;s customers newly out during the six hours starting two hours from now, with no credit for outages already underway. Trained on 2020–2024 and tested on 2025 using HRRR forecasts as issued \(the mean of the last five runs\), the model reports PR-AUC of 0.094 versus 0.039 for a rate table of NWS warnings plus the SPC Day 1 outlook, a ratio of about 2.4× with a paired bootstrap range of 2.0–3.3×. At equal alert volume it caught 30% of new outages versus 17%, with precision of 15% versus 11% against a 0.5% base rate; the author reports the system has been live since November 1 with every forecast saved for a blind test.

reddit · r/MachineLearning · /u/CarRepresentative843 · Nov 9, 21:34

**「Context」** The baseline combines two existing public signals: NWS warnings and the Storm Prediction Center&\#x27;s Day 1 outlook, which the author fit as a rate table on the same rows. The model instead consumes HRRR numerical weather forecasts, a higher-resolution input than those categorical products, and the author says the write-up includes a leakage audit and code.

**「Practical takeaway」** The reported precision of 15% at the chosen alert volume means most alerts would still be false positives, so the output is better suited to prioritizing where to look than to triggering action on its own. The author&\#x27;s early transfer test, training only on Missouri and Illinois and evaluating on Iowa, Indiana, and Michigan combined, reports 31% versus 19% caught, suggesting the approach may carry to nearby states, though this is a single-author, non-peer-reviewed result.

**Tags**: `#machine-learning`, `#forecasting`, `#xgboost`, `#power-outages`, `#applied-ml`

---

<a id="item-tech-news-7"></a>
### [JEPA-style tactile pretraining outperforms reconstruction baselines](https://www.reddit.com/r/MachineLearning/comments/1xs05uo/latent_prediction_beats_reconstruction_for/) ⭐️ 7.0/10

Robbyant released LingBot-Touch, a self-supervised tactile encoder that predicts latent representations of masked contact rather than reconstructing raw sensor signals, with inference code and checkpoints already public. On tactile-to-video top-5 recall at 1K hours of data, the JEPA-style model reportedly scores 32.1% versus 5.6% for a same-size MAE baseline and 4.4% for a VAE; at 4K hours it reaches 49.3% while MAE stays under 9% and the VAE falls to 3.1%. The authors attribute the gap to tactile clips being mostly near-zero background, letting reconstruction loss shrink without learning contact. The encoder feeds three sensor types \(magnetic, piezoresistive, visuotactile\) through one shared Transformer using canonical fingertip coordinates and 5D RoPE, with a masking ratio that warms up from 40% to 80% over 300 steps to avoid gradient explosions.

reddit · r/MachineLearning · /u/Zealousideal-War7154 · Nov 9, 18:52

**「Background」** LingBot-Touch is a JEPA-based tactile foundation model that learns a shared representation across piezoresistive, magnetic, and optical \(visuotactile\) sensors using modality-specific tokenizers and a shared Haptic Transformer, pretrained on roughly 5,000 hours of tactile data. The project&\#x27;s public repository currently ships the frozen target encoder and utilities for extracting token-level tactile features, while the paper describes the full method. The reported comparison is against same-size MAE and VAE reconstruction baselines trained on the same data.

**「Impact」** On 26 real robot tasks with 4 policies, frozen LingBot-Touch features scored highest in 89 of 104 policy-and-task combinations, and on a magnetic hand unseen during pretraining LingBot-VLA improved from 57.21 to 75.04. The authors note the Tiny model plateaus around 4K hours while Small keeps improving, indicating scaling data and model size is the next step; teams evaluating the released checkpoints should account for that size-dependent ceiling.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/Robbyant/lingbot-touch">GitHub - Robbyant/lingbot-touch: Learning Heterogeneous ...</a></li>
<li><a href="https://technology.robbyant.com/lingbot-touch">LingBot-Touch Tactile Foundation Model - Robbyant</a></li>
<li><a href="https://arxiv.org/pdf/2611.12806">Learning Heterogeneous Tactile Representation for General ...</a></li>

</ul>
</details>

**Tags**: `#self-supervised-learning`, `#tactile-sensing`, `#robotics`, `#representation-learning`, `#JEPA`

---