---
title: "From Cow Pancreases to Designer Peptides: How We Learned to Engineer Weight Loss"
date: 2025-12-05
draft: false
author: "Alondra Escobar"
tags: ["GLP-1", "drug development", "peptide engineering", "obesity"]
image: /images/notes/post.jpg
description: "How decades of failures — and a detour through lizard venom — led to the most effective weight loss drugs ever developed."
---

For most of the twentieth century, the drugs we reached for to treat obesity worked the way a sledgehammer works: broadly, imprecisely, and often destructively. It took decades of failures — and a detour through lizard venom — to understand that the body already had a system for regulating weight, and that the real engineering challenge was learning to speak its language.

---

## The Blunt Instruments Era

The first assumption underlying early weight loss drugs was simple: if a patient eats less, they lose weight, so suppress appetite by any means necessary. In the 1950s and 60s, amphetamines were widely prescribed for exactly this purpose. They worked, in the narrow sense — appetite dropped, weight followed. But amphetamines act on the central nervous system indiscriminately, hijacking dopamine and norepinephrine pathways in ways that drove dependency, cardiovascular stress, and abuse. The mechanism was never specific to appetite; it just happened to suppress it alongside everything else.

The 1990s produced a more targeted-seeming attempt: fenfluramine-phentermine, better known as fen-phen. The logic here was serotonin and norepinephrine modulation — neurotransmitter systems more plausibly linked to satiety. Fen-phen worked well enough that it became widely prescribed before long-term safety data existed. It was withdrawn from the market in 1997 after patients developed fatal cardiac valvulopathy. The assumption — that you could manipulate neurotransmitter tone for appetite without systemic consequences — was wrong.

Orlistat, approved in 1998, abandoned the brain entirely and targeted the gut mechanically, inhibiting pancreatic lipase to block dietary fat absorption. It was technically effective and, unlike its predecessors, not dangerous. But blocking fat absorption indiscriminately produces predictable GI consequences, and real-world compliance was poor. It is still on the market. It is not widely used.

The through-line across these three decades: each drug was built on an assumption about where weight regulation happened — the brain's reward system, its satiety circuits, the digestive tract — and each assumption turned out to be too narrow, or wrong in ways that became apparent only after widespread use. None of these drugs engaged the body's own metabolic feedback machinery.

---

## Insulin and the Bioengineering Template

To understand how we eventually got to drugs that do engage that machinery, you have to go back to insulin — and to Eli Lilly.

When Frederick Banting and Charles Best isolated insulin in 1921, the immediate problem was scale. Diabetic patients needed a reliable supply, and the only source was animal pancreases — primarily bovine and porcine. Eli Lilly moved quickly to industrialize extraction, and by the mid-1920s was producing insulin at commercial scale. But animal-derived insulin was impure by modern standards, mildly immunogenic (bovine insulin differs from human insulin at three amino acid positions), and inconsistent batch to batch. It kept people alive. It was not a precise therapeutic.

The pivot came in 1982, when Lilly and Genentech brought recombinant human insulin to market under the name Humulin — the first bioengineered therapeutic protein approved for human use. The production method: insert the human insulin gene into *E. coli*, let bacteria do the manufacturing. The product was chemically identical to endogenous human insulin. The immunogenicity problem dissolved. The consistency problem dissolved.

More importantly, it established a template. Pharmaceutical companies now knew they could engineer peptide therapeutics at scale using recombinant biology — and that they could modify the sequence itself to change pharmacological properties. The question that followed, almost immediately, was what else could be engineered this way.

---

## The Discovery of GLP-1: A Collaboration Across Disciplines

The search for incretins — gut hormones that stimulate insulin secretion in response to food — had been underway since 1906, when researchers in Liverpool showed that intestinal extracts could lower blood glucose. Interest faded with the discovery of insulin, revived in the 1960s when three independent groups observed that oral glucose raised insulin more than intravenous glucose did, implying a gut-derived signal. GIP (glucose-dependent insulinotropic polypeptide) was identified first but failed to show efficacy in diabetic patients. The search continued.

The breakthrough came from an unlikely methodological choice. Joel Habener, an endocrinologist and molecular biologist at Massachusetts General Hospital, wanted to study how the glucagon precursor protein was processed — but instead of using mammalian tissue, he turned to fish. In fish, unlike mammals, the insulin-producing islets of Langerhans reside in a separate organ called Brockman bodies, providing an anatomically isolated and enriched source of glucagon-producing cells. Working from cDNAs derived from Brockman bodies, Habener's group reported in 1982 that glucagon is a cleavage product of a 124-amino acid precursor that also encodes a previously unknown 34-amino acid peptide — which they named glucagon-related peptide and noted bore homology to both glucagon and GIP.

The mammalian sequence followed the next year, when Graeme Bell and colleagues cloned the hamster glucagon precursor and found the glucagon-related peptide was 37 amino acids in the mammalian form, with a 6-amino acid N-terminal extension absent in fish. This peptide — renamed Glucagon-Like Peptide 1, or GLP-1 — was structurally suggestive of function, but initial biological testing of the full-length GLP-1(1-37) showed no effect on insulin secretion. Its function remained unclear.

The identification of the biologically active form required a different kind of expertise. Svetlana Mojsov had trained in the laboratory of Nobel laureate Bruce Merrifield at Rockefeller University, where she developed novel peptide synthesis methods using solid-phase chemistry to synthesize glucagon and its variants — methods still in use today. When she arrived at MGH in 1983, the Bell et al. hamster sequence had just appeared, and she quickly began collaborating with Habener. Mojsov noticed a conserved histidine at position 7 of GLP-1(1-37), preceded by an arginine residue — a pattern suggesting a proteolytic cleavage site. In a notebook entry, she marked this as a potential site that would liberate a shorter, potentially active form.

To test this, she fractionated extracts from pancreas, small intestine, and large intestine using gel filtration followed by ion exchange chromatography, assaying each fraction with seven different radioimmunoassays built from peptides she had synthesized herself. The results confirmed it: GLP-1(7-37) was present in large amounts in intestinal tissue, while only larger precursor forms of glucagon were found there. The landmark 1986 paper, published under the understated title "Preproglucagon Gene Expression in Pancreas and Intestine at the Level of Posttranslational Processing," contained the key finding: GLP-1(1-37) is a prohormone, and GLP-1(7-37) is its active cleavage product.

In early 1987, Mojsov, Weir, and Habener demonstrated that GLP-1(7-37) potently stimulated insulin secretion six-fold in isolated rat pancreas at physiological concentrations — and critically, only in the presence of elevated glucose. Full-length GLP-1(1-37) had no effect at any concentration. That same year, the Bloom group showed that infusion of GLP-1(7-36) amide increased plasma insulin and reduced blood glucose in humans after a glucose load but not during fasting — the glucose-dependence that defines incretin activity. GLP-1(7-37) had satisfied all the criteria. The molecule problem was real; now the engineering had to begin.

## Nature's Proof of Concept: The Gila Monster

The half-life of native GLP-1(7-37) in circulation is 1 to 2 minutes. It is cleaved almost immediately by the enzyme DPP-4, which recognizes the alanine at position 8 following the N-terminal histidine. A hormone that disappears within minutes requires continuous intravenous infusion to maintain therapeutic levels — not a viable drug format. The engineering challenge was to make a version that lasted.

An unexpected piece of evidence that this was solvable came from the Gila monster (*Heloderma suspectum*). John Eng, working at the VA Medical Center in New York in the mid-1980s, was systematically screening bioactive peptides from Gila monster venom for molecules with an N-terminal histidine — a structural feature he had noticed was shared by GLP-1 and several other gut peptides. He identified exendin-4, a 39-amino acid peptide with extensive sequence homology to GLP-1(7-37) that bound the GLP-1 receptor with high affinity and stimulated insulin secretion in rodents. Crucially, exendin-4 carries a mutation that blocks DPP-4 cleavage, extending its half-life to 2.4 hours. The Gila monster had independently evolved a GLP-1-like peptide stable enough to function as a circulating signal — demonstrating that DPP-4 resistance was biochemically achievable without loss of receptor activity.

Eng's collaboration with Amylin Pharmaceuticals brought exenatide (Byetta) to approval in 2004 as the first GLP-1 receptor agonist for type 2 diabetes. It worked, but twice-daily injection and modest efficacy set a clear ceiling. Exenatide was proof of concept, not the destination.

---

## Engineering the Molecule

With exendin-4 establishing DPP-4 resistance as achievable, the central engineering problem shifted to half-life extension through a different mechanism — one that could be applied to the human GLP-1 sequence itself rather than relying on the Gila monster scaffold. This work was led at Novo Nordisk by Lotte Knudsen, who had joined the company's newly formed innovation team in the early 1990s and, notably, believed from the outset that a stable GLP-1 analog would treat obesity — not just diabetes. That was not the consensus view at the time.

The approach Knudsen's team adopted was fatty acid conjugation, a strategy first developed by Novo chemists for insulin analogs: attach a fatty acid to a lysine residue via a linker, enabling the peptide to reversibly bind serum albumin. Albumin-bound drug is too large for renal filtration and is shielded from proteolytic degradation, dramatically extending circulation time. The challenge was finding the right fatty acid, the right linker, and the right attachment site without destroying receptor activity.

**Liraglutide** (Victoza, approved 2010) was the result of extensive mutagenesis and screening across combinations of fatty acids, linkers, and coupling sites. The final molecule attaches a C-16 fatty acid via a glutamic acid linker to lysine at position 26. To ensure specificity — only one attachment site — lysine 34 was mutated to arginine, leaving K26 as the only available coupling point. The result: half-life extended to approximately 13 hours, enabling once-daily injection. Clinically, liraglutide reduced HbA1c by 1.1–1.6% in diabetic patients with significant weight loss in the majority of patients. An important practical insight during development: the nausea that appeared at full dose could be mitigated by starting low and escalating gradually — a dose-titration protocol now standard across this drug class.

**Semaglutide** (Ozempic, 2017; Wegovy, 2021) was built by Knudsen's team with Jesper Lau and Thomas Kruse, testing thousands of linker-fatty acid-sequence combinations with the goal of once-weekly dosing. Three modifications distinguish it from liraglutide. First, the same K26 attachment site is retained, but the fatty acid is a C-18 diacid connected via a longer, hydrophilic linker — this increases albumin binding affinity substantially, reducing the fraction of unbound, degradable drug at any given time. Second, alanine at position 8 is replaced with alpha-aminoisobutyric acid (Aib), a non-natural amino acid that directly blocks DPP-4 cleavage at that site — a modification absent in liraglutide and responsible for much of semaglutide's additional stability. Third, as with liraglutide, lysine 34 is mutated to arginine to enforce single-site fatty acid attachment. Together these modifications extend half-life to approximately 7 days.

The clinical signal was striking. In the STEP-1 trial, semaglutide at 2.4 mg produced mean weight loss of ~15% body weight over 68 weeks — roughly double liraglutide's effect size, which tracks directly to greater time-averaged receptor occupancy from the improved pharmacokinetics. The progression from exenatide to liraglutide to semaglutide is not incremental in the colloquial sense. Each generation was built on a mechanistic diagnosis of why the previous molecule was still failing pharmacokinetically — and each structural solution can be mapped to a specific improvement in the clinical data.

---

## Where This Leaves Us

The arc from bovine insulin to semaglutide is a story about precision. The blunt instruments of the mid-twentieth century failed because metabolic regulation is not a single lever — it is a coordinated system involving the gut, the pancreas, the brain, and circulating peptides that talk between them. Drugs that pulled one lever without understanding the system produced side effects, cardiovascular damage, or compliance failures.

GLP-1 analogs work because the right receptor system was found — through a combination of molecular biology, peptide chemistry, and the unexpected evidence from a lizard's venom — and then the engineering problems standing between a biological signal and a viable drug were solved one by one. What makes the progression from Habener's fish islets to Mojsov's cleavage site to Knudsen's fatty acid conjugation strategy legible in retrospect is that each step addressed a specific, identifiable limitation of the previous one. That is what rational drug development looks like when it works.

The molecule problem, for now, appears largely solved. The fight that has emerged since — between Eli Lilly and Novo Nordisk, between injectables and pills, between insurance coverage and access — is a different kind of problem. That's the subject of the next post.
