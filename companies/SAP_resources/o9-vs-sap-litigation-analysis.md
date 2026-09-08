# o9 Solutions v. SAP — Litigation Analysis

**As of:** 2026-09-02 · **Case:** *o9 Solutions, Inc. v. SAP SE, SAP America, Inc., Stephan de Barse, Stijn-Pieter van Houten, Sean Zonneveld*, No. 3:25-cv-03245 (N.D. Tex., Dallas Div.)
**Judges:** District Judge Sam A. Lindsay · Magistrate Judge David L. Horan (pretrial) · **Jury demanded**

---

## 1. Snapshot

| Item | Status |
|---|---|
| Filed | 2025-11-25 |
| Claims | DTSA (18 U.S.C. § 1836), Texas Uniform Trade Secrets Act, breach of contract (NDA / non-solicit / stock option agreements), tortious interference |
| Core allegation | Three senior o9 executives downloaded **>22,000 files** from o9 shared drives before defecting to SAP; SAP allegedly used them in **Integrated Business Planning (IBP)** and related SCM planning products, plus sales/competitive strategy |
| Damages pleaded | **No dollar figure** — lost profits, unjust enrichment, reasonable royalty, exemplary (up to 2× under DTSA for willful/malicious), fees, injunction |
| Latest ruling | **2026-08-11** — Magistrate Horan recommends **denying all defense motions** (12(b)(6) group-pleading, more definite statement, *forum non conveniens* to the Netherlands) |
| Stage | Pleadings — **no answer, no scheduling order, no trial date** |
| SAP accounting treatment | **Not named** in SAP's H1 2026 report; no provision, no contingent-liability disclosure |
| SAP public posture | "We will review o9's complaint and respond, as appropriate, within the legal process" — notably *not* "meritless" |

**The three individuals** (all Dutch nationals, all now in senior SAP roles):

| Name | Role at o9 (departure) | Role at SAP |
|---|---|---|
| Stephan de Barse | Chief Revenue Officer (2025-01-03) | President, Global Business Suite |
| Stijn-Pieter van Houten | SVP, Knowledge Innovation Lead (2025-05-30) | Chief Product Officer, SCM Planning |
| Sean Zonneveld | Global SVP (2025-05-30) | Global CRO, Procurement |

Alleged download pattern: van Houten 9,000+ files on 2024-12-30; Zonneveld 1,200+ files on de Barse's last day; 530+ Henkel account files on 2025-01-31. Eight pleaded trade-secret categories, including the architecture of o9's Digital Brain / Enterprise Knowledge Graph, product roadmap, pricing, and account intelligence.

---

## 2. Current state — where the case actually stands

Ten months of briefing produced one substantive event: SAP tried to get out on the pleadings and on forum grounds, and lost at the magistrate level. Horan found o9's allegations gave "minimally adequate notice" under *Twombly/Iqbal*, and held that although the Netherlands is an adequate forum, defendants did not show it was **significantly more convenient** — they identified no European witnesses, and Texas has a public interest in adjudicating theft from a Texas company.

Two things matter about that:

- **"Minimally adequate" is a low bar, not a merits signal.** Surviving a 12(b)(6) in a trade-secret case says almost nothing about whether o9 can identify its secrets with particularity later, or prove use. The real filters are the trade-secret identification order and summary judgment, both years away.
- **The forum ruling is the more consequential loss for SAP.** SAP wanted this in the Netherlands: no jury, no punitive damages, no US-style discovery, loser-pays fee shifting. Losing that keeps SAP in front of a Dallas jury with its own internal documents discoverable. That single ruling is worth more to o9's settlement leverage than the pleading outcome.

The R&R is a recommendation. Lindsay reviews objections de novo; adoption is likely but not automatic, and district judges do occasionally trim R&Rs on forum questions.

**Accounting tell:** SAP disclosed and provisioned the Teradata matter, and settled it for $480m / €408m in Feb 2026. o9 appears nowhere in the H1 2026 report. Under IAS 37 that means SAP does not currently regard a loss as probable and reliably estimable. A first appearance of o9 in the contingent-liabilities note would be a genuine change of state.

---

## 3. Merits — what each side actually has

**o9's strengths**

- Forensic download logs are the strongest evidence type in trade-secret litigation: volume, timing (bulk pulls in the weeks before departure), and correlation with resignations are hard to explain innocently.
- Three coordinated departures into *directly competitive* senior roles supports the "inevitable use" narrative and the tortious-interference count.
- Contract claims against the individuals are largely independent of the trade-secret merits — o9 can lose the DTSA claim and still win breach.
- Jury venue in the plaintiff's home district; Kirkland & Ellis on the file.

**SAP's defenses**

- **Possession ≠ use.** The central battleground. o9 must show SAP incorporated the material into IBP or its planning roadmap. SAP will argue the executives were hired for domain expertise, that IBP's architecture predates them by two decades, and that o9's "secrets" are industry-general planning concepts or already public in marketing and product documentation.
- **Identification with particularity.** Eight categories is a pleading construct. Courts routinely force plaintiffs to name specific secrets before discovery; broad categories like "competitive intelligence" and "business proposals" are vulnerable.
- **Secrecy and value.** Sales roadmaps and account plans go stale in months — weak candidates for meaningful damages even if misappropriated.
- **Causation / apportionment.** Even if some material was used, SAP will argue de minimis contribution to IBP revenue, and that o9's growth did not suffer.
- **Clean-up posture.** If SAP quarantined the files on notice and can prove it, that guts exemplary damages and much of the injunctive case.

**Honest read:** the intake facts look bad for the individuals and materially worse than a typical departing-employee case. The leap from "they took files" to "SAP built product with them" is the one o9 has not yet been required to prove, and it is where cases of this shape usually thin out.

---

## 4. Expected timeline

| Window | Expected milestone |
|---|---|
| Q3–Q4 2026 | Lindsay rules on objections; R&R adopted (likely). SAP and individuals answer. |
| Q4 2026 – Q1 2027 | Rule 26(f) conference, scheduling order, protective order. First trial date *set* here — expect a paper date in 2028 that slips. |
| 2027 | Trade-secret identification fight; document discovery; cross-border friction — SAP SE is German, the three individuals Dutch, so Hague Evidence Convention requests, GDPR and EU blocking-statute objections. This phase adds a year. |
| H1 2028 | Depositions of the three executives and SAP product leadership. **Peak settlement pressure** — the depositions are the reputational risk event. |
| Late 2028 – 2029 | Expert reports, *Daubert*, summary judgment. Second real settlement window, post-ruling. |
| 2029–2030 | Trial, if it gets there. Appeal adds 18–30 months. |

Base case: **settlement in 2028**, before or shortly after summary judgment. Teradata v. SAP is the reference — filed 2018, settled on the eve of trial in Feb 2026, ~7.5 years. SAP's demonstrated pattern is to litigate hard and pay late.

Probability of an actual jury verdict: **~15–20%**.

---

## 5. Damage to SAP

### 5.1 Financial exposure

DTSA allows actual loss **plus** unjust enrichment (non-duplicative), or a reasonable royalty; up to **2× exemplary** for willful and malicious misappropriation; plus fees. The plaintiff-side anchor will be unjust enrichment tied to SAP's IBP/planning franchise, not o9's lost profits — SAP will attack it on apportionment.

Scale context: o9 is private, ~$3.7bn valuation (2023), ARR ~$200m in 2023 growing ~37%, so plausibly $350–500m now, 200+ customers, ~2,500 staff. SAP: ~€40bn revenue run-rate, ~€3bn quarterly FCF, ~$252bn market cap (2026-08-25).

| Scenario | Subjective probability | Cash cost to SAP |
|---|---|---|
| Defense win (SJ or verdict) or de minimis outcome | ~20% | Legal fees only, ~$30–60m cumulative |
| Nuisance / early settlement, narrow terms | ~20% | $50–150m |
| **Mid-case settlement post-discovery (base case)** | **~40%** | **$200–600m** |
| Large settlement or adverse verdict | ~15% | $600m–1.5bn |
| Tail: willful finding + exemplary doubling + fees | ~5% | >$1.5bn |

Comparables: **Teradata/SAP $480m** (2026, settled); Epic Systems v. TCS $940m verdict cut to $420m; Motorola v. Hytera $543m; Waymo/Uber $245m in equity; Appian v. Pegasystems $2.04bn **vacated on appeal**; Title Source v. HouseCanary $706m **reversed**. Headline trade-secret verdicts survive appeal poorly — which is exactly why defendants settle at a discount to the verdict tail and plaintiffs accept it.

**Materiality:** even the base case is roughly one to two months of SAP free cash flow, ~0.1–0.25% of market cap, and a one-time non-IFRS add-back. SAP absorbed €408m for Teradata in Q1 2026 without disturbing guidance. **On money alone this is not a thesis-changing event.**

### 5.2 Non-financial damage — where the real risk sits

Ranked by how much it could actually matter:

1. **Injunctive relief against IBP/SCM planning.** A product-level injunction against IBP is very unlikely — courts don't enjoin flagship enterprise products years after the fact when money is adequate. Realistically available: quarantine/return of files, a use injunction on specifically identified secrets, possibly a time-limited "head start" injunction on particular roadmap features. Low probability of product impact, but it is the only outcome that touches the growth story rather than the cash balance.
2. **Personnel remedy.** de Barse is **President of Global Business Suite** — not a peripheral hire. A negotiated or court-ordered wall, role change, or departure for any of the three would be a visible governance event, landing awkwardly against the "Autonomous Enterprise" leadership narrative from the Q2 2026 call.
3. **Competitive sales friction.** o9, Kinaxis, Blue Yonder and Anaplan will use the complaint in supply-chain planning bake-offs. SAP is mid-way through pushing the APO base to IBP ahead of the 2027 sunset — a live migration decision is exactly when procurement committees are most sensitive to "is this product under an IP cloud?" Most probable form of real damage, and the least measurable.
4. **Reputational overlay.** Teradata → Celonis → o9 invites a "serial IP defendant" framing from short-side research and press. Narrative only — unless discovery produces a genuinely bad internal document, in which case it becomes the story.
5. **Management distraction and discovery cost.** Depositions of a division president and a CPO, plus preservation/collection across German and US entities, during a headcount freeze and an agent-platform roadmap year.

### 5.3 What would change the assessment

- o9 appearing in SAP's contingent-liability note, or a provision being taken → management now views loss as probable.
- The trade-secret identification order: forced narrowing to a handful of specific technical secrets compresses exposure sharply; broad technical categories surviving into discovery keeps the unjust-enrichment theory alive.
- Any preliminary injunction motion by o9 — **none filed to date**, which is notable and favours SAP.
- SAP counterclaims, or a countersuit in Germany/Netherlands.
- Departure or reassignment of any of the three executives.

---

## 6. Bottom line

The case survived its first real test and SAP lost the forum fight it most wanted to win, which raises the settlement price. But this is a pleadings-stage case with no trial date, a base-case resolution in 2028, and a most-likely cost of a few hundred million dollars — meaningful as a headline, immaterial against ~€40bn of revenue and a $252bn market cap. The exposure that would actually matter is not the damages number; it is (a) an injunction or discovery finding touching the IBP roadmap during the APO-sunset migration window, or (b) a senior-personnel consequence for de Barse. Both are currently low-probability.

Treat the litigation as a modest, quantifiable overhang and a small competitive headwind in supply-chain planning deals — not as a variable in the cloud/CCB growth case.

---

*Not legal or investment advice. Probability estimates and damage ranges are my own judgement, not sourced figures. No damages amount has been pleaded, and no scheduling order or trial date exists in the docket as of this writing.*

**Sources:** [o9 press release](https://o9solutions.com/news/o9-solutions-files-trade-secret-misappropriation-complaint-against-sap-and-former-o9-executives-in-u-s-district-court) · [IPWatchdog on the Aug 11 R&R](https://ipwatchdog.com/2026/08/12/magistrate-judge-recommends-denying-motion-to-dismiss-trade-secret-case-against-sap/) · [Bloomberg Law](https://news.bloomberglaw.com/ip-law/sap-cant-escape-or-move-ai-firms-trade-secrets-case-abroad) · [Justia docket 3:25-cv-03245](https://dockets.justia.com/docket/texas/txndce/3:2025cv03245/412244) · [FreightWaves](https://www.freightwaves.com/news/o9-solutions-accuses-sap-of-trade-secret-theft-in-high-stakes-supply-chain-software-dispute) · [D CEO](https://www.dmagazine.com/business-economy/2025/11/dallas-tech-firm-o9-solutions-accuses-sap-of-a-coordinated-attack-in-trade-secrets-lawsuit/) · [LegalClarity](https://legalclarity.org/o9-sap-lawsuit-trade-secret-theft-allegations-explained/) · [SAP H1 2026 report](https://www.sap.com/docs/download/investors/2026/sap-2026-half-year-report.pdf) · [Teradata settlement](https://news.bloomberglaw.com/antitrust/teradata-sap-reach-480-million-settlement-in-antitrust-ip-row) · [Contrary Research on o9](https://research.contrary.com/company/o9-solutions)
