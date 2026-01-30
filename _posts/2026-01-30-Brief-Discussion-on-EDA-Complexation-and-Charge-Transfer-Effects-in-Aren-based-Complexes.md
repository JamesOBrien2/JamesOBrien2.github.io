---
layout: post
title: A Brief Discussion on EDA Complexation and Charge-Transfer Effects in Arene-based complexes
date: 2026-01-30 18:41:00
description:
tags: Chemistry
categories: discussion
---

# Brief Discussion on EDA Complexation and Charge-Transfer Effects in Arene-based complexes

This discussion is strongly encouraged from a reading of the book chapter "Charge-Transfer Effects on Arene Structure and Reactivity" by S. V. Rosokha and J. K. Kochi.

## Electron Donor-Acceptor Complexation

Arenes are surprisingly sociable molecules. They'll oftentimes "hang out" with electron-poor partners (electrophiles, cations, oxidants, Lewis Acids etc.). Whereby, an electron rich molecule (arena) can form a preorganised complex Whilst, these complexes remain unreacted, they can preorganise together into a prereactive complex, which can be experimentally observed. These systems can allow for the formation of some interesting systems such as EDA Complexes (eq. 1) and exciplexes (eq. 2).

$$
D + A \rightarrow [D,A] \xrightarrow{h\nu_{CT}} [D^{+},A^{-}]^{*}
\tag{1}
$$

<!-- ## (Check paper to revise this and cite it!) -->

$$
D + A \xrightarrow{h\nu} D^{*} + A \rightarrow [D^{+},A^{-}]^{*}
\tag{2}
$$

According to Mulliken's quantitative description of intermolecular (Charge-Transfer) complexes, an EDA complex isn't an "all-or-nothing electron transfer". Instead, the ground state is a mixture of a mostly neutral "van der Waals / no-bond" description and a partly ionic "charge-transferred / dative" description. As a result of this mixing, a new optical transition (the CT band) is formed.

Furthermore, Mullikan infers that hv<sub>CT</sub> derives from a single electron transfer from the donor to the acceptor. <!-- as shown in the MO diagram below.-->

<!--![Simple EDA MO Diagram]({{ '/assets/img/blogs/example_MO_EDA_diagram.png' | relative_url }}){: style="width:100%; height:auto;"}
-->

## Donor Vs. Acceptor

Typically chemists will use their intuition when denoted an electron donor or acceptor. However, this is not a quantitative measurement. Therefore, how are donor and acceptor strengths typically measured?

In solution, donor strength is commonly related to oxidation potential (E<sup>°</sup><sub>ox</sub> , eq. 3) and acceptor strength is similarly related to reduction potential (E<sup>°</sup><sub>red</sub> , eq. 4).

$$
R \xrightarrow{E^°_{ox}} R^{\bullet+}
\tag{3}
$$

$$
R \xrightarrow{E^°_{red}} R^{\bullet-}
\tag{4}
$$

Practically, fully reversible redox potentials aren'talways accessible for reactive aromatic radical ions, so people often compare irreversible peak potentials from cyclic voltammetry. However, these values contain kinetic contributions, any comparison with the values of E° is restricted to structurally similar donors.

In gas phase, ionisation potential (IP) and electron affinity (EA) can be similarly used to determine electron donor/acceptor strengths. These values differ from redox potentials due to lack of solvation contributions to the energetics.

## The CT Band

The most recognisable fingerprint of an EDA complex is the formation of a new absorption band in the UV/vis/NIR spectrium that neither the free donor nor the free acceptor has on its own.

<!-- ![New Absorption Band in Complex]({{ '/assets/img/blogs/example_new_absorption_band.png' | relative_url }}){: style="width:100%; height:auto;"} -->

As previously noted, Mulliken's interpretation denotes that shining light at that CT band corresponds to promoting an electron within the complex from donor to acceptor, generating an ion-radical pair in an electronically excited (Franck-Condon) state (eq. 1).

For a set of similar donors (or similar acceptors), this CT transition energy often tracks donor/acceptor energetics in a simple way:

$$
h\nu=IP-EA+constant
\tag{5}
$$

This lets us predict trends, as if you make the donor easier to oxidise (lower IP, or lower E<sup>°</sup><sub>ox</sub>), you generally produce a lower energy CT band (longer wavelength), due to the electron transfer inside the complex becoming "less uphill". For example, swapping benzene for anisole produces a redshifted CT band because anisole is a stronger electron donor.

![Redshifted Absorption Band in Complex]({{ '/assets/img/blogs/example_redshifted_CT_band.png' | relative_url }}){: style="width:60%; height:auto;"}

## Weak vs. Strong CT complexes

As the difference in redox potentials between the Donor and Acceptor become smaller, the photoexcitation becomes smaller, and for strong enough complexes this absorption becomes better described by bonding/antibonding (MO) instead of as a CT transition.

Spectral behaviour of a strong CT complex can be shown with NO+ complexation to a series of arenes.

For weak complexes with relatively small orbital ovelap / a large HOMO/LUMO gap, the value of charge-transfer contribution is small. Resulting in less pronounced changes on the donor complex's IR band shift. The effects of which are detailed in the table below.

|     Donor      | Acceptor | Stretching Band (cm⁻¹) |
| :------------: | :------: | :--------------------: |
| Cl<sub>2</sub> |   None   |          557           |
| Cl<sub>2</sub> | Benzene  |          527           |
| Cl<sub>2</sub> | Toluene  |          524           |

<!-- ## Thermodynamics of CT Complexation

Formation constant K<sub>CT</sub> is one of the primary measures for donor/acceptor binding in CT complexes. The formation constant can be determined by absorption spectroscopy through utilising Benesi-Hildebrand treatment.
-->
