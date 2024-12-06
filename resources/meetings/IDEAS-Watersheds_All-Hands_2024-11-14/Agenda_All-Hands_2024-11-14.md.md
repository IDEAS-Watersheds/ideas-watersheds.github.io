---
layout: page_resources
title: IDEAS-Watersheds All Hands Fall 2024
permalink: /resources/meetings/IDEAS-Watersheds_All-Hands_2024-11-14
hero_image: /img/black.jpg
hero_height: is_fullheight

---

<style>
    .gallery {
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        grid-auto-rows: auto;
        grid-auto-flow: dense;
        gap: 6px;
        min-width: 200px;
    }

    img.four-grid-cells {
        grid-row: span 2 / auto;
        grid-column: span 2 / auto;
        width: 100%;
        height: 100%;
        object-fit: cover;
    }

    img.single-grid-cell {
        grid-row: span 1 / auto;
        grid-column: span 1 / auto;
        width: 100%;
        height: 100%;
        object-fit: cover;
    }

</style>

<div>
        <div class="gallery">
            <img class="four-grid-cells"
                src="/img/All-Hands_2024/IMG_6049.jpg"/>
            <img class="single-grid-cell"
                src="/img/All-Hands_2024/IMG_6051.jpg"/>
            <img class="single-grid-cell"
                src="/img/All-Hands_2024/IMG_6052.jpg"/>
            <img class="single-grid-cell"
                src="/img/All-Hands_2024/IMG_6053.jpg"/>
            <img class="single-grid-cell" 
                src="/img/All-Hands_2024/IMG_6050.jpg"/>
        </div>
</div><br><br>

<h4>
November 14-15, 2024<br>
Courtyard Marriott Denver Airport<br>
Denver, Colorado<br>
6901 Tower Road<br>
<a href="https://www.marriott.com/en-us/hotels/denap-courtyard-denver-airport/overview/">Hotel Map</a> 
</h4>

# Meeting Agenda:

#### Day 1: Thursday November 14, 2024 8:30AM-5:00PM (MST)

|Wall Clock (MT)|Elapsed Time (min)|Talks/Activity
|:---------------|:-----------------------|:-----------------------------------------------------|
|8:30|30|Coffee and Continental Breakfast|
|| | **Introductions**|
|9:00|10|Introductions and Project Overview|
|9:10|20|Icebreaker Activities|
|| | **SFA Partnership Updates**|
|9:30|8+2|LBNL Watershed Function SFA: Sergi Molins|
|9:40|8+2|ORNL Watershed Dynamics and Evolution SFA: Scott Painter|
|9:50|8+2|PNNL River Corridor SFA: Xingyuan Chen|
|10:00|8+2|Shared Infrastructure: David Moulton|
|10:10|20|Group discussion and activities|
|10:30|30|Coffee Break|
|| |**Flash Talks** <br>Early-career and mid-career staff, and postdocs present highlights of their recent work <br>*(4 minutes for the presentation and 1 minute for questions and transition)*|
|11:00|4+1|Zhi Li, Integrating ELM-BGC Carbon Cycling with ATS-PFLOTRAN Hydro-Biogeochemical Modeling in a Wildfire-Impacted Pacific Northwest Watershed|
|11:05||Andrew Graus, ATS-EcoSIM Snow Model Progress|
|11:10||Maria Contreras-Vargas, Why are our coastal forests dying? Explaining tree mortality using remote sensing detection and integrated hydrology simulations.|
|11:15||Tasneem Ahmadullah, Understanding Water Column Respiration Kinetics Using Substrate Explicit Thermodynamic Model|
|11:20||Jesus Gómez-Vélez, Exploring the Influence of Hyporheic Exchange on Stream Oxygen Dynamics|
|11:25||Saubhagya Rathore, Incorporating Water Management Infrastructure into the ATS Integrated Hydrology Model.|
|11:30||Daniil Svyatsky, Simulation of below ground drainage network for mitigation of urban flooding|
|11:35||Georgios Artavanis, ParFlow, SubsetTools, HydroData and integration with Watershed Workflow.|
|11:40||Erica Woodburn, Topographic controls on mountainous hydrology with ParFlow-ELM-FATES|
|11:45||Rich Fiorella, Toward a parallelized coupling between ATS and ELM|
|12:00|60|**Working Lunch**|
|| |**Hands-On:** Adding Transport to Integrated Hydrology in ATS<br>**Lead:** Phong Le<br>**Duration:** 3 hours|
|1:00|120|{::nomarkdown}<ul><li>Understand the basics of the transport process kernel (PK) in Amanzi-ATS; </li><li> Develop workflows that couple transport PK with hydrology PK; </li><li> Visualize and analyze Amanzi-ATS model output.</li></ul>{:/}|
|3:00|30|Coffee Break|
|3:30|30|Continue transport in ATS hands-on session|
|| | **Visualization Part I** |
|4:00|60|Review Gallery Examples and Collect/rank Questions.|
|| | **Adjourn** |

<br><br>

#### Day 2: Friday November 15, 2024 9:00 AM-5:00PM (MST)

|Wall Clock (PT) |  Elapsed Time (min)    | Talks/Activity
|:---------------|:-----------------------|:-----------------------------------------------------|
|8:00|30|Coffee and Continental Breakfast|
|| | **Group Discussion** |
|8:30|30|{::nomarkdown}<ul><li>Feedback on Day 1</li><li> What’s next, what do you need, what’s slowing you down?</li></ul>{:/}|
|| |**Hands-On:**  Mixed-Element meshes in Watershed Workflow with ATS<br>**Lead:** Saubhagya Rathore<br>**Duration:** 3 hours|
|9:00|90|**Introduction:** (10 minutes){::nomarkdown}<ul><li>Outline of the workshop</li><li>Overview of the meshing workflow</li></ul>{:/}**Module 1: Exploring Key Conceptual Objects:** (20 minutes){::nomarkdown}<ul><li>Dive into WW components like RiverTree and SplitHucs critical to mixed-polyhedral meshing, understanding their roles in meshing.</li><li>Understand basics of manipulating WW objects.</li></ul>{:/}**Module 2: Simplify and Redensify** (30 minutes){::nomarkdown}<ul><li> Explore different simplify and redensify methods including variable quad lengths.</li><li> Manipulate reaches to identify and resolve data inconsistencies and errors like dual intersection problem</li></ul>{:/}**Module 3: Mesh Generation** (30 minutes){::nomarkdown}<ul><li>Leverage various refinement methods and constraints during triangulation to generate a high-quality mesh.</li><li>Provide river widths using multiple methods.</li><li>Meshing troubleshooting</li></ul>{:/}|
|10:30|30|**Coffee Break**|
|11:00|90|**Continue mixed-element meshes**<br><br>**Module 4: Labeled Sets**(10 minutes){::nomarkdown}<ul><li>Define labeled sets in the river mesh at different levels of granularity (e.g., stream network, stream order, individual reaches).</li></ul>{:/}**Module 5: Hydrologic Conditioning** (20 minutes){::nomarkdown}<ul><li>Condition the river mesh using different methods.</li><li> Provide supplemental depth to the stream mesh.</li></ul>{:/}**Module 6: Office Hours** (1 hour){::nomarkdown}<ul><li>Attendees work on their watersheds and troubleshoot issues with the help of the facilitators and fellow attendees.</li><li>Discussions and feedback on the workshop.</li></ul>{:/}|
|12:30|30|**Working Lunch**| 
|| |**Evaluators in ATS**<br>**Lead:** Ethan Coon|
|1:00|60|An overview of evaluator design and their use in observations and visualization.  Examples of existing evaluators (e.g., depth to water table), and creating a custom evaluator.|
|| |**Visualization Part 2**|
|2:00|60|Group discussion and followup on key challenges and what next?|
|3:00|30|**Coffee Break**|
|3:30|60|Optional Informal Breakout discussions, topics could include building ATS with custom TPLs (e.g., PFLOTRAN), spatially dependent …|
|| |**Adjourn**|

