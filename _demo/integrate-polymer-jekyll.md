---
title: Polymer Integration with Jekyll
description: Integrating Polymer in Jekyll is very simple. Polymer elements are the future of web design. Polymer is an ambitious project by Google which might take off a lot of burden on web designers and developers.
keywords: polymer Jekyll, polymer github pages, polymer and github.
article: /integrate-polymer-jekyll/
layout: demo
---



<link rel="import" href="https://cdn.rawgit.com/download/polymer-cdn/1.1.4/lib/paper-card/paper-card.html"/>


## Jekyll Polymer Demo

<div class="inline">
<paper-card heading="Card Title" class="card-ex">
  <div class="card-content">Some content</div>
  <div class="card-actions">
    <paper-button>Some action</paper-button>
  </div>
</paper-card>
 
 <paper-card heading="Card Title" class="card-ex" style="background-color: #B67CE0">
  <div class="card-content">Some content</div>
  <div class="card-actions">
    <paper-button>Some action</paper-button>
  </div>
</paper-card> 
 
 <paper-card heading="Card Title" class="card-ex" style="background-color: #7CE0BA">
  <div class="card-content">Some content</div>
  <div class="card-actions">
    <paper-button>Some action</paper-button>
  </div>
</paper-card>
</div>

<style>
.inline {
    margin: 2em 0;
}
paper-card {
    margin-left: 10px;
}
</style>