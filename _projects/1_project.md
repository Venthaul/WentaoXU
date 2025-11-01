---
layout: page
title: Conformational Dynamics of Spike Protein
description: The open-close conformational landscape of the SARS-CoV-2 spike protein undergone evolution as the virus has evolved.
img: assets/img/project1/figure1.jpg
importance: 1
category: work
related_publications: false
---

<p style="text-align: justify;">
The conformational transition of the receptor binding domain (RBD) of the SARS-CoV-2 spike (S) protein from the “closed” to the “open” state is an important dynamic event influencing the infectivity of the virus.  However, how accumulating mutations reshape these conformational dynamics during viral evolution remains to be clarified.  In this study, we observed the motion of the RBD of fully glycosylated S protein trimers from wild type to Omicron (BA.2, BA.4&5) variants by using all-atomic molecular dynamics simulations.  Our study indicates that, although a fully converged free energy landscape in all motion directions was not obtained, analysis of the molecular dynamics trajectories reveals significant differences in the RBD motional patterns among variants due to mutations.  These changes in motion patterns suggest a potential evolution of the conformational dynamics free energy landscape.  We found that this mechanistic divergence is closely correlated with the motional patterns of the N165 and N343 glycan, which are modulated by variant-specific surface mutations.  This work highlights a connection between surface mutations and glycan dynamics, providing a mechanistic basis for understanding viral evolution and function.
</p>

<div class="row">
    <div class="col-sm mt-3 mt-md-0" style="max-width: 400px; margin-left: auto; margin-right: auto;">
        {% include figure.liquid loading="eager" path="assets/img/project1/BA45_MetaD_traj.gif" title="Metad traj" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The closed-to-open process of the spike protein RBD (Red part) is an important process for viruses to invade the human body. During this process, the glycans (Blue and Orange part) on the surface of the spike protein play a significant role. {% cite sztain_glycan_2021 %} {% cite casalino_beyond_2020 %} 
</div>

<p style="text-align: justify;">
Molecular dynamics (MD) simulation combined with enhanced sampling methods and free energy calculation is a powerful tool for studying functional roles of SARS-CoV-2 proteins at the atomic level. For example, free energy calculations via 2D umbrella sampling have been used to explore the impact of a single mutation on this transition process, providing insights into the dynamic evolution of spike proteins, even when the specific mutations studied did not become prevalent variants {% cite fallon_free_2021 %}. Other work focused on the influence of distant residues, demonstrating that the analysis of residue motion synergy from MD trajectories can provide profound insights for predicting the outcomes of distant mutations {% cite ray_distant_2021 %}. Furthermore, research on the surface glycans of the spike protein has innovatively revealed their key regulatory role in the conformational dynamics of the RBD. Studies combining conventional molecular dynamics simulations with experimental validation first demonstrated that N-glycans at sites N165 and N234 play an essential structural role by stabilizing the RBD in the open conformation {% cite casalino_beyond_2020 %} .
</p>
<p style="text-align: justify;">
Subsequently, a distinct mechanistic contribution was uncovered through weighted ensemble simulations, which showed that the N343 glycan acts as a “glycan gate”, actively facilitating the closed-to-open transition by interacting with the RBD surface {% cite sztain_glycan_2021 %} . These findings highlight two different aspects of glycans’ influence: stabilization of the open state and facilitation of the opening transition. This understanding has been quantitatively refined by 2D free energy surface constructed using replica exchange umbrella sampling, which showed that glycans increase the energy barrier to opening and highlighted the roles of N165 and N343 in stabilizing both the up and down states {% cite pang_sars-cov-2_2022 %}. Further investigations have explored how the specific type and size of glycans at these key sites (N165, N234, N343) fine-tuned the stability of the open RBD, and examined the evolutionary implications of changes in the glycan shield topology, such as the loss of the N370 glycosylation site in SARS-CoV-2. These important studies have established that factors, from key mutations such as D614G to specific glycans such as N165, can play crucial regulatory roles in the S protein conformational dynamics.
</p>

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/project1/fep.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    We used Metadynamics in combination with Reweighting to plot the free energy surface, which was used to monitor and compare the conformational dynamics of RBD of different variants.
</div>
