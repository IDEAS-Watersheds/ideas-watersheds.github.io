---
layout: page_resources
title: Success Stories
subtitle: Flexible software infrastructure for bridging scales in simulations benefits multiple projects
permalink: /success-stories/stories/flexible-infrastructure
hero_image: /img/black.jpg
hero_height: is_fullheight

---
<style>
	.info-box{ 
		border: 1px solid black; 
		padding: 25px;
		margin-bottom: 20px;
		background-color: #d3eaf2;
		font-size: 12px;
	}
</style>

<div class="info-box" style= "margin-left: 25px; float: right; width: 30vw; ">
	<h4><b><i>Key Takeaways</i></b></h4>
	<ul>
		<li>Multiscale models are often intuitive to domain scientists and modelers but difficult to implement in software, so often one-off and unsustainable simulations are developed.</li>
		<li>By taking a best practices approach and recognizing characteristics of the mesh-infrastructure design that are common across many multiscale settings IDEAS-Watersheds developed infrastructure that can be reused and extended.</li>
		<li>Initial design and first success were with the NGEE-Arctic intermediate scale hydrology model, which NGEE-Arctic continues to use and extend today.</li>
		<li>Following the natural progression from hydrology to hydro-biogeochemistry the collaboration with the WaDE SFA led to an additional extension to implement a new multiscale method in streambed biogeochemistry modeling.</li>
		<li>These capabilities were released in the software ecosystem and are available to all ESS projects as well as the broader community.</li></ul>
</div>
<p>Scientists seeking to build process-based models for the hydrological and biogeochemical function of the nation’s watersheds must confront the multiscale nature of those systems. Much of our fundamental understanding of critical hydro-biogeochemical processes exists from studies at laboratory and plot scales. Those fine-scale processes interact with spatial heterogeneity across a wide-range of space and time scales to control watershed-scale hydro-biogeochemical function. Unfortunately, no generic modeling framework exists to bridge those scales, and computational watershed scientists have traditionally had to rely on one-off ad-hoc approaches to incorporate detailed process understanding in watershed-scale models. That approach often required significant effort and was plagued by significant uncertainties.</p>
<p>The IDEAS-Watersheds project has made significant contributions to the long-standing challenge of multiscale watershed modeling, thus allowing detailed process understanding developed from plot- and site-scale investigations to be incorporated in watershed-scale models. In particular, the project extended the integrated surface/subsurface hydrology model ATS to support a collection of fine-scale models for important processes that operate below the mesh resolution of a large-scale model. Importantly, each subgrid model can receive information from and provide information to the larger-scale model as the simulation proceeds, a configuration that is often referred to as an inline multiscale model. Inline multiscale models are intuitively appealing and closely match how hydrologists and biogeochemists think about watershed hydro-biogeochemical function, but are difficult to implement in software.</p>
<p>The multiscale modeling capability in ATS resulted from partnerships with the multilab  <a href="https://ngee-arctic.ornl.gov/">NGEE-Arctic</a> project and ORNL’s <a href="https://wade.ornl.gov/">WaDE Science Focus Area</a>. The partnership with NGEE-Arctic was one of the use cases of the original <a href="https://ideas-productivity.org/activities/ideas-classic/">IDEAS-Classic</a> project. That use case partnership developed an intermediate-scale model for permafrost hydrology of ice-wedge polygonal tundra in ATS (see box 1). The intermediate-scale model (Jan et al. 2018a,b) allowed NGEE scientists to simulate, for the first time, the co-evolution of polygonal tundra microtopography and hydrology at catchment scales (Painter et al. 2023). The NGEE-Arctic team adopted the ATS intermediate-scale model in 2018 and continues to develop and use it as a way of informing Arctic parameterizations in land surface models. </p>

<div class="info-box" style= "margin-right: 25px; float: left; width: 35vw; ">
		<center>
			<img src="/img/polygonal.png" max-width="200px">
			<img src="/img/tundra.png" max-width="200px">
		</center>
		<br><h4><b><i>Multiscale Model of Polygonal Tundra Motivates Design</i></b></h4>
		Ice-wedge polygon tundra, depicted in the artist’s rendering on the left, is a common type of landscape in lowland Arctic regions. In these low-relief carbon-rich environments, small variations in topography at scales of a few meters have outsized effects on watershed-scale hydrology and the carbon cycle. An intermediate-scale model developed through a partnership between the IDEAS and NGEE-Arctic projects makes it possible to represent those effects of microtopography. The model approximates the three-dimensional system with a collection of one-dimensional column models that are each coupled to a two-dimensional overland thermal flow model (Jan et al., 2018), as depicted on the right. This mixed-dimensional approximation is the result of conceptual understanding developed by permafrost scientists from detailed simulation and observation work. The partnership made it possible to express that understanding in software. With this new capability, NGEE-Arctic scientists were able to perform first-of-a-kind simulations of the co-evolution of microtopography and permafrost hydrology caused by melting of unevenly distributed ground ice (Painter et al. 2023). The mesh infrastructure required to implement this model has been reused in other multiscale models (see Box 2).		
</div>
<p>The NGEE-Arctic multiscale model was enabled by two key enhancements to ATS. First, ATS’s mesh infrastructure was extended to allow one-dimensional column meshes to be extracted from a primal three-dimensional mesh and then used in column simulations that are each coupled to the surface flow system but otherwise mutually independent. Second, time stepping in ATS was extended to allow columns to independently evolve between specified synchronization times where they exchange information with the surface flow system. </p>
<p>The resulting flexible mesh manipulation infrastructure that allows for multiple meshes and submeshes with different process representations and advanced time-stepping capability that allows for subcycling of different submodels are unique to ATS and enable many different types of multiscale models. These enhancements were later re-used to build a multiscale model for reactive transport in stream corridors as part of a use case partnership with the Critical Interfaces SFA (now the WaDE SFA). The multiscale stream corridor model (Box 2) makes it possible to represent the effects of small-scale biogeochemical hotspots in the saturated sediment adjacent to a flowing stream in river-basin scale simulations (Jan et al. 2021). The approach associates a subgrid model for hyporheic-zone reactive transport with each grid cell in a relatively coarsely discretized basin-scale model of the riverine network. The model has been successfully compared with results of stream tracer tests (Rathore et al. 2021; Phong et al. 2023,2024) and used to evaluate novel strategies for combining multiple types of tracers to characterize stream corridor processes (Rathore et al. 2024). The WaDE SFA is currently using the capability to build whole-watershed models of stream oxygen dynamics. </p>


<div class="info-box" style= "float: right; margin-left: 25px; width: 35vw; ">
	<center>
		<img src="/img/stream-channel.png" max-width="200px">
		<img src="/img/channel-grid.png" max-width="200px">
	</center>
	<br><h4><b><i>Multiscale Modeling of BGC in Stream Channels</i></b></h4>
	<p>Many of the important biogeochemical processes that transform or remove carbon, contaminants, and excess nutrients occur in highly localized regions in saturated sediments adjacent to the stream channel, as illustrated schematically in the top panel. How to tractably represent those fine-scale hyporheic-zone biogeochemical processes in watershed-scale models is a long-standing challenge for efforts to build process-based models of watershed hydro-biogeochemical function. The IDEAS-Watersheds project partnered with the Critical Interface SFA at ORNL to develop and test a unique multiscale model (Painter 2018) that addresses that challenge. The multiscale model attaches a subgrid model for hyporheic-zone transport and reactions to each grid cell in a channel network flow model, as shown schematically in the right panel. The subgrid models are expressed in a stochastic travel time form that efficiently accounts for a diversity of flowpaths through the hyporheic zone. The mesh infrastructure that made that implementation in ATS possible was the result of the previous NGEE-Arctic partnership (see Callout 1). A subsequent partnership with ORNL’s Watershed Dynamics and Evolution (WaDE) SFA developed methods to estimate parameters in the multiscale model from stream tracer data (Rathore et al. 2021), extended it to accommodate unsteady channel flow (Le et al. 2023), and used it to evaluate tracer test designs (Rathore et al. 2023). The WaDE SFA is currently using it to build full-watershed models of stream metabolism.</p> 
</div>
<p>
This example is typical of how IDEAS-Watersheds partners with other projects to improve the scientific community’s capacity to simulate the hydrological and biogeochemical function of the nation’s watersheds. The IDEAS-Watersheds team co-designed the strategy with the partner projects and then implemented the enabling software capability in our community <a href="https://ideas-watersheds.github.io/software-ecosystem">software ecosystem</a>. Testing and demonstration activities were undertaken jointly, thus ensuring a seamless transfer of the capability. The <a href="https://ideas-watersheds.github.io/research/infrastructure">software stewards</a> of IDEAS-Watersheds continue to provide further support and maintenance for the capability as it adopted by the broader scientific community. Our experience with this development model confirms that it significantly improves scientific productivity of computational watershed scientists through greater software reuse and improvements to software quality, which allows environmental systems scientists to focus on science not software. 
</p>