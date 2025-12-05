---
layout: page
title: GABA-AT inhibitor design
description: Using binding free energy calculation to guide drug design. A set of AI tools are examed and intergrated in workflow.
img: assets/img/project2/drug.png
importance: 2
category: work
related_publications: false
---

<p style="text-align: justify;">
In the task of drug design, we need to break down "designing molecules" into several sub-tasks: skeleton optimization, functional group optimization, and pharmacokinetic optimization. These tasks, with the support of AI, are often integrated into various "molecular generation" models. However, the improvement of "binding affinity" by this type of molecular generator is unclear. Therefore, in this project, I mainly study how to wisely combine AI methods with molecular mechanics methods to find an appropriate drug design strategy.
</p>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/project2/figure1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    A drug design process that combines multi-perspective calculation schemes. Functional groups and backbones were designed and combined through various AI software and chemical intuition. Molecular docking and MMGBSA were used for rough screening, and finally the binding mechanism was studied by a strict free energy method.
</div>

<p style="text-align: justify;">
Firstly, we employ a structure-based drug design strategy, dividing the task into two sub-tasks: backbone hopping and terminal functional group design. And in combination with the AI tool Delinker, a molecular library consisting of 20,000 molecules was constructed for screening. These molecules can all geometrically fit well into the target pocket. Not only do we hope to find potential candidate molecules among these 20,000 molecules, but also we aim to obtain a binder database for GABA-AT through free energy calculations. Such a database can be used as a fine-tuning dataset for the subsequent training of the molecular generation model.
</p>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/project2/figure2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

We tested various methods for combining calculations with free energy (mainly focusing on time consumption and operational convenience), including umbrella sampling, funnel-metadynamics, and absolute/relative FEP. Eventually, we decided to adopt the FEP approach and used the PyAutoFEP package to achieve automation. Finally, we decided to adopt the FEP approach and used the PyAutoFEP package to achieve automation.
<div class="row">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/project2/e_samle2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/project2/fig2.2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

When conducting the calculation of Relative FEP, we perform "mutations" on the "head" and "tail" regions of the molecule.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/project2/drugai.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>