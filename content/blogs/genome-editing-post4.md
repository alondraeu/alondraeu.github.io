---
title: "Rewriting the Code: A Decade of Genome Editing and Where It's Heading"
date: 2026-01-06
draft: false
author: "Alondra Escobar"
tags: ["CRISPR", "genome editing", "base editing", "prime editing", "RNA editing", "gene therapy"]
description: "From zinc finger nucleases to CRISPR to base editing to RNA editing: the seventy-four year search for a scalpel precise enough to fix a single letter in the genome."
---
# Rewriting the Code: A Decade of Genome Editing and Where It's Heading

In 1949, Linus Pauling published a paper showing that sickle cell disease was caused by a single abnormal protein in red blood cells. He called it a "molecular disease," the first time a human illness had been traced to a precise biochemical defect. The cause was understood at the molecular level seventy-four years before a cure existed. In December 2023, the FDA approved Casgevy, the first CRISPR-based medicine in humans, for sickle cell disease and beta-thalassemia. The gap between understanding and fixing was not a knowledge problem. It was a tool problem. The body of knowledge about sickle cell accumulated for decades while medicine waited for an instrument precise enough to operate on a single letter in a three-billion-letter text, inside a living cell, without cutting anything else. That instrument took most of a century to build, and the search is not over.

---

## Before CRISPR: Proof That Editing Was Possible

The idea of rewriting a specific DNA sequence in a living cell was considered speculative until the late 1990s, when zinc finger nucleases (ZFNs) demonstrated it was not. ZFNs are engineered proteins that combine a programmable DNA-binding domain with a FokI nuclease that cuts wherever the binding domain lands. By designing the zinc finger array to recognize a specific sequence, researchers could direct a cut to a chosen genomic address. It worked. Targeted edits were made in human cells. The concept was proven.

The limitation was the protein itself. Engineering a zinc finger array to recognize a new DNA sequence required custom protein design for every new target, a process that took months, required specialized expertise, and failed often enough to be impractical at scale. TALENs (transcription activator-like effector nucleases), introduced around 2010, used a more modular DNA-binding architecture that was somewhat easier to engineer, but the bottleneck remained: every new genomic target required designing and building a new protein. The tool worked in principle but was inaccessible to most labs.

Both approaches shared the same underlying logic: a protein-encoded DNA address attached to a universal cutting enzyme. That logic was correct. The problem was that proteins are slow and expensive to reprogram.

---

## CRISPR-Cas9: The Address Became a Molecule of RNA

In 2012, Jennifer Doudna and Emmanuelle Charpentier published the biochemistry of Cas9, a bacterial immune system protein that cuts DNA at a sequence specified not by a custom protein but by a short RNA guide. Changing the genomic target meant synthesizing a new 20-nucleotide RNA sequence, a process that costs roughly ten dollars and takes two days. The same addressability problem that required months of protein engineering with ZFNs and TALENs had collapsed to a routine molecular biology step.

In 2013, Feng Zhang at the Broad Institute and George Church at Harvard independently demonstrated CRISPR-Cas9 editing in mammalian cells. Within months, labs across the world were using it. The patent dispute that followed between the Broad and the University of California (representing Doudna's work) became one of the largest intellectual property battles in the history of biotechnology, still contested internationally. The science, however, moved fast regardless of the legal outcome.

CRISPR-Cas9 works by making a double-strand break (DSB) at the target site. The cell then repairs the break through one of two competing pathways: NHEJ (non-homologous end joining), which is fast and error-prone and typically introduces small insertions or deletions that disrupt gene function, or HDR (homology-directed repair), which is precise but requires a repair template and is inefficient in most cell types. For applications where you want to disrupt a gene, NHEJ is sufficient. For applications where you want to install a specific correction, HDR's inefficiency is a real constraint. And for therapeutic applications at scale, the double-strand break itself carries risk: off-target cuts, chromosomal rearrangements, and activation of DNA damage response pathways.

Casgevy, the 2023 approval, uses CRISPR-Cas9 to reactivate fetal hemoglobin production in patient-derived cells ex vivo, sidestepping the need for precise in-sequence correction. It is an elegant workaround. It is also a sign that the tool, as powerful as it is, still has edges sharp enough to require careful handling.

---

## Base Editing and Prime Editing: Getting the Scalpel Sharper

The limitations of Cas9 motivated David Liu's lab at the Broad Institute to ask a different question: what if you could change a specific base without cutting both strands at all?

Base editing, introduced in 2016, answers that question by fusing a catalytically impaired Cas9 (one that nicks rather than fully cuts, or binds without cutting) to a base deaminase enzyme. The Cas9 finds the target sequence and holds the DNA open; the deaminase chemically converts one base to another within a small editing window. Cytosine base editors convert C to T. Adenine base editors convert A to G. No double-strand break is made. No repair template is required. Editing efficiencies in many cell types reach 50% or higher, and the absence of a DSB substantially reduces the off-target cutting risk that accompanies Cas9. Base editing covers approximately 30% of the point mutations known to cause human disease.

Prime editing, introduced in 2019 from the same lab, extends the range further. A nickase Cas9 is fused to an engineered reverse transcriptase, and the guide RNA is redesigned to carry not just a genomic address but the desired edit sequence. The reverse transcriptase writes the new sequence directly into the target site. Prime editing can make all twelve possible point mutations, small insertions, and small deletions, all without a double-strand break and without a separate repair template. The tradeoff is efficiency: prime editing is currently less efficient than base editing in many contexts, and delivery of the larger construct presents practical challenges. Both are active areas of optimization.

The progression from Cas9 to base editing to prime editing is not a story of replacement but of expanding precision. Each approach has contexts where it is the right tool. Cas9 disruption remains the fastest route to gene knockouts. Base editing is the most efficient option for correctable point mutations within its scope. Prime editing handles the cases base editing cannot. Together they represent a toolkit rather than a single instrument.

---

## RNA Editing: Making the Edit Reversible

All of the above edits DNA, which means they are permanent. For many diseases, permanent correction is exactly what is needed. For others, it is not. Gain-of-function mutations, acute conditions, or applications requiring dose adjustability are better served by an edit that disappears when no longer needed. This is the logic behind RNA editing.

The human body already edits RNA. ADAR (adenosine deaminase acting on RNA) is an endogenous enzyme that converts adenosine to inosine (read as guanosine) in double-stranded RNA regions, effectively making A-to-G changes at the transcript level. The edit exists only in the RNA; the DNA is untouched. When the RNA degrades, the edit is gone. The therapeutic goal is to redirect endogenous ADAR to a disease-relevant target using a guide RNA that creates the double-stranded structure the enzyme requires. No exogenous editing protein needs to be delivered, only the guide RNA itself, a substantially smaller and simpler payload.

Several companies (Wave Life Sciences, Korro Bio, Shape Therapeutics) are building on this approach. Current limitations are real: only A-to-G edits are efficient with endogenous ADAR, the editing window has imprecision, and off-target RNA editing across the transcriptome requires careful characterization. But the conceptual appeal is strong enough that the field is moving quickly. A therapy that can be re-administered, titrated, and stopped is a fundamentally different product than a permanent genomic edit, and for certain disease classes it may be the better answer.

---

## Where the Arc Ends, for Now

ZFNs proved that targeted editing was possible. TALENs made it somewhat easier. CRISPR made it accessible. Base and prime editing made it precise. RNA editing is making it reversible. Each transition was driven by the same underlying pressure: reducing the collateral damage of the editing event while preserving targeting flexibility. The tools have gotten progressively less blunt.

The clinical proof-of-concept era is over. Casgevy's approval in 2023 means genome editing is no longer a research curiosity. The open questions now are about delivery (how to get the tool into the right cells in a living body efficiently and safely), durability (how long edits persist and whether they need to be renewed), and access (who can afford a therapy that currently costs over two million dollars per patient). Those are hard problems, but they are different in character from the tool problems that dominated the previous thirty years. The scalpel exists. The surgery is beginning.