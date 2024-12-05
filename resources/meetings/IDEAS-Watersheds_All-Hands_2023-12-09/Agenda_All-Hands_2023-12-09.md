---
layout: page_resources
title: IDEAS-Watersheds (Phase 2) All Hands Fall 2023
permalink: /resources/meetings/IDEAS-Watersheds_All-Hands_2023-12-09
hero_image: /img/black.jpg
hero_height: is_fullheight

---

<style>
    .cont {
      display: flex;
      flex-wrap: wrap;
    }

.col1 {
      flex: 2; 
      min-width: 200px;
    }

.col2 {
      flex: 3;
      min-width: 200px;
    }

</style>

<body>
    <div class="cont">
        <div class="col1">
            <h4>
            December 9-10, 2023<br>
            Stanford University<br>
            Green Earth Sciences Building <br>
            367 Panama Mall Stanford<br>
            Room 365 <br>
            <a href="https://campus-map.stanford.edu">Campus Map</a> 
            </h4>
        </div>
    <div class="col2">
        <img src="/img/photos/all_hands_group_photo.png" align="right"><br>
    </div>
</div>
</body>

# Meeting Agenda:

#### Day 1: Saturday Noon-5PM (PST)

|Wall Clock (PT) |  Elapsed Time (min)    | Talks/Activity
|:---------------|:-----------------------|:-----------------------------------------------------|
|12:00|15|Introductions and Project Overview|
|12:15|45|Icebreaker Activities|
||**SFA Partnership Updates**||
|1:00|8+2|LBNL Watershed Function SFA: Sergi Molins|
|1:10|8+2|ORNL Watershed Dynamics and Evolution SFA: Scott Painter|
|1:20|8+2|PNNL River Corridor SFA: Xingyuan Chen|
|1:30|8+2|Shared Infrastructure: David Moulton|
|1:40|20|Group discussion and activities|
|2:00|**Break** (30 min)||
||| **Hands - On:** Integrated Hydrology + RTM (Lead: Sergi Molins)<br>**Duration:** 2 - 2.5 hours <br>**Details:** Including objectives and instructions are in available in the [README.md](https://github.com/IDEAS-Watersheds/integrated-reactive-transport-hands-on/blob/main/README.md)|
|2:30||Set up an integrated tracer transport problem in a column building on ATS integrated hydrology inputs (Sergi)|
|||Set up and test a geochemical problem in PFLOTRAN (Glenn) docker run -p 8888:8888 pflotran/jupyter:ideas-dec23-all-hands|
|||Set up a reactive transport problem building on the column simulation and PFLOTRAN inputs, LIVE! debugging (Sergi and Glenn)|
|||Set up more complex simulations: the hillslope example (Sergi)|
||**Break**||
||**Adjourn**||

<br><br>
#### Day 2: Sunday 9:00 AM -- 5PM (PST)

|Wall Clock (PT) |  Elapsed Time (min)    | Talks/Activity
|:---------------|:-----------------------|:-----------------------------------------------------|
|| | **Flash Talks** |
|9:00|4+1|Phong Le (ORNL) A Multiscale Integrated Model for Transport in River Basins|
|||Saubhagya Rathore (ORNL) Spatially Resolved Integrated Hydrology Modeling for Managed Watersheds|
|||Jesus Gomez Velez (ORNL) Nitrate uptake in the benthic biolayer of streams and rivers across Conterminous US|
|||Zhi Li (PNNL) Modeling the fates of pyrogenic carbon in the wildfire-impacted watersheds using ATS-PFLOTRAN|
|||Tasneem Ahmadullah (PNNL) Organic Carbon Speciation in Microbial Respiration Using Lambda-PFLOTRAN Pipeline|
|||Mingjie Shi (PNNL) Ecosystem responses to wildfires in the Columbia River basin|
|||Lijing Wang (LBNL) Understanding Hydrologic Variability in Mountainous Hillslopes: From Intensive Monitoring to Scaling Up.|
|||Dipankar Dwivedi (LBNL) Reactive Transport Benchmarks for Problems Involving Gaseous Species.|
|||Andrew Graus (LBNL) Status update on coupling a fine-scale process-based ecosystem model (EcoSIM) with the Advanced Terrestrial Simulator (ATS).|
|||Luwen Wan (Stanford) Quantifying beaver-induced water storage across scales.|
|||Discussion|
|**10:00**| **Break (30 min)**||
|||**Hands-On:** WW and Mixed-Polyhedral meshing (Lead: Saubhagya Rathore) <br>**Duration:** 2.5 hours <br>**Details:**  Including objectives and docker setup is [here](https://github.com/environmental-modeling-workflows/workshop-watershed-workflow/blob/main/README.md).|
|10:30||Introduction to Watershed Workflow|
|||Exploring Key Conceptual Objects|
|11:15||**Hands-On Session:** Generating Stream-Aligned Mixed-Polyhedral Mesh|
|||Defining Regions and Labeled Sets|
|12:15||Debugging and Manipulating Key Objects|
|||Discussion and Feedbacks|
| **1:00**| **Lunch (1 hour)**||
|||**Hands-On:**  IHSI subsetting CONUS 2.0 data and simulation output <br> **Duration:** 2.5 hours <br> **Details:** Including objectives and docker instructions are in available in the [README.md](https://github.com/gartavanis/IDEAS-watersheds/blob/main/README.md)|
|2:00||Overview of new datasets, CONUS2|
|||Presentation of the new tools, the HydroFrame and HydroData and SubsetTools frameworks|
|||**Hands-on Session:** subset tools/hf_hydrodata sessions with Docker|
|||Discussion/Feedback|
|4:30|| **Group discussion:** **What’s next, what do you need, what’s slowing you down? (~1 hour)**|
|5:00| **Adjourn**||

<br>

