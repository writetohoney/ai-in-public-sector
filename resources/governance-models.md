# Models of AI Governance in the Public Sector

**A comparative catalogue — approaches, not answers.**

Most guidance on public-sector AI is one-size-fits-all: here is the framework, here are the principles, apply them. But a federal department, a municipal service team, a regulator, and a Crown corporation face genuinely different constraints, and what fits one can be wrong for another. This resource is the opposite. It is a menu of how real institutions actually govern and guardrail AI, organized so you can find the pattern closest to your own and adapt it.

Use it two ways: as a **companion to the [adaptive capacity diagnostic](./adaptive-capacity-diagnostic.md)** — once you have assessed an institution, this suggests governance models suited to its type and weakest dimensions — and as a **reference for the capstone**, where your interventions should match your institution's structure, not a generic ideal.

Nothing here is endorsed as best. Each model optimizes for something and pays for it somewhere else; the point is to see the trade-off clearly enough to choose.

---

## Part 1 — Why institution type changes the governance problem

A governance model is not portable just because it is good. Four structural features vary across public bodies and change what "govern AI well" even means.

**Accountability line.** A core department answers to a minister and, through them, to the legislature. A Crown corporation answers to a board and a shareholder ministry at arm's length. An independent regulator answers to a statute, sometimes to no minister at all. Who can *compel* an AI decision to be reversed differs in each case — and that is the spine of any governance model.

**Risk appetite and exposure.** Central agencies operate under intense political scrutiny, which suppresses risk-taking and produces caution that can itself be a failure. Arm's-length bodies operate with less spotlight — which, as this course argues, is exactly where more innovation *and* more unforced error tend to appear, because the external check is weaker and the internal one is doing more work.

**Commercial logic.** A Crown corporation that competes in a market (a utility, a transit authority, a financial entity) has commercial incentives a department does not: speed, cost, competitive advantage. Its AI governance has to reconcile a public mandate with market behaviour — a tension core departments rarely face.

**Proximity to the public.** A frontline service unit deploys AI where a wrong output hits a citizen immediately — a benefits decision, a wait-list triage. A back-office policy shop using AI for analysis has more distance and more time to catch error. The closer to the citizen, the more the model has to weight contestability and feedback.

> **Reading the rest of this catalogue.** For each model: what it is, who it fits, what it optimizes for, what it costs, and the adaptive-capacity dimensions it most strengthens or neglects. Match to your own institution's type and to the dimensions your diagnostic flagged as weakest. The **"seen in"** examples span jurisdictions deliberately — the point is that each pattern appears in many systems, not one. They are illustrative instances current as of early 2026, not endorsements, and they date quickly; verify the current state of any before relying on it, and treat the *pattern* as the durable part.

---

## Part 2 — Governance models

### A. Centralized guardrail authority
A single body sets AI policy, approves use cases, and holds a register for the whole organization.

- **Fits:** large departments, whole-of-government central agencies.
- **Optimizes for:** consistency, auditability, a defensible answer to "who approved this."
- **Costs:** slow; a bottleneck that frontline teams route around; distant from where systems actually run.
- **Strengthens:** legitimacy, feedback (central visibility). **Neglects:** structural flexibility, local sensing.
- **Seen in:** the US General Services Administration's AI Governance Board and mandatory enterprise AI inventory, under OMB Memorandum M-25-21 (2025), which requires every AI use case — pilot, R&D, or production — to be centrally registered before it proceeds.

### B. Federated / tiered model
Central principles and a risk taxonomy; delegated approval, where low-risk uses are self-certified locally and only high-risk uses escalate.

- **Fits:** federated structures, large agencies with capable units, Crown corporations with operating divisions.
- **Optimizes for:** speed where risk is low, scrutiny where risk is high; local ownership.
- **Costs:** only as good as the risk taxonomy; inconsistent if units read it differently; can hide risk that is mis-tiered.
- **Strengthens:** structural flexibility, acting under uncertainty. **Neglects:** consistency, cross-unit legibility.
- **Seen in:** the US federal model under OMB M-25-21, where central policy sets a risk taxonomy but each agency's Chief AI Officer approves and tracks its own use cases — and low-risk, limited pilots are exempt from full risk-management requirements if centrally logged. Its documented weakness is exactly the predicted one: capable agencies produce robust governance while under-resourced ones struggle to stand up the basics, yielding a patchwork.

### C. Embedded ethics / review board
A standing multidisciplinary board (legal, ethics, domain, technical, and — at their best — affected-community voices) reviews AI use cases against a rights and equity frame.

- **Fits:** bodies making consequential decisions about people — benefits, health, justice, child welfare.
- **Optimizes for:** catching rights and equity harms before deployment; legitimacy.
- **Costs:** advisory boards without teeth become theatre; slow; can be captured by the programs they review.
- **Strengthens:** legitimacy, feedback and correction. **Neglects:** speed; can create an illusion of oversight (see the maturity-model trap in the diagnostic).
- **Seen in:** New Zealand's Health NZ National AI and Algorithm Expert Advisory Group (2025–26), which reviews and formally endorses specific AI and algorithm uses within the health system before they reach the approving bodies — notably, an *arm's-length* health entity supplying its own review where a core department would rely on ministerial oversight. New Zealand's whole-of-government GCDO AI Expert Advisory Panel is the system-level version.

### D. Procurement-gated governance
The main control point is the buying process: vendor standards, model documentation, audit rights, and exit clauses written into contracts.

- **Fits:** institutions that buy rather than build most AI capability — the majority.
- **Optimizes for:** governing capability you do not control; preserving the ability to walk away.
- **Costs:** only as strong as procurement capacity (often weak); governs acquisition, not the use that follows.
- **Strengthens:** absorptive capacity, self-legibility. **Neglects:** ongoing use, in-life monitoring.
- **Seen in:** the EU AI Act's Fundamental Rights Impact Assessment (Article 27, applying from August 2026). Before deploying a high-risk system, public bodies — and private entities delivering public services — must assess who could be harmed, how, what human oversight applies, and what happens if the risk materialises, then notify the market-surveillance authority, before the system goes live. A gate on use, tied explicitly to public-service delivery rather than to the contract. New Zealand requires comparable algorithmic impact assessments for high-risk public-sector systems — social welfare, policing, border — under its Public Service AI Framework.

### E. Regulatory-sandbox / staged-permission model
A defined space to trial AI with real data under supervision and constraints, with staged expansion as evidence accumulates.

- **Fits:** regulators, innovation-mandated agencies, arm's-length bodies with room to experiment.
- **Optimizes for:** learning under real conditions; failing small; acting under uncertainty without betting the institution.
- **Costs:** needs a genuine off-ramp — a sandbox no one is allowed to fail in is a pilot in disguise; hard to scale out of.
- **Strengthens:** acting under uncertainty, sensing. **Neglects:** consistency at scale, legitimacy if the public is unaware they are in the trial.
- **Seen in:** Norway's Data Protection Authority (Datatilsynet) AI regulatory sandbox, running since 2020, where selected projects test AI systems against data-protection law with the regulator's iterative guidance. The EU AI Act now requires every member state to stand up a national sandbox, and Singapore and Utah run their own — a model moving from experiment to expectation.

### F. Radical-transparency model
Public registers of algorithms, published impact assessments, open reporting of automated decisions and their error rates.

- **Fits:** bodies whose legitimacy depends on visible trust; those under freedom-of-information regimes already.
- **Optimizes for:** external accountability; legitimacy that precedes rather than follows the scandal.
- **Costs:** transparency without capacity to act on what it reveals is a liability catalogue; can chill useful experimentation.
- **Strengthens:** legitimacy, feedback. **Neglects:** speed; offers little if no one acts on what is disclosed.
- **Seen in:** the UK's Algorithmic Transparency Recording Standard (ATRS), mandatory for central government departments and, tellingly, for arm's-length bodies that deliver public-facing services — the public register had over a hundred published records by early 2026. The Netherlands runs a comparable public algorithm register with several hundred entries. Note the built-in limit: the UK standard is self-declared, with no review or enforcement, so it documents use without gating it.

---

### G. Voluntary framework / soft-law model
Detailed non-binding guidance, testing toolkits, and self-assessment rather than statutory requirements — governance by standard-setting and reputation rather than by law.

- **Fits:** jurisdictions and bodies prioritizing innovation speed; sectors where a hard-law regime would lag the technology.
- **Optimizes for:** flexibility, keeping pace with fast-moving capability, low compliance friction.
- **Costs:** no enforcement teeth — compliance depends on incentive and reputation; weaker recourse when something goes wrong.
- **Strengthens:** sensing, acting under uncertainty. **Neglects:** legitimacy and feedback where a binding remedy is needed.
- **Seen in:** Singapore's Model AI Governance Framework (first issued 2019, updated 2020, with a Generative AI edition in 2024 and an Agentic AI edition in January 2026), paired with the AI Verify testing toolkit — detailed, voluntary, and deliberately pro-innovation rather than legislated. A contrast with the EU's hard-law route, and a reminder that "govern first" and "deliver first" are choices a jurisdiction makes, not a maturity ranking.

### H. Coordinating / capacity-building framework
A framework whose primary work is not to *constrain* AI but to *build the conditions* for governing it at all — shared infrastructure, data governance, skills, and coordination across many governments at very different starting points.

- **Fits:** continental or regional bodies; jurisdictions where the binding constraint is capacity, infrastructure, and compute rather than the absence of rules.
- **Optimizes for:** sovereignty, coordination, and building governance capability where it does not yet exist; asserting a regional voice against dependence on foreign models and cloud providers.
- **Costs:** ambition can outrun implementation — the framework exists on paper while infrastructure, funding, and skills lag, and benefits concentrate in the few best-resourced members.
- **Strengthens:** sensing, absorptive capacity (treated as things to *build*, not assume). **Neglects:** enforceable individual redress, which depends on national law that may not yet exist.
- **Seen in:** the African Union's Continental AI Strategy (endorsed July 2024, implementing 2025–2030), an Africa-centric, development-focused framework across 55 member states that calls for an African Charter on Trustworthy AI and treats data governance and technological sovereignty as central. Independent analysis (Future of Privacy Forum, Carnegie, OECD) notes the core tension the model makes visible: comprehensive continental ambition alongside severe infrastructure, compute, and capacity constraints — governance as something a jurisdiction must first build the conditions to do at all. This is the governance problem for much of the world, and the Global-North models above quietly assume it away.

### I. Rights-based statutory model, treaty-anchored
Comprehensive AI legislation grounded in fundamental rights and data-protection law — and, distinctively, tied to a *supranational* human-rights body whose jurisdiction the state has accepted.

- **Fits:** jurisdictions with a strong data-protection tradition and binding regional human-rights commitments.
- **Optimizes for:** enforceable individual rights, external accountability that a government cannot unwind on its own, alignment with existing privacy law.
- **Costs:** slow legislative passage; heavy for institutions to implement; can lag the technology it regulates.
- **Strengthens:** legitimacy, feedback and correction. **Neglects:** speed and flexibility; risks becoming compliance-heavy.
- **Seen in:** Brazil's AI Bill (PL 2338/2023), approved by the Senate in December 2024 and under review in the Chamber of Deputies — a risk-based framework aligned with Brazil's data-protection law (LGPD) and, uniquely, the first comprehensive AI regulation to cross-reference Inter-American Human Rights System obligations in its operational provisions. Governance whose backstop sits partly *outside* the national government, in a regional court.

### J. State-led / execution-first model
AI governance fused with industrial and economic strategy and driven from the centre of government — the state as builder, funder, and first adopter, with a dedicated minister or office and sovereign investment behind it.

- **Fits:** centralized states with strong executive capacity and the fiscal room to invest directly; governments treating AI as a national-development engine.
- **Optimizes for:** speed, scale, coordination, and rapid deployment across public services; attracting investment and talent.
- **Costs:** oversight and contestability can lag deployment; concentrating both the "build" and the "govern" roles in the same central authority weakens the independent check.
- **Strengthens:** structural flexibility, acting under uncertainty. **Neglects:** the external, arm's-length scrutiny that catches error — the state is marking its own homework.
- **Seen in:** the United Arab Emirates, which appointed the world's first Minister of State for Artificial Intelligence in 2017, runs a National AI Strategy 2031, has committed sovereign-scale investment to compute and data centres, and announced a target for half of government services to be delivered through AI agents. Governance as accelerant rather than brake — the opposite pole from the rights-first models, and a useful stress test of the assumption that "governance" always means "constraint."

---

## Part 3 — The arm's-length question

Crown corporations, agencies, regulators, and special operating bodies are where this course expects the most interesting — and most uneven — AI governance, for a reason it names directly: **the spotlight is on core government, so the arm's-length space carries more room for both genuine innovation and unforced error.** Less external scrutiny means the internal check is doing more of the work, and where the internal check is strong that produces real advances, and where it is weak it produces mistakes that surface late.

Four features make their governance genuinely different from a department's, not just a variation on it:

**The accountability gap is a design feature, not a flaw.** Arm's-length bodies are deliberately insulated from day-to-day political direction — that is the point of them. But that same insulation weakens the external correction that catches AI failures in core departments. A Crown corporation can deploy a consequential system with no minister answerable for it in Question Period. The governance model has to *supply internally* the check that distance removes — which is why board-level AI literacy, not just management assurance, becomes decisive.

**Commercial mandate collides with public obligation.** A Crown utility or transit or financial body has commercial reasons to move fast on AI — cost, competitiveness, service pressure. Its governance has to hold a public-interest obligation and a market logic at once, a tension a policy department rarely feels. Models that ignore the commercial driver will simply be overridden by it.

**The board is the real governance surface.** In a department, the ultimate AI-governance backstop is ministerial and legislative. In an arm's-length body it is the *board* — which means board composition, board AI literacy, and the board's willingness to ask hard questions are the actual controls. A board that cannot read an AI risk is the single biggest governance vulnerability in this space.

**Regulators governing AI while using it.** Bodies that both *use* AI internally and *regulate* others' use of it carry a conflict worth naming: the standard they hold themselves to and the standard they enforce are rarely the same, and the gap is where credibility is lost.

> **For your assessment.** If the institution you are assessing is arm's-length, add one question to each diagnostic dimension: *who supplies the check that political distance removes?* Where the honest answer is "no one," you have found the weakest point — and usually the most useful intervention.

---

## Part 4 — How to use this in the capstone

1. **Identify your institution's type** — core department, arm's-length agency, Crown corporation, regulator, frontline service unit — and the four structural features above.
2. **Note which governance models are already in place**, even informally. Most institutions have some blend; name it honestly rather than assuming a blank slate.
3. **Match candidate models to your weakest dimensions.** If the diagnostic flagged feedback and correction, models C and F speak to it; if absorptive capacity, model D; if acting under uncertainty, model E.
4. **State the trade-off you are accepting.** Every model above pays for its strength somewhere. Name what your recommended model costs and who bears that cost — the same discipline the tensions ledger trains.
5. **Apply the H2+/H2− test.** Does the governance model you are proposing build new capacity, or does it relieve pressure and let the current arrangement persist? A review board with no authority, a sandbox with no off-ramp, a transparency register no one acts on — these are H2− dressed as governance.

---

## A closing caution

A catalogue of models invites a particular mistake: adopting one because it is well described rather than because it fits. The models here are starting points for judgment, not a compliance menu. The institution that picks "the transparency model" and publishes a register while changing nothing about how it actually makes decisions has adopted the vocabulary of governance and none of the substance — which, as the diagnostic warns, is the failure mode this whole course is built to detect.

## Where this catalogue is thin

These ten models are types, not a census, and the sample is uneven. It is strongest on Europe, North America, and East Asia; it now reaches Africa, Latin America, and the Gulf, but with one example each, and it is silent on South and Southeast Asia beyond Singapore, on China's distinct state-and-Party model, and on most of the Global South. Two consequences worth holding: first, the *types* are more portable than the *examples* — a pattern found in one country usually appears in others, so look for the pattern, not the flag; second, an approach's absence here says nothing about its quality, only about the limits of one teaching resource assembled at one moment. If you know a model this catalogue is missing — especially from a system under-represented above — that is a contribution worth making back to it.

---

## Sources for the examples

The "seen in" examples are drawn from public government and institutional sources, current as of early 2026:

- **US GSA AI Governance Board & inventory / OMB M-25-21** — gsa.gov/artificial-intelligence; whitehouse.gov (OMB M-25-21, 2025)
- **US federated model / agency Chief AI Officers** — OMB M-25-21; FAS, "Who Governs Government AI?" (2026)
- **New Zealand Health NZ AI & Algorithm Expert Advisory Group** — healthnz.govt.nz; **GCDO AI Expert Advisory Panel** — digital.govt.nz (2025)
- **Singapore Model AI Governance Framework & AI Verify** — aiverifyfoundation.sg; imda.gov.sg
- **African Union Continental AI Strategy (2024)** — au.int; analysis via Future of Privacy Forum (fpf.org) and Carnegie Endowment
- **Brazil AI Bill (PL 2338/2023)** — Senado Federal; Library of Congress Global Legal Monitor; aligned with the LGPD
- **UAE National AI Strategy 2031 & Minister of State for AI** — ai.gov.ae; IAPP Global AI Governance profile
- **EU AI Act Fundamental Rights Impact Assessment (Art. 27)** — artificialintelligenceact.eu/article/27; **New Zealand Public Service AI Framework & algorithmic impact assessments** — digital.govt.nz
- **Norway Datatilsynet AI regulatory sandbox** — datatilsynet.no; **EU AI Act sandbox requirement** — artificialintelligenceact.eu
- **UK Algorithmic Transparency Recording Standard** — gov.uk/algorithmic-transparency-recording-standard; **Netherlands algorithm register** — algoritmes.overheid.nl

Links change and programs evolve; confirm the current state before citing any in your own work — the verification discipline this course asks of every source.
