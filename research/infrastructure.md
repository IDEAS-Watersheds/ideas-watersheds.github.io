---
layout: page_research
title: Shared Infrastructure Activity 
permalink: /research/infrastructure
hero_image: /img/IDEAS-Watersheds-banner.jpg
hero_height: is_fullheight

---

<style>
    .cont {
      display: flex;
      flex-wrap: wrap;
      column-gap: 20px;
    }

.col1 {
      flex: 3; 
      min-width: 400px;
    }

.col2 {
      flex: 2;
      min-width: 400px;
    }

</style>

# Project Structure and Approach

Although the modeling strategies adopted by various activities within SBR differ in important details, they share significant modeling challenges and infrastructure needs. Shared computational infrastructure needs include workflow tools for transferring information across scales, customized meshing, and model-data integration, and interfaces to couple multiple process-based codes and support code interoperability.

The IDEAS-Watersheds Shared Infrastructure Activity will coordinate the development of the shared infrastructure by creating and advancing existing multiscale workflow tools and software interfaces to support interoperability.

The Shared Infrastructure can be shared among the SFAs to support those multi-scale models and reduce duplication of effort and ensure long-term sustainability of the capability.

<br>
<h3>The IDEAS-Watersheds Shared Infrastructure Activity includes:</h3>
<div class="cont">
  <div class="col1">
    <ul>
      <li><strong><em>Multiscale Workflow Tools for hydrobiogeochemical simulations and analyses across multiple resolutions and scales</em></strong></li>
        <ul>
          <li> multi-resolution unstructured meshes that conform to stream/river geometries and allow refinement in and near river corridors</li>
          <li> using metagenomics data for reaction network generation</li>
          <li> etc.</li>
          </ul>
      <li><strong><em>Interfaces</em></strong></li>
      <ul>
        <li> Continue development of formalized interfaces to support code interoperability, focusing on further development of Alquimia and a land-model interface</li>
        </ul>
      <li><strong><em>Sustainable Software Ecosystem</em></strong></li>
  </ul></div>
  <div class="col2"><img width="75%" src="/img/shared_infrastructure.png"></div>
</div>

<div>
<h3>The IDEAS-Watersheds Shared Infrastructure Activity</h3>
      <ul>
        <li> Extends the BER ecosystem of interoperable software tools and components to better represent hydrobiogeochemical processes in dynamic stream/river corridors along the river continuum.</li>
        <li> Provides software tools and workflows that can be shared among the Science Focus Areas (SFA's) as well as the critical (and currently incomplete) experience base on how to parameterize and use the new capabilities.</li>
      </ul>
</div>
<br>

*Image: Example relationship of modeling domains across scales: the multiscale workflow activity will enable model output to be used to drive boundary conditions of models at finer scales. Workflows will also be developed to work with model input data in native formats and scales, and map it to the desired computational mesh. Particle-based methods are being advanced to analyze scaling relationships and identify potential strategies for bridging fine-scale mechanistic models and understanding to larger scales.*