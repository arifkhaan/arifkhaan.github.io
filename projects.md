---
layout: page
title: Projects
subtitle: ''
head-title: ""
css: "../css/custom.css"
---

<div class="accordion" id="accordionExample">
  <div class="card">
    <div class="card-header" id="headingOne">
      <h2 class="mb-0">
        <button class="btn btn-link btn-block text-left" type="button" data-toggle="collapse" data-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
          AI Enabled Wireless Systen
        </button>
      </h2>
    </div>

    <div id="collapseOne" class="collapse show" aria-labelledby="headingOne" data-parent="#accordionExample">
      <div class="card-body">
        <img align="right" src="../img/unerconst.jpg" height="200px">
      </div>
    </div>
  </div>
  <div class="card">
    <div class="card-header" id="headingTwo">
      <h2 class="mb-0">
        <button class="btn btn-link btn-block text-left collapsed" type="button" data-toggle="collapse" data-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
          Heterogeneous Cellular Networks
        </button>
      </h2>
    </div>
    <div id="collapseTwo" class="collapse" aria-labelledby="headingTwo" data-parent="#accordionExample">
      <div class="card-body">
        <img align="right" src="../img/unerconst.jpg" height="100px">
      </div>
    </div>
  </div>
  <div class="card">
    <div class="card-header" id="headingThree">
      <h2 class="mb-0">
        <button class="btn btn-link btn-block text-left collapsed" type="button" data-toggle="collapse" data-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
          Soft Output Sphere Decoding Reciever for MIMO System
        </button>
      </h2>
    </div>
    <div id="collapseThree" class="collapse" aria-labelledby="headingThree" data-parent="#accordionExample">
      <div class="card-body">
        <img align="center" src="../img/model111.PNG" height="300px">
      </div>
    </div>
  </div>
</div>

<template>
  <Collapsible class="example-collapsible">
    <div slot="trigger">
      <div class="customTrigger">
        <h2>Custom open trigger element</h2>
      </div>
    </div>

    <div slot="closedTrigger">
      <div class="customTrigger">
        <h2>Custom closed trigger element</h2>
      </div>
    </div>

    <div id="example2">
      <p>
        Lorem ipsum dolor sit ...
      </p>
    </div>
  </Collapsible>
</template>

<script>
  import 'vue-collapsible-component/lib/vue-collapsible.css';
  import Collapsible from 'vue-collapsible-component';

  export default {
    components: {
      Collapsible,
    },
  };
</script>
