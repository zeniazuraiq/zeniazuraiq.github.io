---
layout: page
title: Simulating super-Chandrasekhar white dwarfs
description: tracing the formation and evolution of massive, magnetized whtie dwarfs
img: assets/img/bwd_hr_2.png
importance: 2
category: selected projects
---

The famous Chandrasekhar limit was derived back in the 1930s, with Subrahmanyan Chandrasekhar receiving the Nobel Prize for this work in 1983. However, this limit was derived under the assumption of ideal Fermi gases at zero temperatures. Further, effects like rotation and magnetic fields are not considered during the derivation. In fact, there are observations that indicate the violation of this mass limit. Several over-luminous peculiar type Ia supernovae, e.g. SNLS-03D3bb, argue their respective progenitor to be a significantly super-Chandrasekhar WD with a mass-limit higher than the Chandrasekhar limit. 

It has been shown in previous work that the magnetic fields of WDs can lead to higher masses being supported by the star. The magnetic field can lead to both classical and quantum effects on the eventual mass of the star. In fact, previous work showed that in the presence of a magnetic field, there can be a series of mass limits, depending on the type of field geometry and profile present within the WD considered. 

In the current work, we explore the formation and time-dependent evolution of magnetic WDs. For this, we use the Cambridge stellar evolution code, STARS. We explore in detail the evolutionary path taken by a magnetized main sequence star (MS) as it forms a BWD. To fully incorporate the magnetic effects, we have introduced magnetic fields to STARS by modifying the code appropriately.

Through our simulation, we also explore the possible formation scenarios for magnetized, super-Chandrasekhar WDs. 
We explore a formation channel based on accretion. In the initial part of stellar evolution, for magnetic fields upto 10^12 G, the magnetic field is largely dormant and does not affect the evolution. However, on subsequent evolution through accretion, the star gains mass, leading to the strengthening of its magnetic field, and hence the star has enhanced pressure to support additional mass. This leads to super-Chandrasekhar WDs. We have investigated the possible parameter space where this evolution can play out - and we find that under a combination of appropriate profile, accretion rate, and composition of accreted material, stable, super-Chandarasekhar WDs are realizable as end points of realistic stellar evolution.

We explore further the properties of the formed WDs. An important source of deviation from the Chandrasekhar relation other than the magnetic effect is the finite temperature effect. The cores of WDs are isothermal, but there is a finite temperature gradient in the core-crust interface. A combination of the magnetic field and finite temperature effects lead to low mass WDs having larger radii, and showing deviation from the Chandrasekhar relation. This has interesting observational implications, and can be a way to probe the magnetic field effects indirectly.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/bwd_hr_2.png" title="bwd hr" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Evolution of MSs of various masses to WDs in H--R diagrams, where $L$ is the luminosity and $T_{\rm e}$ the effective temperature of the star. The solid, dashed and long-dashed lines show the evolution from MS to WD without accretion, from bottom to top: for $3,~5$ and $8M_\odot$ MSs. Accretion at $\dot{M} = 10^{-9}\,M_\odot\,{\rm yr}^{-1}$ on to the $1.02M_\odot$ WD with an initially dormant magnetic field leads to a $2.4\,M_\odot$ B-WD (dotted line), whereas without magnetic field forms a $M_{\rm Ch}=1.4M_\odot$ WD (dash-dotted line). 
</div>


<i> You can find further details of this work here: [Zuraiq et al.](https://doi.org/10.1007/978-3-031-90186-7_32)</i>