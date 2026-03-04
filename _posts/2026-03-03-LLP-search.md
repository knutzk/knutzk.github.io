---
layout: single
title: "Finding the Invisible: ATLAS Probes Long-Lived Particles with Displaced Muons"
excerpt: >
  The ATLAS Collaboration has released a substantial new search for long-lived particles using the first data from LHC Run 3, pushing our sensitivity to new physics further than ever before.
last_modified_at: 2026-03-03
header:
  overlay_image: "/assets/research/dvmu-event-display.jpg"
  caption: "Candidate event showing a displaced vertex (DV) and a displaced muon produced far from the interaction point (Image: ATLAS Collaboration/CERN)."
  teaser: "/assets/teasers/dvmu.jpg"
categories: [Physics]
tags: [ATLAS, SUSY, LLP, LHC, Run 3, BSM, long-lived particles]
---

In the high-energy environment of the Large Hadron Collider (LHC), most new particles under investigation are expected to decay almost instantaneously. They leave their signatures as *prompt* signals at the heart of the detector. However, many theories suggest that the next major discovery could be a "slow-burner" – particles that travel several millimeters, or even decimeters, before revealing themselves through their decay products.

These are **Long-Lived Particles (LLPs)**, and they are a central prediction of numerous theories that extend beyond the Standard Model. In a new result recently submitted to *Physics Letters B* – an effort I had the privilege of coordinating – the ATLAS Collaboration presents a comprehensive hunt for these elusive travelers, utilizing a dataset collected during the first three years of LHC Run 3 (2022–2024), amounting to 164 inverse femtobarns of data.

## The Challenge of Displaced Events

Searching for LLPs is analogous to looking for a ghost that only becomes visible after it has left the room. Most standard reconstruction algorithms are designed for particles originating from the primary proton–proton collision point. Particles that decay further out – leaving **displaced vertices (DVs)** or **displaced tracks** – are frequently filtered out by standard software as noise or misreconstructions.

To overcome this, we have implemented several technical innovations. In Run 3, ATLAS introduced a dedicated **displaced-muon trigger**. This specialized hardware and software combination allows us to identify muons that do not point back to the collision point with significantly higher efficiency. By requiring the coincidence of these displaced muons with a high-mass (*massive*) displaced vertex, we can suppress the background from traditional *prompt* physics and focus on the signals that truly stand out from the Standard Model expected rates.

## Why Long-Lived?

The stability (or lifetime) of a particle is typically determined by the strength of its interactions and the mass of the *mediators* – the messenger particles that carry forces between others. In the Standard Model (our current best theory of the subatomic world), the neutron is relatively long-lived because its decay is suppressed by the high mass of the *W* boson. In theories such as **Supersymmetry (SUSY)** – which proposes a *superpartner* for every known particle in nature – we encounter a similar phenomenon.

If a symmetry known as **R-parity** is slightly broken – a scenario referred to as **R-parity violation** – the *Lightest Supersymmetric Particle* is no longer stable. While this particle is often considered a dark matter candidate in *stable* theories, in models with broken symmetry it can decay into quarks and leptons. If this instability is rather subtle (that is, the coupling is weak), the particle will travel a measurable distance through the detector before finally revealing itself.

In our analysis, we probed some of these superpartners with R-parity violation couplings. The search was optimized for two primary SUSY scenarios:
1.  **Higgsinos:** The superpartners of the Higgs bosons. In our benchmark models, these can decay into muons and quarks via processes that break the fundamental rules that usually keep the number of leptons (like electrons) or baryons (like protons) balanced in the universe.
2.  **Top Squarks (Stops):** The superpartners of the top quark. When these decay via R-parity-violating couplings, they produce a distinctive signature: a *b*-quark jet and a muon, both originating from a common vertex located far from the initial collision point.

![Feynman diagrams of the R-parity-violating decay modes.](/assets/research/dvmu-feynman-diagrams.jpg)
*Figure 1: Benchmark signal models for long-lived SUSY particles, showing the characteristic displaced vertex and displaced muon signature. (Image: ATLAS Collaboration/CERN)*

## The Art of Reconstruction

Reconstructing these "displaced" events is an immense feat of engineering. The ATLAS detector is constructed like a giant onion, with concentric layers of sensors. When a particle decays *inside* these layers – rather than at the geometric center – it creates a complex hit pattern that requires specialized logic to interpret.

We employ two distinct tracking passes. The first pass captures the standard, "prompt" particles. Any detector hits not used in the initial pass are then analyzed by a second, more computationally intensive pass. This *large-impact-parameter* pass is designed specifically for tracks with a large **transverse impact parameter** – essentially a *miss distance* that quantifies how far a track deviates from the center of the collision. These tracks are then algorithmically grouped to form a **Displaced Vertex (DV)**.

To ensure the signal is robust, a vertex must meet stringent criteria: it must have at least four associated tracks and a high **invariant mass**. We categorize these vertices into two regions based on their distance from the collision point: *near* DVs, which occur between 1–4 mm from the center and require a mass of at least 40 GeV, and *far* DVs, which occur more than 4 mm out and require a mass of at least 20 GeV. These mass thresholds are powerful discriminators, as random track crossings or hadronic interactions with detector material typically result in much lower masses.

## Cleanliness through Data-Driven Methods

One of the most significant hurdles in any exotic search is the "background" – the billions of Standard Model events that can mimic the signal. For LLPs, the backgrounds are particularly diverse:
*   **Heavy-flavor decays:** Quarks such as "bottom" and "charm" have finite lifetimes and can naturally produce displaced muons.
*   **Cosmic rays:** High-energy muons from space that happen to traverse the detector during a collision.
*   **Algorithmic fakes:** Random combinations of hits that the reconstruction software mistakenly identifies as a coherent track or vertex.

To address this, we developed a **fully data-driven background estimate**. Rather than relying on potentially imprecise simulations of these rare events, we measure the background rates directly in the data. By defining *validation regions* where we relax certain selection requirements, we can accurately measure the rates of individual background sources. We then extrapolate these into our signal region using the **transfer factor method**.

This method relies on the statistical independence of our selection variables. For instance, the probability of an event having a "fake" vertex is largely uncorrelated with whether it also contains a "fake" muon. By carefully measuring these independent probabilities, we can construct a robust prediction of the *background*, ensuring that any observed excess would be statistically significant.

![Schematic of the Transfer Factor implementation.](/assets/research/dvmu-tf-method.jpg)
*Figure 2: Schematic of the background estimation strategy. By measuring the rates in validation regions, we can predict the expected yield in the signal region using the transfer factor approach. (Image: ATLAS Collaboration/CERN)*

## Innovation in Run 3

The foundation of this search is the 164 fb⁻¹ of data collected at a center-of-mass energy of 13.6 TeV between 2022 and 2024. This represents not just a larger sample, but a higher-quality one due to Run 3 upgrades.

The new **displaced-muon trigger** allowed us to lower the **transverse momentum** thresholds for muons to just 20 GeV. In previous operational years, we often had to rely on much higher energy thresholds or additional signatures like large missing transverse momentum. This improvement has significantly expanded our sensitivity to lower-mass LLPs, which may have decay products with lower energy but are equally critical for a complete understanding of new physics that goes beyond our current theories.

## Reading the Results

Upon analysis of the initial Run 3 dataset, the observed data were found to be remarkably consistent with the Standard Model background predictions. We observed only three events in our "far" signal region and one in our "near" signal region – results that align well with our expectations from instrumental fakes and rare background processes.

While these results do not constitute a discovery, they allow us to set the most stringent limits to date on these specific R-parity-violating models.

![Exclusion contours for Top Squark decays.](/assets/research/dvmu-contour.jpg)
*Figure 3: The 95% confidence level exclusion limits for long-lived Top Squarks. The new results significantly extend our reach in both mass (up to 1.85 TeV) and lifetime compared to previous searches. (Image: ATLAS Collaboration/CERN)*

The primary highlights of the exclusion limits include:
- **Higgsinos:** We have excluded Higgsino masses up to **1.6 TeV** for proper lifetimes near 0.1 nanoseconds. For these specific models, this is an improvement in sensitivity of nearly **two orders of magnitude** compared to results from LHC Run 1.
- **Top Squarks:** The exclusion limit was pushed to **1.85 TeV** for intermediate lifetimes, representing a significant step forward in our hunt for supersymmetric partners.

## A Stepping Stone for the Future

This result stands as one of the first major "Exotics" publications from the Run 3 era. It demonstrates the efficacy of the ATLAS detector upgrades and the sophisticated new trigger and reconstruction strategies developed by our teams.

By targeting the *displaced* and the *invisible*, we are systematically closing the gaps in our search for the fundamental laws of nature. Having coordinated this analysis and drafted the resulting publication, it was rewarding to see how our results fully exploit the improved technical capabilities of the ATLAS detector in Run 3. As the LHC continues to provide high-quality collision data, we will continue to refine these techniques. The remaining years of Run 3 will allow us to probe even deeper into the mass–lifetime plane, bringing us closer to discovering the particles that have, until now, remained hidden from view.

---

**Publication Details:**

**Author:** ATLAS Collaboration<br>
**Title:** *Search for massive, long-lived particles in events with displaced vertices and displaced muons in pp collisions at an energy of 13.6 TeV with the ATLAS experiment*<br>
**Reference:** Submitted to *Phys. Lett. B*. [[arXiv:2603.03100](https://arxiv.org/abs/2603.03100)].
