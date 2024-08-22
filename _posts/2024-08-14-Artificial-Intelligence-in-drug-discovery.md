---
layout: post
title:  "(WIP) Paper - Artificial Intelligence in Drug Discovery:Applications and Techniques"
date:   2024-08-01 12:09:11 +0200
category: Paper-Reviews
---

# Notes
## Introduction
The paper focuses on small-molecule drugs, rather than biologics like antibodies or vaccines.

Pre-requisite for drug discovery is presence of a hypothesis for activation or inhibition of a target that results in therapeutic effects for the disease. High-throughput screening is used to rapidly identify compounds that 'hit-candidates', i.e. candidates for this specific interaction, by searching through large databases of SAR(structure-activity relationship) databases. This search technique is known as 'virtual screening'. VS can be conducted using computational approaches that focus on structure-based knowledge of the target or known active ligands of the target.

Binding specificity is important - molecules usually bind to more than one target, binding to unintended targets can lead to unexpected side-effects. Some important properties considered whilst developing a drug compound: Synthetic Accessibility Score (how easy or hard it is to synthesise a molecule), Quantitative estimation of drug likeliness (how likely the molecule is a viable candidate). Usually, a predictive model is built to predict these scores for a given molecule. A more intriguing prospect
from QSAR is that these models can be exploited inversely to reveal the structural features underlying the optimal properties to guide drug design from scratch.



# Definitions and Concepts
* `de-novo` drug design - from scratch, not based on existing drugs.

Key Concepts of De-Novo Drug Design:
- Target Identification: The process begins with identifying a biological target, usually a protein associated with a disease. Understanding the structure and function of this target is crucial.
- Structure-Based Design: Using the 3D structure of the biological target (often obtained through techniques like X-ray crystallography or NMR spectroscopy), scientists design molecules that can interact with the target in a specific manner.
- Computational Methods: Advanced algorithms and computational models are employed to predict how new molecules will interact with the target. Techniques like molecular docking, molecular dynamics, and virtual screening are commonly used.
- Scaffold Creation: A basic chemical scaffold (or core structure) is designed, onto which functional groups can be added to optimize interaction with the target.
- Optimization: Once potential drug candidates are identified, they undergo optimization to enhance properties like potency, selectivity, solubility, and stability.
- Iterative Process: De-novo drug design is often iterative, with multiple rounds of design, testing, and refinement to improve the drug candidates.

* `retrosynthesis` Building up a complex target molecule from simpler precursors.

Retrosynthesis is a method used in organic chemistry and drug discovery to plan the synthesis of complex molecules by breaking them down into simpler precursor molecules. This approach involves working backward from the target molecule to simpler starting materials, essentially "deconstructing" the molecule step by step. Retrosynthesis is a critical tool for designing synthetic routes to produce complex drugs and other organic compounds.

Key Concepts of Retrosynthesis:
- Target Molecule: The process begins with a defined target molecule, which is the complex structure that needs to be synthesized. In drug discovery, this could be a potential drug candidate.
- Disconnection: The target molecule is "disconnected" or broken down into simpler structures, called intermediates or precursors. This is done by identifying bonds that can be theoretically broken to yield simpler, more readily available molecules.
- Synthons: The simpler molecules derived from the disconnection process are called synthons. These are idealized fragments that represent the building blocks from which the target molecule can be constructed.
- Reagents and Reactions: Each synthon corresponds to a real chemical reagent or a set of reagents that can be used to create the bond that was "disconnected" in the retrosynthesis step.
- Iterative Process: Retrosynthesis is typically an iterative process. The simpler intermediates identified from the first round of disconnections may themselves be subjected to further retrosynthesis until they are reduced to simple, commercially available, or easily synthesized starting materials.
- Synthetic Pathway Design: Once a retrosynthetic analysis is complete, it provides a synthetic pathway or strategy to construct the target molecule from basic starting materials. Chemists then use this pathway to carry out the synthesis in the lab.

* Ligand definition: 

A ligand is a molecule that can bind to a specific site on a target molecule, typically a protein, forming a complex. Ligands are key players in various biological processes and are crucial in fields like biochemistry, pharmacology, and drug design.

Binding: Ligands interact with their target molecules through various types of bonds, including ionic bonds, hydrogen bonds, van der Waals forces, and sometimes covalent bonds. The binding site on the target molecule is usually a specific region, such as the active site of an enzyme or a receptor's binding pocket.

Agonists and Antagonists:

Agonists: Ligands that bind to a receptor and activate it, triggering a biological response. For example, adrenaline is an agonist that binds to adrenergic receptors to stimulate the "fight or flight" response.
Antagonists: Ligands that bind to a receptor but do not activate it, instead blocking the receptor's normal function. For instance, beta-blockers are antagonists that prevent adrenaline from binding to its receptor, reducing heart rate.

Role in Drug Design:
In drug design, the goal is often to create or identify ligands that can specifically bind to a target protein involved in a disease process. By doing so, the ligand can modulate the protein's activity, leading to therapeutic effects. This concept is fundamental in the development of many pharmaceutical drugs.