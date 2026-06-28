---
layout: page
title: Mechanistic Elucidation
description: Computational characterisation of reactive intermediates and conformational landscapes
img: assets/img/projects/mechanistic_elucidation.png
importance: 3
category: work
related_publications: true
---

A significant component of my research has involved elucidating reaction mechanisms and rationalising biological activity through computational chemistry, in collaboration with synthetic and biochemical groups. These studies apply density functional theory (DFT) for potential energy surface mapping and excited-state characterisation, as well as conformational analysis, to investigate systems that are experimentally inaccessible or difficult to characterise directly.

---

## Periodate Photoactivation and Oxene Generation

In collaboration with Dr Aaron Trowbridge's group (University of Manchester), DFT calculations were employed to rationalise the experimentally observed oxenoid reactivity arising from the violet-light photolysis of tetrabutylammonium periodate {% cite bossonet2024oxene %}. Excited-state calculations revealed an unexpected geometric change upon photoexcitation of periodate (IO₄⁻) that facilitates intersystem crossing to the triplet manifold. Subsequent potential energy surface mapping demonstrated near-barrierless dissociation of triplet periodate to generate a triplet oxene species, accounting for the broad epoxidation reactivity observed experimentally across a diverse substrate scope.

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/io4_dissociation.gif" title="Triplet periodate dissociation to oxene" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
    DFT-computed dissociation of triplet periodate (IO₄⁻) along the potential energy surface, generating a triplet oxene intermediate. Collaboration with Dr Aaron Trowbridge (University of Manchester).
</div>

---

## Macrocyclic Peptide Synthesis via Photochemical Radical Thiol–yne Cyclisation

In collaboration with Prof Eoin Scanlan's group (Trinity College Dublin), conformational analysis was applied to rationalise the divergent biological activities of vinyl sulfide macrocyclic peptide analogues produced via a photochemical radical thiol–yne strategy {% cite williams2026thiolyne %}. A conformational search was performed on three macrocyclic systems using GOAT-DIVERSITY, sampling thermally accessible and inaccessible conformers within an energy cutoff of 60 kcal mol⁻¹: endogenous oxytocin, the (<i>Z</i>)-vinyl sulfide analogue, and the (<i>E</i>)-vinyl sulfide analogue. The (<i>Z</i>)-analogue exhibited a single dominant conformer accounting for 99.8% of the sampled conformational space, closely mirroring endogenous oxytocin (97.1%), while the (<i>E</i>)-analogue displayed eight distinct major conformers spanning 1 to 35% population. This marked difference in conformational rigidity accounts for the enhanced potency of the (<i>Z</i>)-isomer at the human oxytocin receptor, where a well-defined, compact binding pose facilitates productive receptor interactions.

<div class="row justify-content-sm-center">
  <div class="col-sm-10 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/thiolyne_jacs_rotating.gif" title="Thiol–yne macrocyclic peptide systems" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
    Lowest-energy conformers of three macrocyclic peptide systems from GOAT-DIVERSITY conformational analysis: oxytocin (left), (<i>Z</i>)-analogue (middle), and (<i>E</i>)-analogue (right). Collaboration with Prof Eoin Scanlan (Trinity College Dublin).
</div>
