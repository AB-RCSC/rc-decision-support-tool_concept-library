---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.17.2 <!--0.13-->
    jupytext_version: 6.5.4 <!-- 1.16.4-->
kernelspec:
  display_name: Python 3
  language: python
  name: python3
editor_options: 
  markdown: 
  wrap: none
---
(i_mod_scr_secr)=
# {{ name_mod_scr_secr }}

**{{ term_mod_scr_secr }}**: {{ term_def_mod_scr_secr }}

::::::{dropdown} Assumptions, Pros, Cons
:::::{grid}

::::{grid-item-card} Assumptions
- {{ mod_scr_secr_assump_01 }}
- {{ mod_scr_secr_assump_02 }}
- {{ mod_scr_secr_assump_03 }}
- {{ mod_scr_secr_assump_04 }}
- {{ mod_scr_secr_assump_05 }}
- {{ mod_scr_secr_assump_06 }}
- {{ mod_scr_secr_assump_07 }}
- {{ mod_scr_secr_assump_08 }}
- {{ mod_scr_secr_assump_09 }}
- {{ mod_scr_secr_assump_10 }}
- {{ mod_scr_secr_assump_11 }}
- {{ mod_scr_secr_assump_12 }}
- {{ mod_scr_secr_assump_13 }}
- {{ mod_scr_secr_assump_14 }}
::::
::::{grid-item-card} Pros
- {{ mod_scr_secr_pro_01 }}
- {{ mod_scr_secr_pro_02 }}
- {{ mod_scr_secr_pro_03 }}
- {{ mod_scr_secr_pro_04 }}
- {{ mod_scr_secr_pro_05 }}
- {{ mod_scr_secr_pro_06 }}
- {{ mod_scr_secr_pro_07 }}
- {{ mod_scr_secr_pro_08 }}
- {{ mod_scr_secr_pro_09 }}
::::
::::{grid-item-card} Cons
- {{ mod_scr_secr_con_01 }}
- {{ mod_scr_secr_con_02 }}
- {{ mod_scr_secr_con_03 }}
- {{ mod_scr_secr_con_04 }}
- {{ mod_scr_secr_con_05 }}
- {{ mod_scr_secr_con_06 }}
- {{ mod_scr_secr_con_07 }}
::::
:::::
::::::

:::::::{tab-set}

::::::{tab-item} Overview
Spatial capture-recapture (SCR) models are used to estimate animal density. They use a combination of information 

SCR models rely on data in which individual animals are observed on multiple occasions, either being captured, marked and released, or individuals being identified on multiple occasions via specific diagnostic features (e.g., leopard print patterns, dolphin fin markings, etc.).


::::::

::::::{tab-item} Advanced:::{note}
**This content was adapted from**: The Density Handbook, "[Using Camera Traps to Estimate Medium and Large Mammal Density: Comparison of Methods and Recommendations for Wildlife Managers](https://www.researchgate.net/publication/368601884_Using_Camera_Traps_to_Estimate_Medium_and_Large_Mammal_Density_Comparison_of_Methods_and_Recommendations_for_Wildlife_Managers)" (Clarke et al., 2024)
:::

Spatial capture-recapture (SCR) models can be applied to any survey method where animals are individually identifiable and trap locations are known: live trapping and tagging, DNA sampling, camera trapping, etc. ({{ ref_intext_royle_et_al_2014 }}). Here, we will discuss camera trap SCR. 

SCR models break populations down into the activity, or home range, centres of individual animals. Let us first imagine we know the number and location of all individuals’ activity centres in a population. If we did, we could easily estimate density:

```{figure} ../03_images/03_image_files/clarke_et_al_2023_eqn_scr1.png
:width: 80px
:align: center
```  

assuming each member of the population has an activity centre, and so the number of activity centres is equivalent to population size; and since the area encompassing all activity centres is the total area sampled by the camera array (i.e., the sampling frame; Sollmann, 2018). In reality, we do not know the number and location of activity centres – indeed, the estimated number and location of activity centres is the SCR model output.

To resolve the number and location of activity centres – and thus estimate density – SCR models combine information about 1) where animals are detected in space (using an observation model) and 2) how animals are distributed in space (using a spatial process model; Figure 4; {{ ref_intext_royle_2016 }}).

```{figure} ../03_images/03_image_files/clarke_et_al_2023_fig4_clipped.png
:width: 80px
:align: center
```  

**Clarke et al., 2023 – Fig. 4** SCR models are made up of two sub-models: an observation model, which describes where individual animals are detected (i.e., their detection histories); and a spatial process model, which describes how animals’ activity centres are distributed.

<br>
The observation model uses the record of where each individual was detected (i.e., individuals’ detection histories) to infer the location of each individual’s respective activity centre (Figure 5A; {{ ref_intext_chandler_royle_2013 }}; {{ ref_intext_royle_2016 }}). It relies on the inverse relationship between detection probability and cameratrap-to-activity-centre distance: as the distance between a camera and an individual’s activity centre increases, the likelihood that individual will be detected there decreases (Figure 5B; {{ ref_intext_royle_et_al_2014 }}). So, animals will be detected most frequently at camera traps near their activity centres, and least frequently (or not at all) at camera traps far from their activity centres. Because the locations of activity centres are unknown, we use a spatial process model to approximate their distribution. Point-process models are a common choice ({{ ref_intext_royle_2016 }}). A point-process model is a random pattern of points in space ({{ ref_intext_baddeley_nd }}); it can be homogenous (completely spatially random) or inhomogeneous (the density of points depends on landscape/habitat covariates; ({{ ref_intext_royle_2016 }}).

Taken together: SCR essentially “downscales” density – a population-level estimator – to the level of the individual. The model asks: where does each animal live ({{ ref_intext_royle_2016 }})? Although the location of animals’ activity centres is not known, we can use information about where individuals are captured (detection histories) and how activity centres are distributed in space (point-process model) to infer where they live, and thus estimate density ({{ ref_intext_royle_2016 }}). SCR can be implemented using many statistical frameworks, including full likelihood estimation ({{ ref_intext_borchers_efford_2008 }}), dataaugmented maximum likelihood estimation ({{ ref_intext_royle_et_al_2014 }}), and data-augmented Bayesian estimation ({{ ref_intext_royle_young_2008 }}; {{ ref_intext_morin_et_al_2022 }}).

When deploying cameras for SCR analysis, practitioners must balance the area covered by the camera array with trap spacing to maximize both the number of unique individuals captured and the number of spatial recaptures of each individual. A larger sampling area will yield a higher count of unique individuals; closely-spaced traps will yield a higher number of spatial recaptures (i.e., detections of the same individual at different camera traps; {{ ref_intext_royle_et_al_2014 }}). Both are important for SCR density estimation. Cameras should also be deployed across habitat types with different levels of use ({{ ref_intext_morin_et_al_2022 }}; {{ ref_intext_sun_et_al_2014 }}). Grid and clustered sampling designs can help meet all these needs ({{ ref_intext_clarke_2019 }}; {{ ref_intext_sun_et_al_2014 }}). Note that optimal camera trap placement and spacing will change with focal species, landscape and project limitations.

See Clark (2019), Dupont et al., (2021), Fleming et al., (2021), McFarlane et al., (2020), Nawaz et al., (2021), Romairone et al., 2018, Sollmann et al., (2012) and Sun et al., (2014) for more detailed explorations of SCR study design.

```{figure} ../03_images/03_image_files/clarke_et_al_2023_fig5_clipped.png
:width: 80px
:align: center
``` 

**Clarke et al. (2023) – Fig. 5** Adapted from Morin et al., (2022) and Royle et al., (2014). A) A diagram of how the individual activity centres (circles) that make up a population might overlap with a camera array (grey crosses). The red circle highlights an example individual’s activity centre. The red arrows point towards camera stations where the red individual was detected; the numbers beside the camera stations show how many times the red individual was detected at each station. Note, the number and location of individual’s activity centres is not known, but rather inferred from the spatial pattern of detections (i.e., the number of detections of each individual at camera stations of known location). B) An example graph showing how the probability the red individual is detected at a camera station decreases with distance from its activity centre. This is reflected in A); as the distance between the red individual’s activity centre and a camera station increases, the number of detections dwindles. σ is the spatial scale parameter; it describes how detection probability decreases with increasing distance.

Another aspect of sampling design practitioners must consider is the number and configuration of cameras deployed at a station to identify animals to the individual. Left and right flanks may need to be photographed simultaneously, for example, to avoid assigning different identities to each side  ({{ ref_intext_augustine_et_al_2018 }}); as another example, chest markings may need to be photographed from multiple angles at bait stations to be able to resolve identity ({{ ref_intext_proctor_et_al_2022 }}).
::::::

::::::{tab-item} Visual resources
:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_clarke_et_al_2023 }}
```{figure} ../03_images/03_image_files/clarke_et_al_2023_eqn_scr1.png
:class: img_grid
```
**Efford (2011) - Figure 1**: Hypothetical Poisson distribution of range centres near an array of detectors. We estimate the intensity (density) of this distribution
::::

::::{grid-item-card} {{ ref_intext_clarke_et_al_2023 }}
```{figure} ../03_images/03_image_files/clarke_et_al_2023_fig4_clipped.png 
:class: img_grid
```
**Clarke et al. (2023) – Fig. 4.** SCR models are made up of two sub-models: an observation model, which describes where individual animals are detected (i.e., their detection histories); and a spatial process model, which describes how animals’ activity centres are distributed.
::::

::::{grid-item-card} {{ ref_intext_clarke_et_al_2023  }}
```{figure} ../03_images/03_image_files/clarke_et_al_2023_fig4_clipped.png 
:class: img_grid
```
**Clarke et al. (2023) - Fig. 5** Adapted from Morin et al., (2022) and Royle et al., (2014). A) A diagram of how the individual activity centres (circles) that make up a population might overlap with a camera array (grey crosses). 
:::{dropdown}
The red circle highlights an example individual’s activity centre. The red arrows point towards camera stations where the red individual was detected; the numbers beside the camera stations show how many times the red individual was detected at each station. Note, the number and location of individual’s activity centres is not known, but rather inferred from the spatial pattern of detections (i.e., the number of detections of each individual at camera stations of known location). B) An example graph showing how the probability the red individual is detected at a camera station decreases with distance from its activity centre. This is reflected in A); as the distance between the red individual’s activity centre and a camera station increases, the number of detections dwindles. σ is the spatial scale parameter; it describes how detection probability decreases with increasing distance.
:::
::::

:::::

:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_efford_2011 }}
```{figure} ../03_images/03_image_files/efford_2011_fig1.png 
:class: img_grid
```
figure4_caption
::::

::::{grid-item-card} {{ ref_intext_efford_2023 }}
```{figure} ../03_images/03_image_files/efford_2023_fig1.png 
:class: img_grid
```
figure5_caption
::::

::::{grid-item-card} {{ ref_intext_figure6_ref_id }}
```{figure} ../03_images/03_image_files/secr_creemmural_org_secr.png
:class: img_grid
```
figure6_caption
::::
:::::

:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_vid1_ref_id }}
<iframe 
    width="100%"
    height="300"
    src="https://www.youtube.com/embed/4HKFimATq9E"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

J. Andrew Royle,"Spatial Capture-Recapture Modelling" ✨
::::

::::{grid-item-card} {{ ref_intext_vid2_ref_id }} 
<iframe 
    width="100%"
    height="300"
    src="https://www.youtube.com/embed/4HKFimATq9E"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

PAWS: Spatial Capture Recapture Data Analysis Part 1 ✨
::::

::::{grid-item-card} {{ ref_intext_vid3_ref_id }}
<iframe 
    width="100%"
    height="300"
    src="https://www.youtube.com/embed/IHVez1a_hqg"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

PAWS: Spatial Capture Recapture Data Analysis Part 2✨
::::
:::::

:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_royle_2020 }} 

<iframe 
    width="100%"
    height="300"
    src="https://www.youtube.com/embed/yRRDi07FtPg?si=vmGQslB9Wv9MnkYC"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

Introduction to Spatial Capture-Recapture with the oSCR Package 
::::

:::::

::::::

::::::{tab-item} Shiny apps/Widgets
:::::{card} Secrdesign app 1.5 {{ ref_bib_efford_boulanger_2019 }}
<iframe 
    width="100%"
    height="900"
    src="https://www.stats.otago.ac.nz/secrdesignapp"
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>
::::

::::::

::::::{tab-item} Analytical tools & resources
| Type | Name | Note | URL |Reference |
|:----------------|:-------------------------------|:----------------------------------------------------------------|:----------------------|:----------------------------------------|
| Article | Fast Evaluation of Study Designs for Spatially Explicit Capture–Recapture | resource1_note | <https://doi.org/10.1111/2041-210X.13239> | {{ ref_bib_efford_boulanger_2019 }} |
| App/Program | Program SPACECAP | Removed from cran | <https://cran.r-project.org/web/packages/SPACECAP/index.html> | {{ ref_bib_gopalaswamy_et_al_2021 }} |
| R function | R package “oSCR”- “sim.SCR” function | resource3_note | <https://onlinelibrary.wiley.com/doi/10.1111/ecog.04551> | {{ ref_bib_sutherland_et_al_2018 }} |
| R package | R package “secr” | resource4_note | Package info: <https://cran.r-project.org/web/packages/secr/index.html><br>Help forum: <www.phidot.org> | {{ ref_bib_resource4_ref_id }} |
| App/Program | DENSITY | resource5_note | <https://science.uct.ac.za/seec/stats-toolbox-seminars-spatial-and-species-distribution-toolboxes/spatial-capture-recapture-scr-modelling> | {{ ref_bib_resource5_ref_id }} |
| Powerpoint slides | SEEC Toolbox seminars - Spatial Capture-Recapture (SCR) models | Additional information can be accessed [here](https://science.uct.ac.za/seec/stats-toolbox-seminars-spatial-and-species-distribution-toolboxes/spatial-capture-recapture-scr-modelling) | <https://science.uct.ac.za/sites/default/files/content_migration/science_uct_ac_za/708/files/SEEC%2520Stats%2520Toolbox%2520-%2520Spatial%2520capture%2520recapture%2520slides.pdf> | {{ ref_bib_u_capetown_2024 }} |
| R package  | Package “oSCR” | resource7_note | resource7_url | {{ ref_bib_resource7_ref_id }} |
| Tutorial | 2. Getting started with oSCR | resource8_note | <https://sites.google.com/site/spatialcapturerecapture/oscr-package/2-getting-started-with-oscr>| {{ ref_bib_resource8_ref_id}} |
::::::

::::::{tab-item} References
{{ ref_bib_augustine_et_al_2018 }}

{{ ref_bib_baddeley_nd }}

{{ ref_bib_borchers_efford_2008 }}

{{ ref_bib_chandler_royle_2013 }}

{{ ref_bib_clarke_2019 }}

{{ ref_bib_clarke_et_al_2023 }}

{{ ref_bib_dupont_et_al_2021 }}

{{ ref_bib_efford_boulanger_2019 }}

{{ ref_bib_efford_2024 }}

{{ ref_bib_efford_2011 }}

{{ ref_bib_efford_2023 }}

{{ ref_bib_fleming_et_al_2021 }}

{{ ref_bib_gopalaswamy_et_al_2021 }}

{{ ref_bib_proctor_et_al_2022 }}

{{ ref_bib_mcfarlane_et_al_2020 }}

{{ ref_bib_morin_et_al_2022 }}

{{ ref_bib_nawaz_et_al_2021 }}

{{ ref_bib_sollmann_et_al_2012 }}

{{ ref_bib_sun_et_al_2014 }}

{{ ref_bib_romairone_et_al_2018 }}

{{ ref_bib_royle_et_al_2014 }}

{{ ref_bib_royle_2016 }}

{{ ref_bib_royle_2020 }}

{{ ref_bib_royle_young_2008 }}

{{ ref_bib_u_capetown_2024 }}	
::::::

:::::::