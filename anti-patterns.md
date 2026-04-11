# Anti-Patterns — Dialectical Thinking (矛盾论)

Six failure modes in dialectical reasoning. Each pattern includes what it looks like, why it fails, and how to fix it.

---

## 1. Pseudo-synthesis (伪综合)

### What it looks like

Appears to combine both sides of a contradiction but actually picks one side and adds cosmetic elements of the other. The "synthesis" is a dressed-up version of the preferred position.

### Example

**Contradiction**: Engineering wants to build a robust platform; Sales wants to ship features fast.

**Pseudo-synthesis**: "We'll build a robust platform AND ship features fast by working harder and being more efficient."

This is not synthesis — it's picking "ship fast" and adding "robust" as an adjective. Nothing structural changed. The contradiction is papered over, not resolved.

**Genuine synthesis**: "We decouple the platform core (monthly releases, high stability bar) from the feature layer (weekly releases, lower stability bar). Engineering owns core stability, feature teams own velocity. The contradiction transforms from 'speed vs quality' to 'which layer does this change belong to?' — a classification problem, not a trade-off."

### Why it fails

Pseudo-synthesis satisfies no one. Engineering sees through the "robust" label when deadlines keep overriding quality. Sales sees through the "fast" label when platform work keeps delaying features. The underlying contradiction festers because it was never actually addressed.

### Detection test

Ask: "Would the steel-manned opposition accept this synthesis as genuinely incorporating their concerns?" If Engineering would say "you just told us to ship faster with nicer words," it's pseudo-synthesis.

### Fix

- Steel-man both sides fully before attempting synthesis.
- The synthesis must change the structure of the situation, not just the description.
- If you can't find a genuine synthesis, be honest: name which side you're prioritizing and why.

---

## 2. Contradiction avoidance (矛盾回避)

### What it looks like

Treats contradictions as "factors to balance" or "trade-offs to optimize." Uses optimization language to avoid naming the opposing forces directly. Everything becomes a multi-criteria decision problem instead of a dialectical one.

### Example

**Situation**: A company needs to decide between investing in its existing product line or building a new one.

**Avoidance**: "We should allocate 70% to existing products and 30% to new products, balancing innovation with stability."

This treats the contradiction as a resource allocation problem. But the real contradiction may be: the existing product's architecture prevents the new product from being built — they share infrastructure, and optimizing for one degrades the other. No percentage split addresses this.

**Dialectical approach**: "The principal contradiction is that our infrastructure is optimized for Product A's workload patterns, which are fundamentally incompatible with Product B's requirements. The resolution is not allocation — it's architectural separation. Once separated, both can be invested in freely."

### Why it fails

Contradiction avoidance eliminates the engine of development. Contradictions drive change — they reveal where the system needs to transform. Treating them as "factors" to optimize keeps the system in its current structure, which may be the actual problem.

Mao: "矛盾是事物发展的动力" — contradiction is the motive force of development. Avoiding contradictions means avoiding development.

### Detection test

Check your language: Are you using "balance," "trade-off," "optimize," "allocate"? These words may indicate you're avoiding a contradiction. Replace with: "What two forces are pulling in opposite directions here?"

### Fix

- Name the opposing forces explicitly as "X vs Y."
- If everything in your analysis is a "factor" with a weight, you haven't found the contradictions yet.
- Ask: "What would have to change structurally if one side won completely?" The answer reveals the real contradiction.

---

## 3. Template application (模板套用)

### What it looks like

Applying a contradiction analysis from one situation to a different situation without fresh examination. "Last time the principal contradiction was growth vs profitability, so it must be this time too." Universality without particularity.

### Example

**Template**: "In every startup, the principal contradiction is growth vs profitability."

**Reality**: Company A's principal contradiction is actually founder alignment — the co-founders have incompatible visions for the product. Growth vs profitability is secondary; it would resolve itself once the founders agree on direction. But the template analysis keeps everyone focused on burn rate and revenue, while the real contradiction (the founders) goes unaddressed.

### Why it fails

Mao: "矛盾的普遍性寓于特殊性之中" — universality resides in particularity. Yes, all businesses face growth vs profitability at some point. But in THIS business, at THIS moment, THAT may not be the principal contradiction. Template analysis misses the specific configuration of forces.

### Detection test

Ask: "Did I identify this as the principal contradiction through analysis of THIS situation, or did I import it from a previous situation?" If you can't describe the specific evidence that pointed you here, you're applying a template.

### Fix

- Analyze each situation's contradiction network from scratch.
- Use previous analyses as hypotheses to test, not conclusions to apply.
- The same organization can have different principal contradictions in different quarters, departments, or product lines.

---

## 4. Principal-secondary confusion (主次混淆)

### What it looks like

Spending energy and resources on secondary contradictions while the principal contradiction remains unaddressed. Often happens because secondary contradictions are more visible, more comfortable to address, or have louder advocates.

### Example

**Situation**: A product team is losing market share. They spend three months redesigning the UI (secondary: user experience vs legacy interface) while the principal contradiction is that their pricing model is incompatible with the market segment they're targeting (pricing structure vs market position).

The UI redesign may even succeed — the product looks better. But market share keeps declining because the principal contradiction (pricing) was never addressed. The team feels productive but is solving the wrong problem.

### Why it fails

Secondary contradictions are often symptoms of the principal one. Treating symptoms doesn't resolve the underlying disease. Worse, it creates the illusion of progress, delaying the reckoning with the principal contradiction.

Mao: "抓住了主要矛盾，一切问题就迎刃而解" — grasp the principal contradiction and all problems can be readily solved.

### Detection test

For each contradiction you're addressing, ask: "If I resolve this, do the other contradictions simplify?" If yes, you may have the principal one. If resolving it changes nothing about the other contradictions, you're working on a secondary one.

### Fix

- Before committing resources, explicitly rank contradictions by structural leverage.
- The principal contradiction test: resolution transforms the network.
- Be suspicious of contradictions that are easy to address, comfortable to discuss, or have the loudest advocates. The principal contradiction is often the one people are avoiding.

---

## 5. Nature misjudgment (性质误判)

### What it looks like

Using the wrong resolution method for the type of contradiction. Two common forms:
- **Negotiating the irreconcilable**: Trying to find compromise when the sides are fundamentally incompatible.
- **Forcing the reconcilable**: Using decisive action to eliminate one side when both sides serve legitimate functions.

### Example — Negotiating the irreconcilable

**Situation**: A company's core product is a privacy-focused messaging app. A new VP of Growth wants to monetize user data for advertising.

**Mismatched approach**: "Let's find a middle ground — maybe we can use anonymized data for targeted ads while maintaining our privacy commitment."

This is an irreconcilable contradiction. The company's identity, user trust, and product value are built on privacy. Advertising monetization of user data, even "anonymized," fundamentally undermines the product's reason for existence. The "middle ground" satisfies neither privacy advocates nor growth targets.

**Correct approach**: Recognize this as antagonistic. Choose: either the company is a privacy product (and finds privacy-compatible revenue) or it pivots to an advertising model (and rebuilds its value proposition). Trying to be both destroys both.

### Example — Forcing the reconcilable

**Situation**: Marketing wants brand consistency; regional teams want local adaptation.

**Mismatched approach**: "All materials must be approved by central marketing. No exceptions." This eliminates local adaptation entirely — a legitimate function that serves real market differences.

**Correct approach**: Recognize this as non-antagonistic. Both brand consistency and local adaptation serve the same ultimate goal (effective marketing). Redesign: brand guidelines as guardrails (central), execution within guardrails (local). Like Deng's "one country, two systems" — structural coexistence, not winner-take-all.

### Why it fails

Negotiating the irreconcilable wastes time and produces weak outcomes that satisfy no one. Forcing the reconcilable destroys value unnecessarily and creates resentment.

Mao's《关于正确处理人民内部矛盾的问题》: the nature of the contradiction determines the method. Antagonistic contradictions require struggle (斗争); non-antagonistic contradictions require democratic methods (民主方法).

### Detection test

Ask: "Can both sides coexist in a redesigned system, or is one fundamentally incompatible with the system's identity/purpose?" If coexistence is possible, it's reconcilable — redesign. If one side's existence negates the other's, it's irreconcilable — choose.

### Fix

- Always judge the nature before choosing the method.
- For reconcilable contradictions: look for structural redesigns, governance frameworks, "both/and" architectures.
- For irreconcilable contradictions: make a clear choice, communicate it directly, and commit to the consequences.
- When unsure: ask "what happens if we try to maintain both?" If the answer is "both sides degrade," it's likely irreconcilable.

---

## 6. Static analysis (静态分析)

### What it looks like

Analyzing the contradiction network once and treating it as permanently valid. Executing a plan based on the initial analysis without checking whether the landscape has shifted. Treating a dynamic system as a photograph.

### Example

**Quarter 1 analysis**: "Our principal contradiction is product-market fit vs engineering capacity. We need to hire more engineers."

**Quarter 3 reality**: They hired the engineers. The product now has strong PMF. But the principal contradiction has shifted: it's now sales execution vs product complexity — the product is too complex for the sales team to demo effectively. The company is still hiring engineers based on the Q1 analysis, when the principal contradiction moved to sales enablement months ago.

### Why it fails

Contradictions transform. When you act on the principal contradiction, the network reshapes. What was secondary becomes principal. What was irreconcilable may become reconcilable as conditions change (or vice versa).

Mao: "矛盾的各方面，在一定条件下，向着其相反的方面转化" — under certain conditions, each aspect of a contradiction transforms into its opposite.

### Detection test

Ask: "When was the last time I re-mapped the contradiction network?" If the answer is "at the beginning of the project/quarter/strategy cycle," you're doing static analysis. The network should be re-examined after every major action or environmental shift.

### Fix

- Build contradiction re-assessment into your process: after each major milestone, re-map.
- Watch for transformation signals: a contradiction that used to generate heat (debate, conflict, resource contention) going quiet may mean it's been resolved — or that people have given up. Investigate which.
- When the principal contradiction shifts, update the plan. Don't keep executing the old plan on momentum.

---

## Summary table

| # | Anti-pattern | Core error | One-line fix |
|---|---|---|---|
| 1 | Pseudo-synthesis | Picks a side, calls it synthesis | Steel-man opposition; synthesis must change structure, not description |
| 2 | Contradiction avoidance | Treats contradictions as factors | Name opposing forces as X vs Y |
| 3 | Template application | Copies previous analysis | Analyze this situation's specific contradiction network |
| 4 | Principal-secondary confusion | Solves the wrong contradiction | Test: does resolving this transform the others? |
| 5 | Nature misjudgment | Mismatches method to type | Judge nature before choosing approach |
| 6 | Static analysis | Freezes the contradiction map | Re-map after every major action or shift |
