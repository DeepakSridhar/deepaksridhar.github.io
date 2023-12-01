---
layout: page
title: Scalable Channel Mixer for Vision Transformers
description: Generic channel mixer to scale all ViTs
img:
importance: 1
category: work
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/CARMixer_and_Inference.png" title="Architecture" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Proposed SCHEME channel mixer. The channel mixer of the standard transformer consists of two MLP layers, performing dimensionality expansion and reduction by a factor of $E$. SCHEME uses a combination of a block diagonal MLP (BD-MLP), which reduces the complexity of the MLP layers by using block diagonal weights, and a channel covariance attention (CCA) mechanism that enables communication across feature groups through feature-based attention. This, however, is only needed for training. The weights (1-alpha) decay to zero upon training convergence and CCA can be discarded during inference, as shown on the right. Experiments show that CCA helps learn better feature clusters, but is not needed once these are formed.
</div>

<div class="row">
    <div class="col-sm">
        <a href="">SCHEME: Scalable Channel Mixer for Vision Transformers</a>
    </div>
</div>
