---
title: "The Acoustic GFP: How Gas Vesicles Are Giving Ultrasound a Reporter Gene"
date: 2026-02-20
draft: false
author: "Alondra Escobar"
tags: ["acoustic reporter genes", "gas vesicles", "ultrasound imaging", "synthetic biology", "neuroscience"]
description: "GFP transformed biology by letting researchers watch living cells in real time. Acoustic reporter genes are attempting the same for ultrasound, and the brain."
---
# The Acoustic GFP: How Gas Vesicles Are Giving Ultrasound a Reporter Gene

Before 1994, if you wanted to study gene expression in a specific cell type, you first had to kill it. Standard methods (antibody staining, in situ hybridization, beta-galactosidase assays) all required fixing and permeabilizing the tissue. You could only look at dead cells, producing a static snapshot. If you wanted to understand how gene expression changed over time during development, you had to compare snapshots from dozens of different animals and infer a timeline you could never directly observe. Then in 1994, Martin Chalfie showed that you could tag living cells in an intact *C. elegans* worm with a fluorescent protein from a jellyfish (green fluorescent protein, GFP) and watch them under a microscope in real time, no fixation, no killing, no inference. The animal was alive. The cells were lit up. The response from the research community was immediate: within a year, 1,500 labs had requested the GFP vectors. Within 15 years, GFP had generated over 30,000 publications and had been expressed in every major research organism on earth. In 2008, the Nobel Prize in Chemistry went to the three scientists behind it. Today, fluorescent reporters are so embedded in biological research that it is nearly impossible to publish a cell biology paper without one.

Thirty years later, the frontier has moved to the brain, and fluorescent proteins have hit a wall. Light scatters aggressively in biological tissue, limiting useful optical imaging to roughly 1 to 2 mm of depth. The mammalian skull makes it worse. Studying the living brain non-invasively with optical tools requires cranial windows, fiber optics, or implanted lenses, all surgical. fMRI offers a non-invasive alternative but measures blood flow as a proxy for neural activity, has millimeter-scale resolution, and has no cell-type specificity whatsoever: you can see that a region is active, not which neurons within it are doing what. What neuroscience is missing is something analogous to what GFP provided for cell biology: a genetically encodable reporter that connects a specific cellular identity or genetic program to a detectable signal, but one that works at depth, through tissue, without surgery. Acoustic reporter genes are the first serious attempt to build that tool.

---

## Why Ultrasound and Why Now

Ultrasound penetrates centimeters of tissue with sub-millimeter spatial resolution, is real-time, requires no ionizing radiation, and is the most widely deployed imaging modality in clinical medicine. It has been used in biomedicine for decades. What it has always lacked is a genetically encodable contrast agent, a molecular reporter that connects ultrasound signal to what a specific cell is actually doing.

Existing ultrasound contrast agents are microbubbles: gas-filled spheres roughly 1 to 10 micrometers in diameter, injected into the bloodstream, detectable because gas scatters sound waves strongly due to the acoustic impedance mismatch between gas and tissue. Microbubbles work for vascular imaging. They cannot be genetically encoded, they cannot be linked to gene expression, and they are too large to enter cells. They are the acoustic equivalent of an injected dye, useful but disconnected from cell biology.

The key insight behind acoustic reporter genes is that microorganisms already make their own gas-filled structures, encoded entirely in their genomes.

---

## The Physical Substrate: Gas Vesicles

Gas vesicles (GVs) are protein-shelled, gas-filled nanostructures produced naturally by buoyant photosynthetic bacteria and archaea (including *Anabaena flos-aquae* and *Halobacterium salinarum*) as buoyancy regulation devices. They are 45 to 250 nm wide and 100 to 600 nm long, roughly 10 to 100 times smaller than a microbubble. Their protein shell is permeable to dissolved gas but excludes water, which means no pressure differential exists across the shell. Unlike a soap bubble, there is no internal force trying to collapse them, which makes them inherently stable at nanoscale despite being gas-filled.

They scatter ultrasound for the same reason microbubbles do: the acoustic impedance mismatch between their gas interior and surrounding tissue. But because they are genetically encoded, the genes that produce them can be transplanted into other organisms, placed under the control of any promoter of interest, and used to report on gene expression exactly as GFP does for fluorescence.

Two additional physical properties make GVs practically useful as imaging agents. First, above a species-specific pressure threshold (ranging from 40 to 700 kPa depending on GV type), GVs irreversibly collapse and lose their acoustic signal. Imaging before and after a collapse pulse and subtracting the two images produces a GV-specific contrast map with tissue background removed. Second, GVs without their outer scaffolding protein (GvpC) are mechanically flexible enough to produce nonlinear harmonic signals under ultrasound, signals that are distinguishable from the linear response of surrounding tissue. This nonlinear contrast enables continuous imaging without needing to collapse the GVs, which is essential for any experiment that requires watching the same cells over time.

---

## Building the Acoustic Reporter Gene: 2014 to 2023

**2014: The physical proof of concept**

Mikhail Shapiro and colleagues at Berkeley published the founding paper of the field in *Nature Nanotechnology*, demonstrating that purified GVs from *Anabaena* and *Halobacterium* produce stable, detectable ultrasound contrast in gel phantoms and in live mice after injection. Collapsed GVs produced no contrast, confirming the gas compartment was responsible for the signal. Surface-functionalized GVs that aggregated in response to a target molecule changed their acoustic signature, showing that GVs could act as biosensors. The GVs here were purified and injected, with no gene expression connection. This paper is the acoustic equivalent of Shimomura's 1962 isolation of GFP from jellyfish: the physical substrate is identified and shown to work. The reporter gene application comes next.

*2018: First acoustic reporter genes in bacteria, imaged in living mammals*

The Shapiro lab, now at Caltech, demonstrated the first true ARGs: genetic constructs that allow bacterial gene expression to be visualized in vivo using ultrasound. GV production is encoded by an operon of 8 to 14 genes, including the primary structural protein GvpA, optional scaffolding protein GvpC, and several accessory chaperone proteins. Transplanting this cluster into *E. coli* and *Salmonella typhimurium* required engineering a hybrid gene cluster that produced GVs large enough to scatter ultrasound detectably. The result: engineered bacteria detectable at volumetric densities below 0.01% with sub-100 micrometer resolution in living mice. Two acoustically distinct ARG variants with different GV collapse pressures enabled multiplexed imaging of two bacterial populations simultaneously in the same animal, the acoustic equivalent of two-color fluorescence. Proof-of-concept applications included tracking tumor-colonizing bacteria and gastrointestinal bacteria in live mice, non-invasively, without any surgery.

*2019: ARGs in mammalian cells*

Moving from bacteria to mammalian cells required solving a fundamentally different problem. Bacteria routinely transcribe multiple genes from a single polycistronic mRNA; mammalian ribosomes do not. A 9-gene bacterial GV cluster inserted into a mammalian cell produces proteins that the cell does not know how to assemble into structures. Arash Farhadi and colleagues in the Shapiro lab spent several years solving this: using viral regulatory elements (the same tricks retroviruses use to express polyprotein precursors) to produce multiple GV proteins from a shared RNA while maintaining the correct stoichiometry for assembly. The correct ratio of GvpA to accessory proteins had to be established empirically. When it worked, HEK293T cells expressing the mammalian ARG construct produced intracellular gas vesicles confirmed by electron microscopy and detectable by ultrasound in living mice at depths inaccessible to optical methods. The first-generation construct had significant limitations: weak signal requiring buoyancy enrichment steps, a large genetic footprint across two cassettes, and expression heterogeneity requiring single-cell clonal selection. Shapiro said at the time that they probably had 20 years of optimization ahead. The analogy to early GFP was intentional.

*2023: ARG 2.0, 38-fold improvement*

Rather than continuing to engineer the first-generation bacterial cluster, Hurt, Buss, Duan, and colleagues took a phylogenetic approach: screening GV gene clusters from dozens of diverse bacteria and archaea, reasoning that evolution had already explored the sequence space for GV properties. The winning candidate for mammalian cells was the *Anabaena flos-aquae* cluster, which produces large GVs with strong nonlinear acoustic contrast when expressed without GvpC. Two key optimizations drove the improvement: overexpression of GvpA relative to accessory proteins (reflecting the native expression pattern of the cluster) and stabilization of the GvpA transcript with a WPRE element. The result was a second-generation mammalian ARG producing 38-fold stronger nonlinear contrast than first-generation constructs, with a smaller genetic footprint, no clonal selection required, and stable long-term expression. Bacterial ARG 2.0 showed a 9-fold improvement over its first-generation counterpart. Both constructs are available on Addgene. This is the version the field will actually use.

---

## What ARGs Cannot Yet Do, and Why It Matters

ARGs as currently developed are reporters of gene expression, not neural activity. They tell you which cells are expressing a genetic program, not when those neurons are firing. The GFP analogy holds precisely: GFP reports gene expression, GCaMP (a GFP variant fused to a calcium-sensing domain) reports neural activity. ARGs are at the GFP stage. An acoustic GCaMP equivalent, a genetically encoded ultrasound contrast agent whose signal changes with intracellular calcium or membrane voltage, does not yet exist.

Three additional engineering challenges remain. GV gene clusters of 8 to 14 genes exceed the roughly 4.7 kb cargo limit of AAV vectors, the standard tool for in vivo gene delivery. This is a hard constraint for any therapeutic or in vivo neuroscience application requiring viral delivery, and compact cluster engineering is an active problem. Neuronal expression without cytotoxicity or functional disruption has not been demonstrated; neurons are more metabolically sensitive than HEK cells, and the metabolic cost of maintaining large protein assemblies is not trivial. And single-cell sensitivity in intact mammalian tissue remains challenging, though single bacterial cell detection has been demonstrated with specialized pulse sequences.

None of these are reasons to discount the technology. They are the engineering problems of a field that is roughly where GFP was in 1995: proof of concept demonstrated, first-generation limitations identified, optimization just beginning. The comparison to GFP is not hype. It is a realistic assessment of how long building a new reporter class actually takes, and a reasonable basis for thinking about what the next decade might produce.

---

## The Experiment That Does Not Yet Exist

GFP enabled an experiment that was previously impossible: watching a living cell express a gene in real time, without killing it. The experiment that ARGs are reaching toward is analogous: watching a living brain express a genetic program in real time, at depth, through the skull, without surgery.

That experiment does not exist yet. The tool that would enable it is being built, paper by paper, one generation of constructs at a time. The people who will build the next generation are likely reading papers like the ones described here, in labs that have just received the ARG 2.0 constructs from Addgene. That is where this field is. It is early enough that the contribution of a single lab, or a single person, could define what acoustic reporter genes become.
