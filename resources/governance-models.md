# Models of AI Governance in the Public Sector

**A comparative catalogue of approaches**

Most guidance on public-sector AI is one-size-fits-all: "here is the framework, here are the principles, apply them." But a federal department, a municipal service team, a regulator, and a Crown corporation face genuinely different constraints, and what fits one can be wrong for another. This resource offers a menu of how real institutions actually govern and guardrail AI, organized so you can find the pattern closest to your own and adapt it.

Use it two ways: as a **companion to the [adaptive capacity diagnostic](./adaptive-capacity-diagnostic.md)** — once you have assessed an institution, this suggests governance models suited to its type and weakest dimensions — and as a **reference for the capstone**, where your interventions should match your institution's structure.

Nothing here is endorsed as best. Each model optimizes for something and pays for it somewhere else; the point is to see the trade-off clearly enough to choose.

---

## Part 1 — Why institution type changes the governance problem

A governance model is not portable just because it is good. Four structural features vary across public bodies and change what "govern AI well" even means.

**Accountability line.** A core department answers to a minister and, through them, to the legislature. A Crown corporation answers to a board and a shareholder ministry at arm's length. An independent regulator answers to a statute, sometimes to no minister at all. Who can *compel* an AI decision to be reversed differs in each case; that is the spine of any governance model.

**Risk appetite and exposure.** Central agencies operate under intense political scrutiny, which suppresses risk-taking and produces caution that can itself be a failure. Arm's-length bodies operate with less spotlight which, as this course argues, is exactly where more innovation *and* more unforced error tend to appear, because the external check is weaker and the internal one is doing more work.

**Commercial logic.** A Crown corporation that competes in a market (a utility, a transit authority, a financial entity) has commercial incentives a department does not: speed, cost, competitive advantage. Its AI governance has to reconcile a public mandate with market behaviour, a tension that core departments rarely face.

**Proximity to the public.** A frontline service unit deploys AI where a wrong output hits a citizen immediately: a benefits decision, a wait-list triage. A back-office policy shop using AI for analysis has more distance and more time to catch error. The closer to the citizen, the more the model has to weight contestability and feedback.

> **Reading the rest of this catalogue.** For each model: what it is, who it fits, what it optimizes for, what it costs, and the adaptive-capacity dimensions it most strengthens or neglects. Match to your own institution's type and to the dimensions your diagnostic flagged as weakest. The **"seen in"** examples span jurisdictions deliberately to get across the point that each pattern appears in many systems. They are illustrative instances current as of early 2026 and are not to be interpreted as endorsements. Also, they date quickly. Verify the current state of any before relying on it, and treat the *pattern* as the durable part.

---

## Part 2 — Governance models

### A. Centralized guardrail authority
A single body sets AI policy, approves use cases, and holds a register for the whole organization.

- **Fits:** large departments, whole-of-government central agencies.
- **Optimizes for:** consistency, auditability, a defensible answer to "who approved this."
- **Costs:** slow; a bottleneck that frontline teams route around; distant from where systems actually run.
- **Strengthens:** legitimacy, feedback (central visibility). **Neglects:** structural flexibility, local sensing.
- **Seen in:** the US General Services Administration's AI Governance Board and mandatory enterprise AI inventory, under OMB Memorandum M-25-21 (2025), which requires every AI use case pilot, R&D, or production to be centrally registered before it proceeds.

### B. Federated / tiered model
Central principles and a risk taxonomy; delegated approval, where low-risk uses are self-certified locally and only high-risk uses escalate.

- **Fits:** federated structures, large agencies with capable units, Crown corporations with operating divisions.
- **Optimizes for:** speed where risk is low, scrutiny where risk is high; local ownership.
- **Costs:** only as good as the risk taxonomy; inconsistent if units read it differently; can hide risk that is mis-tiered.
- **Strengthens:** structural flexibility, acting under uncertainty. **Neglects:** consistency, cross-unit legibility.
- **Seen in:** the US federal model under OMB M-25-21, where central policy sets a risk taxonomy but each agency's Chief AI Officer approves and tracks its own use cases and low-risk, limited pilots are exempt from full risk-management requirements if centrally logged. Its documented weakness is exactly the predicted one: capable agencies produce robust governance while under-resourced ones struggle to stand up the basics, yielding a patchwork.

### C. Embedded ethics / review board
A standing multidisciplinary board (legal, ethics, domain, technical, and — at their best — affected-community voices) reviews AI use cases against a rights and equity frame.

- **Fits:** bodies making consequential decisions about people — benefits, health, justice, child welfare.
- **Optimizes for:** catching rights and equity harms before deployment; legitimacy.
- **Costs:** advisory boards without teeth become theatre; slow; can be captured by the programs they review.
- **Strengthens:** legitimacy, feedback and correction. **Neglects:** speed; can create an illusion of oversight (see the maturity-model trap in the diagnostic).
- **Seen in:** New Zealand's Health NZ National AI and Algorithm Expert Advisory Group (2025–26), which reviews and formally endorses specific AI and algorithm uses within the health system before they reach the approving bodies, notably an *arm's-length* health entity supplying its own review where a core department would rely on ministerial oversight. New Zealand's whole-of-government GCDO AI Expert Advisory Panel is the system-level version.

### D. Procurement-gated governance
The main control point is the buying process: vendor standards, model documentation, audit rights, and exit clauses written into contracts.

- **Fits:** institutions that buy rather than build most AI capability — the majority.
- **Optimizes for:** governing capability you do not control; preserving the ability to walk away.
- **Costs:** only as strong as procurement capacity (often weak); governs acquisition, not the use that follows.
- **Strengthens:** absorptive capacity, self-legibility. **Neglects:** ongoing use, in-life monitoring.
- **Seen in:** Canada's Directive on Automated Decision-Making (in force 2020, amended since), which gates deployment behind a mandatory Algorithmic Impact Assessment: a system is scored into one of four impact levels, and higher levels trigger scaled requirements — peer review, notice to affected people, human oversight, and published results — before it can go into production. A gate on use, not just on the contract.

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
- **Seen in:** the UK's Algorithmic Transparency Recording Standard (ATRS), mandatory for central government departments and, tellingly, for arm's-length bodies that deliver public-facing services, the public register had over a hundred published records by early 2026. The Netherlands runs a comparable public algorithm register with several hundred entries. Note the built-in limit: the UK standard is self-declared, with no review or enforcement, so it documents use without gating it.

---

## Part 3 — The arm's-length question

Crown corporations, agencies, regulators, and special operating bodies are where this course expects the most interesting — and most uneven — AI governance, for a reason it names directly: **the spotlight is on core government, so the arm's-length space carries more room for both genuine innovation and unforced error.** Less external scrutiny means the internal check is doing more of the work, and where the internal check is strong that produces real advances, and where it is weak it produces mistakes that surface late.

Four features make their governance genuinely different from a department's, not just a variation on it:

**The accountability gap is a design feature.** Arm's-length bodies are deliberately insulated from day-to-day political direction, but that same insulation weakens the external correction that catches AI failures in core departments. A Crown corporation can deploy a consequential system with no minister answerable for it in Question Period. The governance model has to *supply internally* the check that distance removes, which is why board-level AI literacy, not just management assurance, becomes decisive.

**Commercial mandate collides with public obligation.** A Crown utility or transit or financial body has commercial reasons to move fast on AI: cost, competitiveness, service pressure. Its governance has to hold a public-interest obligation and a market logic at once, a tension a policy department rarely feels. Models that ignore the commercial driver will simply be overridden by it.

**The board is the real governance surface.** In a department, the ultimate AI-governance backstop is ministerial and legislative. In an arm's-length body it is the *board*, which means board composition, board AI literacy, and the board's willingness to ask hard questions are the actual controls. A board that cannot read an AI risk is the single biggest governance vulnerability in this space.

**Regulators governing AI while using it.** Bodies that both *use* AI internally and *regulate* others' use of it carry a conflict worth naming: the standard they hold themselves to and the standard they enforce are rarely the same, and the gap is where credibility is lost.

> **For your assessment.** If the institution you are assessing is arm's-length, add one question to each diagnostic dimension: *who supplies the check that political distance removes?* Where the honest answer is "no one," you have found the weakest point and usually the most useful intervention.

---

## Part 4 — How to use this in the capstone

1. **Identify your institution's type** — core department, arm's-length agency, Crown corporation, regulator, frontline service unit and the four structural features above.
2. **Note which governance models are already in place**, even informally. Most institutions have some blend; name it honestly rather than assuming a blank slate.
3. **Match candidate models to your weakest dimensions.** If the diagnostic flagged feedback and correction, models C and F speak to it; if absorptive capacity, model D; if acting under uncertainty, model E.
4. **State the trade-off you are accepting.** Every model above pays for its strength somewhere. Name what your recommended model costs and who bears that cost — the same discipline the tensions ledger trains.
5. **Apply the H2+/H2− test.** Does the governance model you are proposing build new capacity, or does it relieve pressure and let the current arrangement persist? A review board with no authority, a sandbox with no off-ramp, a transparency register no one acts on — these are H2− dressed as governance.

---

## A closing caution

A catalogue of models invites a particular mistake: adopting one because it is well described rather than because it fits. The models here are starting points for judgment, not a compliance menu. The institution that picks "the transparency model" and publishes a register while changing nothing about how it actually makes decisions has adopted the vocabulary of governance and none of the substance which, as the diagnostic warns, is the failure mode this whole course is built to detect.

---

## Sources for the examples

The "seen in" examples are drawn from public government and institutional sources, current as of early 2026:

- **US GSA AI Governance Board & inventory / OMB M-25-21** — gsa.gov/artificial-intelligence; whitehouse.gov (OMB M-25-21, 2025)
- **US federated model / agency Chief AI Officers** — OMB M-25-21; FAS, "Who Governs Government AI?" (2026)
- **New Zealand Health NZ AI & Algorithm Expert Advisory Group** — healthnz.govt.nz; **GCDO AI Expert Advisory Panel** — digital.govt.nz (2025)
- **Canada Directive on Automated Decision-Making & Algorithmic Impact Assessment** — tbs-sct.canada.ca; canada.ca/responsible-use-ai
- **Norway Datatilsynet AI regulatory sandbox** — datatilsynet.no; **EU AI Act sandbox requirement** — artificialintelligenceact.eu
- **UK Algorithmic Transparency Recording Standard** — gov.uk/algorithmic-transparency-recording-standard; **Netherlands algorithm register** — algoritmes.overheid.nl

Links change and programs evolve; confirm the current state before citing any in your own work — the verification discipline this course asks of every source.
