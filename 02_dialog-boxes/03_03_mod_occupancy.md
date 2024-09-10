---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: '1.16'
    jupytext_version: 1.16.1
kernelspec:
  display_name: Python 3
  language: python
  name: python3
editor_options: 
  markdown: 
    wrap: none
--- 
<style>
  h1 {
    font-size: 1.5rem;font-weight: bold;
  }
</style>
(i_mod_occupancy)=
# {{ name_mod_occupancy }}
:::::::::{div} full-width

::::::{dropdown} Assumptions, Pros, Cons
:::::{grid}

::::{grid-item-card} Assumptions
- {{ mod_occupancy_assump_01 }}
- {{ mod_occupancy_assump_02 }}
- {{ mod_occupancy_assump_03 }}
- {{ mod_occupancy_assump_04 }}
- {{ mod_occupancy_assump_05 }}
::::
::::{grid-item-card} Pros
- {{ mod_occupancy_pro_01 }}
- {{ mod_occupancy_pro_02 }}
- {{ mod_occupancy_pro_03 }}
- {{ mod_occupancy_pro_04 }}
- {{ mod_occupancy_pro_05 }}
::::
::::{grid-item-card} Cons
- {{ mod_occupancy_con_01 }}
- {{ mod_occupancy_con_02 }}
::::
:::::
::::::

:::::::{tab-set}

::::::{tab-item} Overview

**{{ term_mod_occupancy }}**: {{ term_def_mod_occupancy }}
<br>Add some info here

::::::

::::::{tab-item} Advanced
Occupancy models describe spatial patterns of animal occurrence ({{ ref_intext_sollmann_et_al_2018 }}) and have been proposed as a proxy for abundance ({{ ref_intext_noon_et_al_2012 }}). They ask: what proportion of a study area is inhabited by a population – that is, at how many camera sites do one or more individuals of a species occur ({{ ref_intext_mackenzie_et_al_2017 }})? The basic equation for occupancy is: <br><br>

```{figure} ../03_images/03_image_files/clarke_et_al_2023_eqn_occupancy1.png
:align: center
```

where *𝜓* is the probability a site is occupied, *𝑥̂* is the estimated number of occupied sites (i.e., the count of sites where animals were detected, corrected for detection probability) and 𝑠 is the total number of sites surveyed ({{ ref_intext_mackenzie_et_al_2017 }}). Unlike simple measures of presence-absence, occupancy models account for imperfect detection ({{ ref_intext_sollmann_et_al_2018 }}). They attempt to differentiate between absence – animals truly not present – and nondetection – animals present but not detected – by repeatedly sampling sites over time. The central assumption of basic occupancy models is that repeated samples occur during a period in which the site is closed to changes in occupancy (i.e., occupancy status – present or absent – does not change during the sampling period). Thus if a species is detected during one of three sampling occasions, it is assumed that it was present during all three occasions but undetected during two. <br>
<br>
In theory, occupancy and abundance share a predictable relationship. As population size increases, the number of sites occupied by members of that population should also increase (until all sites are occupied); likewise, a decrease in population size should lead to a decrease in the number of sites used ({{ ref_intext_gaston_et_al_2000 }};  {{ ref_intext_royle_dorazio_2008 }}). This is called an occupancy-abundance relationship, and – because of it – occupancy can be used as an index of abundance. <br>
<br>
Advantages of occupancy as an index of abundance include: <br>
<br>
- Occupancy studies may be easier to implement than some abundance or density estimators ({{ ref_intext_noon_et_al_2012 }};  {{ ref_intext_sollmann_et_al_2018 }}). 
- Occupancy-abundance relationships appear to be robust to territoriality, group travelling behaviour and other biological traits (
 {{ ref_intext_steenweg_et_al_2018 }}). 
- Occupancy can be modelled as a function of site- and sampling-specific covariates to better understand which factors predict animal occurrence ({{ ref_intext_sollmann_et_al_2018 }}). <br>
<br>
However, many researchers have cautioned against the use occupancy as an index. As with relative abundance (RA; see above), there is no consistent, long-term relationship between occupancy and abundance ({{ ref_intext_efford_dawson_2012 }}). Occupancy can change with abundance, but also with survey duration, species home range size, animal movement, etc., muddling occupancy-abundance relationships and thus inferences about population size ({{ ref_intext_neilson_et_al_2018 }};  {{ ref_intext_steenweg_et_al_2018 }}). While occupancy is a powerful stand-alone metric, Sollmann (2018) says it should not be “misinterpreted” as an index of abundance. <br>
<br>
Despite its widespread use, occupancy may be particularly problematic for camera trap studies due to the violation of the closure assumption. Burton et al. (2015) highlighted that many camera trap studies using occupancy do not explicitly define the “site,” although is often implicitly given as some larger area around a camera trap. Since camera trap studies typically target mammal species with relatively large home ranges, the site closure assumption is almost certainly violated in most cases. Many camera trappers therefore assume that “occupancy” is in fact “use” of a site (i.e., the site is not closed), and that detection probability also includes availability for detection. Mackenzie et al. (2017) suggested that estimates should be unbiased if movements in and out of a site are random, but this assumption is rarely tested. And where occupancy estimates have been tested using realistic mammal movements, they have generally performed poorly ({{ ref_intext_neilson_et_al_2018 }};  {{ ref_intext_stewart_et_al_2018 }}).
::::::

::::::{tab-item} Visual resources
:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_murray_et_al_2021 }}
```{figure} ../03_images/03_image_files/murray_et_al_2021.jpg
:height: 300px
:align: center
```
<font size="2">**Murray et al. (2021) - Fig. 1.** Schematic of our multi- state occupancy model to estimate the occurrence of coyotes and mange. We used images of coyotes collected along transects following an urban gradient in the Chicago metro area in a standard single-species multi-season model with a stacked design. Following the coyote occupancy model, our mange model estimates the distribution of coyote with sarcoptic mange conditional on the distribution of coyote, mangy or otherwise, using by-image variation in the presence of mange signs and the quality of the image</font>
::::

::::{grid-item-card} {{ ref_intext_southwell_et_al_2019 }}
```{figure} ../03_images/03_image_files/southwell_et_al_2019_fig1_clipped.png 
:width: 300px
:align: center
```
<font size="2">**Southwell et al. (2019) - Fig. 1.** Structure of the spatially explicit power analysis framework for multiple species in dynamic landscapes.</font>
::::

::::{grid-item-card} {{ ref_intext_clarke_et_al_2023 }}
```{figure} ../03_images/03_image_files/clarke_et_al_2023_eqn_occupancy1.png 
:width: 300px
:align: center
```
<font size="2">   </font>
::::

:::::

:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_chatterjee_et_al_2021 }}
```{figure} ../03_images/03_image_files/chatterjee_et_al_2021_table2_clipped.png 
:width: 300px
:align: center
```
<font size="2">**Chatterjee et al. (2021) - Table 2.** Broad classifications of mammals based on occupancy and detection probabilities.</font>
::::

::::{grid-item-card} {{ ref_intext_figure5_ref_id }}
```{figure} ../03_images/03_image_files/figure5_filename.png 
:width: 300px
:align: center
```
<font size="2">figure5_caption</font>
::::

::::{grid-item-card} {{ ref_intext_figure6_ref_id }}
```{figure} ../03_images/03_image_files/figure6_filename.png
:width: 300px
:align: center
```
<font size="2">figure6_caption</font>
::::
:::::

:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_figure7_ref_id }}
```{figure} ../03_images/03_image_files/figure7_filename.png
:width: 300px
:align: center
```
<font size="2">figure7_caption</font>
::::

::::{grid-item-card} {{ ref_intext_figure8_ref_id }}
```{figure} ../03_images/03_image_files/figure8_filename.png
:width: 300px
:align: center
```
<font size="2">figure8_caption</font>
::::

::::{grid-item-card} {{ ref_intext_figure9_ref_id }}
```{figure} ../03_images/03_image_files/figure9_filename.png
:width: 300px
:align: center
```
<font size="2">figure9_caption</font>
::::
:::::

:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_figure10_ref_id }}
```{figure} ../03_images/03_image_files/figure10_filename.png
:width: 300px
:align: center
```
<font size="2">figure10_caption</font>
::::

::::{grid-item-card} {{ ref_intext_figure11_ref_id }}
```{figure} ../03_images/03_image_files/figure11_filename.png
:width: 300px
:align: center
```
<font size="2">figure11_caption</font>
::::

::::{grid-item-card} {{ ref_intext_figure12_ref_id }}
```{figure} ../03_images/03_image_files/figure12_filename.png
:width: 300px
:align: center
```
<font size="2">figure12_caption</font>
::::
:::::

:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_vid1_ref_id }}
<iframe 
    width="300"
    height="200"
    src="https://www.youtube.com/embed/n21Ugw0lYcY?si=RUCD7WjcLPJdHR00"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

<font size="2">Occupancy Modeling Video 1 -- Sampling Techniques for Mammals</font>
::::

::::{grid-item-card} {{ ref_intext_vid2_ref_id }} 
<iframe 
    width="300"
    height="200"
    src="https://www.youtube.com/embed/u--F8_oRpVU?si=XzL4GMaQmvlL-noj"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

<font size="2">Occupancy Modeling Video 2 -- Introductory Statistical Review</font>
::::

::::{grid-item-card} {{ ref_intext_vid3_ref_id }}
<iframe 
    width="300"
    height="200"
    src="https://www.youtube.com/embed/-F-txltI_iA?si=C8R-MQ3pKcskOcQt"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

<font size="2">Occupancy Modeling Video 3 -- What are Occupancy Models and What are the Applications?</font>
::::
:::::

:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_vid4_ref_id }} 

<iframe 
    width="300"
    height="200"
    src="https://www.youtube.com/embed/DVo4KVMPnWg?si=m_umrFr9FjNb9KlK"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

<font size="2">Occupancy Modeling Video 4 -- How to Run and Interpret the Models in PRESENCE</font>
::::

::::{grid-item-card} {{ ref_intext_vid5_ref_id }}

<iframe 
    width="300"
    height="200"
    src="https://www.youtube.com/embed/Sp4kb4_TiBA?si=HfYJ3DgqOJfiJ4Z4l"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

<font size="2">Occupancy modelling - more than species presence/absence! (Darryl MacKenzie)</font>
::::

::::{grid-item-card} {{ ref_intext_vid6_ref_id }}
<iframe 
    width="300"
    height="200"
    src="vid6_url"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

<font size="2">vid6_caption</font>
::::

:::::

::::::


::::::{tab-item} Shiny apps/Widgets
Check back in the future!
<!--
:::::{card}
**shiny_name **

shiny_caption

<iframe 
    width="100%"
    height="900"
    src="shiny_url"
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>
:::::-->
<!--ALT-->
<!--
:::::{card}
::::{dropdown} shiny_name 

shiny_caption

<iframe 
    width="100%"
    height="900"
    src="shiny_url"
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

::::

::::{dropdown} shiny_name2

shiny_caption2

<iframe shiny_url2
    width="100%"
    height="900"
    src=""
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>
::::
:::::-->
::::::

::::::{tab-item} Analytical tools & resources
| Type | Name | Note | URL |Reference |
|:------------|:---------------------------------------|:----------------------------------------------------------------|:----------------------------------------------------------------|:----------------------------------------------------------------|
| rJAGS/R code | mfidino/multi-state-occupancy-models | Mason Fidino's GitHub | <https://github.com/mfidino/multi-state-occupancy-models> | {{ ref_bib_resource1_ref_id }} |
| JAGS/R code | mfidino/integrated-occupancy-model” | Mason Fidino's GitHub | <https://github.com/mfidino/integrated-occupancy-models>l | {{ ref_bib_resource2_ref_id }} |
| JAGS code | mfidino/auto-logistic-occupancy | Mason Fidino's GitHub | <https://github.com/mfidino/auto-logistic-occupancy> | {{ ref_bib_resource3_ref_id }} |
| R package | R package - “autoOcc” | An R package for fitting autologistic occupancy models | <https://github.com/mfidino/autoOcc> | {{ ref_bib_resource4_ref_id }} |
| R code | mfidino/periodicity | Using Fourier series to predict periodic patterns in dynamic occupancy models | <https://github.com/mfidino/periodicity> | {{ ref_bib_resource5_ref_id }} |
| R shiny | Simulated Occupancy Model Shiny App | could incorporate mammal data fairly easily to provide information on occupancy and detection probability | <https://drive.google.com/drive/folders/1B-h1yGYgfxz5ki-O4Q8R_-1Ts__SnpIM> | {{ ref_bib_resource6_ref_id }} |
| R code/Tutorial | “An Introduction to Camera Trap Data Management and Analysis in R > Chapter 11 Occupancy” |     | <https://bookdown.org/c_w_beirne/wildCo-Data-Analysis/occupancy.html> | {{ ref_bib_resource7_ref_id }} |
| Program  | “PRESENCE” | "Relatively simple, but comprehensive, software dedicated to occupancy estimation. Linux version available. Can also be used for occupancy-based species richness estimation." (Wearn & Glover-Kapfer, 2017) | **Software**: <www.mbr-pwrc.usgs.gov/ software/presence.html>;<br>**Help forum**: <www.phidot.org> | {{ ref_bib_resource8_ref_id}} |
| R package | R package - “RPresence” | “The R counterpart to Presence. Cross-platform (Windows, Mac and Linux)." (Wearn & Glover-Kapfer, 2017) | <https://www.mbr-pwrc.usgs.gov/software/presence.shtml> | {{ ref_bib_resource9_ref_id }} |
| R package | R package "unmarked” | "Implements a wide variety of occupancy and count-based abundance models (the latter are mostly not appropriate for camera-trapping). Actively being developed and supported by a community of users. Cross-platform (Windows, Mac and Linux)." (Wearn & Glover-Kapfer, 2017) | <https://cran.r-project.org/web/packages/unmarked/index.html>;<br><https://groups.google.com/g/unmarked> | {{ ref_bib_resource10_ref_id }} |
| R code/Tutorial | “Multi-season Occupancy Models” | Mason Fidino's GitHub | <https://darinjmcneil.weebly.com/multi-season-occupancy.html> | {{ ref_bib_resource11_ref_id }} |
| R package | R package for analyzing wildlife data with detection error | resource12_note | resource12_url | {{ ref_bib_resource12_ref_id }} |
::::::

::::::{tab-item} References
<font size="3">
{{ ref_bib_burton_et_al_2015 }}

 {{ ref_bib_efford & dawson_2012 }}

 {{ ref_bib_gaston_et_al_2000 }}

 {{ ref_bib_mackenzie_et_al_2017 }}

 {{ ref_bib_murray_et_al_2021 }}

 {{ ref_bib_neilson_et_al_2018 }}

 {{ ref_bib_noon_et_al_2012 }}

 {{ ref_bib_royle_dorazio_2008 }}

 {{ ref_bib_sollmann_et_al_2018 }}

 {{ ref_bib_southwell_et_al_2019 }}

 {{ ref_bib_steenweg_et_al_2018 }}

 {{ ref_bib_stewart_et_al_2018 }}
</font>	
::::::

:::::::

:::::::::