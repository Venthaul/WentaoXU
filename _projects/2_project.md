---
layout: page
title: GABA-AT inhibitor design
description: Using binding free energy calculation to guide drug design. A set of AI tools are examed and intergrated in workflow.
img: assets/img/project2/drug.png
importance: 1
category: work
giscus_comments: true
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


<p style="text-align: justify;">
In the task of drug design, we need to break down "designing molecules" into several sub-tasks: skeleton optimization, functional group optimization, and pharmacokinetic optimization. These tasks, with the support of AI, are often integrated into various "molecular generation" models. However, the improvement of "binding affinity" by this type of molecular generator is unclear. Therefore, in this project, I mainly study how to wisely combine AI methods with molecular mechanics methods to find an appropriate drug design strategy.
</p>
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/project2/figure2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This image can also have a caption. It's like magic.
</div>

<div class="row">
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/project2/e_samle2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/project2/fig2.2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    You can also have artistically styled 2/3 + 1/3 images, like these.
</div>



The code is simple.
Just wrap your images with `<div class="col-sm">` and place them inside `<div class="row">` (read more about the <a href="https://getbootstrap.com/docs/4.4/layout/grid/">Bootstrap Grid</a> system).
To make images responsive, add `img-fluid` class to each; for rounded corners and shadows use `rounded` and `z-depth-1` classes.
Here's the code for the last row of images above:

{% raw %}

```html
<div class="row justify-content-sm-center">
  <div class="col-sm-8 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/6.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm-4 mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/11.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
```

{% endraw %}
