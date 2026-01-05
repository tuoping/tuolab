---
title: "Ping Tuo - Research"
layout: textlay
excerpt: "Ping Tuo -- Research"
sitemap: false
permalink: /research/
---

# Research

## Overview

High-throughput computational approaches aim to transform materials discovery by enabling rapid prediction of novel inorganic compounds. In 2023, 84,641 distinct compounds has been predicted to be thermodynamically stable, of which 24,541 were reported in the ICSD as experimentally realized.
The gap between predicted and synthesized materials can be attributed to four primary failure modes[^Szymanski2023]: slow reaction kinetics, precursor volatility, product amorphization, and intrinsic limitations of density functional theory calculations performed at 0 K.

<div style="text-align: center">
<img style="width: 80%;" src="{{ site.url }}{{ site.baseurl }}/images/Overview_freeenergy.png" alt="Chemical discovery overview"/>
</div>

However, all of this information is encoded in the free energy landscape $F(x)$, which has traditionally been prohibitively expensive to compute and therefore inaccessible to high-throughput studies. Generative models establish a machine-learned probability field mapping, which is related to the free energy landscape by $P(x)\propto e^{-F(x)/k_BT}$, offering a promising route towards scalable, high-throughput free energy calculations.

<div style="text-align: center">
<img style="width: 50%;" src="{{ site.url }}{{ site.baseurl }}/images/Overview_gen.png" alt="Generative modeling overview"/>
</div>

My research builds physics-aware generative frameworks for free energy calculations and free energy-driven kinetics simulation, addressing a central gap in today’s AI-driven materials discovery: The lack of thermodynamic and kinetic realism in generative structure models.

[^Szymanski2023]: Szymanski N J, Rendy B, Fei Y, et al. An autonomous laboratory for the accelerated synthesis of novel materials[J]. Nature, 2023, 624(7990): 86-91.

## Current research directions

<div class="two-col">
  <div class="col-left">
<img src="{{ site.url }}{{ site.baseurl }}/images/tocpic/algo_schematic.png"  style="width: 100%" />
  </div>

  <div class="col-right">

### Conditional flow matching framework MolGEN

[MolGEN](https://github.com/tuoping/MolGEN) is a conditional generative modeling package that couples the state-of-the-art flow matching frameworks with equivariant transformers. The framework can be easily adapted to evaluate the free energy surfaces, metastability, and generate kinetic pathways.

[1] Tuo P, Chen J, Li J. Flow matching for reaction pathway generation[J]. arXiv preprint arXiv:2507.10530, 2025. https://arxiv.org/abs/2507.10530

  </div>
</div>


<div class="two-col">
  <div class="col-left">
<img src="{{ site.url }}{{ site.baseurl }}/images/tocpic/TOC.png"  style="width: 100%" />
  </div>

  <div class="col-right">

### Free energy sampling in the alchemical space

Free energy sampling in the alchemical space is increasingly important with the emergence of high entropy materials. Yet it faces unique challenge due to the discrete nature of the alchemical space. [alchemicalFES](https://github.com/tuoping/alchemicalFES) implements free energy sampling of the alchemical space based on flow matching of the Dirichlet distribution and achieves multi-temperature generation with a light-weight CNN model by reformulating the guidance technique. 

[1] Tuo P, Zeng Z, Chen J, et al. Scalable Multitemperature Free Energy Sampling of Classical Ising Spin States[J]. Journal of Chemical Theory and Computation, 2025, 21(22): 11427-11435. https://pubs.acs.org/doi/full/10.1021/acs.jctc.5c01248

  </div>
</div>



<div class="two-col">
  <div class="col-left">
<img src="{{ site.url }}{{ site.baseurl }}/images/tocpic/Nanodomain_perov.jpg"  style="width: 100%" />
  </div>

  <div class="col-right">

### Collective Ordering Phase Behavior

Collective ordering refers to macroscopic order emerging under frustration, mediated by long-range interactions, on a flattened free-energy landscape. Collective ordering is characterized by:

- Strong correlations across length scales

- Competing interactions (elastic, electrostatic, magnetic, entropic)

- Multiple nearly degenerate states

- History dependence and hysteresis

- Mesoscopic heterogeneity rather than uniform order

Example phenomena include martensitic transformations, ferroic transitions, charge/spin density waves, and nanodomain ordering. 

[1] Tuo P, Li L, Wang X, et al. Spontaneous Hybrid Nano‐Domain Behavior of the Organic–Inorganic Hybrid Perovskites[J]. Advanced Functional Materials, 2023, 33(32): 2301663. https://advanced.onlinelibrary.wiley.com/doi/abs/10.1002/adfm.202301663

[2] Liu Y, Tuo P, Dai F Z, et al. A Highly Deficient Medium‐Entropy Perovskite Ceramic for Electromagnetic Interference Shielding under Harsh Environment[J]. Advanced Materials, 2024, 36(28): 2400059. https://advanced.onlinelibrary.wiley.com/doi/abs/10.1002/adma.202400059

  </div>
</div>


<div class="two-col">
  <div class="col-left">
<img src="{{ site.url }}{{ site.baseurl }}/images/tocpic/chemicalspace_MgSiAs.png"  style="width: 100%" />
  </div>

  <div class="col-right">

### Functional Ceramics Design for Tailored Electronic, Magnetic, and Photoelectronic Properties


[1] Tuo P, Pan B C. Dilute magnetism in Co-doped spinel Mg3Si6As8[J]. Journal of Applied Physics, 2020, 128(3).

[2] Ye X B, Tuo P, Pan B C. Flatband in a three-dimensional tungsten nitride compound[J]. The Journal of Chemical Physics, 2020, 152(22).

[3] Tuo P, Ye X B, Pan B C. A machine learning based deep potential for seeking the low-lying candidates of Al clusters[J]. The Journal of Chemical Physics, 2020, 152(11).

[4] Tuo P, Pan B C. New compounds Mg3IV6V8 (IV= Si, Ge, Sn; V= P, As, Sb) and their potential application to photovoltaic materials[J]. Journal of Alloys and Compounds, 2019, 786: 434-439.

[5] Tuo P, Pan B C. First-principles study of intrinsic point defects in MgSiAs2[J]. Physical Chemistry Chemical Physics, 2019, 21(9): 5295-5304.

[6] Li S, Tuo P, Xie J, et al. Ultrathin MXene nanosheets with rich fluorine termination groups realizing efficient electrocatalytic hydrogen evolution[J]. Nano energy, 2018, 47: 512-518.

  </div>
</div>
