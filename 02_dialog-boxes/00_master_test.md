---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
kernelspec:
  display_name: Python 3
  language: python
  name: python3
editor_options:
  markdown:
    wrap: none
---
# master test
::::::::{hint}
```{admonition} See also
:class: sidebar tip
{{ link_bdg_sp_asymptote }}
```

**{{ name_mod_scr_secr }}**: {{ def_mod_scr_secr }}

replace me with text

{{ rtxt_ahumada_et_al_2011 }}

::::::::

```{include} pro_con_assump/mod_scr_secr_apc.md
```

::::::::{tab-set}

:::::::{tab-item} Overview
```{include} include/00_coming_soon.md
```
:::::::

:::::::{tab-item} In-depth
```{include} include/00_coming_soon.md
```
:::::::

:::::::{tab-item} Visual resources
::::::{grid} 3
:gutter: 3
:class-container: wrapper

:::::{grid-item-card} {{ rtxt_figure1_ref_id }}
<img src="../03_images/03_image_files/figure1_filename.png" class="img_grid"><br><br>figure1_caption
:::::

:::::{grid-item-card} {{ rtxt_figure2_ref_id }}
<img src="../03_images/03_image_files/figure2_filename.png" class="img_grid"><br><br>figure2_caption
:::::

:::::{grid-item-card} {{ rtxt_figure3_ref_id }}
<img src="../03_images/03_image_files/figure3_filename.png" class="img_grid"><br><br>figure3_caption
::::: 

:::::{grid-item-card} {{ rtxt_figure4_ref_id }}
<img src="../03_images/03_image_files/figure4_filename.png" class="img_grid"><br><br>figure4_caption
:::::

:::::{grid-item-card} {{ rtxt_figure5_ref_id }}
<img src="../03_images/03_image_files/figure5_filename.png" class="img_grid"><br><br>figure5_caption
:::::

:::::{grid-item-card} {{ rtxt_figure6_ref_id }}
<img src="../03_images/03_image_files/figure6_filename.png" class="img_grid"><br><br>figure6_caption
:::::

:::::{grid-item-card} {{ rtxt_vid1_ref_id }}
<div class="iframe-container-vid"><iframe class="iframe-responsive-vid" src="vid1_url"></iframe></div> 

vid1_caption
:::::

:::::{grid-item-card} {{ rtxt_vid2_ref_id }} 
<div class="iframe-container-vid"><iframe class="iframe-responsive-vid" src="vid2_url"></iframe></div> 

vid2_caption
:::::

:::::{grid-item-card} {{ rtxt_vid3_ref_id }}
<div class="iframe-container-vid"><iframe class="iframe-responsive-vid" src="vid3_url"></iframe></div> 

vid3_caption
:::::

:::::{grid-item-card} {{ rtxt_vid4_ref_id }} 
<div class="iframe-container-vid"><iframe class="iframe-responsive-vid" src="vid4_url"></iframe></div> 

vid4_caption
:::::

:::::{grid-item-card} {{ rtxt_vid5_ref_id }}
<div class="iframe-container-vid"><iframe class="iframe-responsive-vid" src="vid5_url"></iframe></div> 

vid5_caption
:::::

:::::{grid-item-card} {{ rtxt_vid6_ref_id }}
<div class="iframe-container-vid"><iframe class="iframe-responsive-vid" src="vid6_url"></iframe></div> 

vid6_caption
::::: 
::::::
:::::::

:::::::{tab-item} Shiny apps/Widgets
::::::{card}

:::::{dropdown} shiny_name
shiny_caption

<div class="iframe-container-shiny"><iframe class="iframe-responsive-shiny" src="shiny_url"></iframe></div> 
:::::

:::::{dropdown} shiny_name2 
shiny_caption2

<div class="iframe-container-shiny"><iframe class="iframe-responsive-shiny" src="shiny_url2"></iframe></div> 
:::::
::::::
:::::::

:::::::{tab-item} Analytical tools & Resources
| <div style="width:5%">Type</div> | <div style="width:15%">Name</div> | <div style="width:15%">Note</div> | <div style="width:10%">URL</div> | <div style="width:15%">Reference</div> |
|:----------------|:-------------------------------|:----------------------------------------------------------------|:----------------------|:----------------------------------------|
| rJAGS/R code | mfidino/multi-state-occupancy-models | | <https://github.com/mfidino/multi-state-occupancy-models> | {{ rbib_fidino_2021a }} |
| JAGS/R code | A gentle introduction to an integrated occupancy model that combines presence-only and detection/non-detection data, and how to fit it in JAGS; <br>integrated-occupancy-model" | | <https://masonfidino.com/bayesian_integrated_model/>;<br><https://github.com/mfidino/integrated-occupancy-model> | {{ rbib_fidino_2021b }}; <br>{{ rbib_fidino_2021c }} |
| JAGS code/Tutorial | So, you don't have enough data to fit a dynamic occupancy model? An introduction to auto-logistic occupancy models;<br>auto-logistic-occupancy |
| <https://masonfidino.com/autologistic_occupancy_model/>;<br><https://github.com/mfidino/auto-logistic-occupancy> | {{ rbib_fidino_2021d }}; <br>{{ rbib_fidino_2021e }} |
| R package | Package "autoOcc" | An R package for fitting autologistic occupancy models | <https://github.com/mfidino/autoOcc> | {{ rbib_fidino_2023 }} |
| R code | mfidino/periodicity | Using Fourier series to predict periodic patterns in dynamic occupancy models | <https://github.com/mfidino/periodicity> | {{ rbib_fidino_magle_2017 }} |
| Spreadsheet | OccPower.xlsx | Spreadsheet to compute power to detect difference in 2 independent occupancy estimates using asymptotic approximations described in Guillera-Arroita et. al. (2012). | [Download the XLS](../09_downloads/OccPower.xlsx) | {{ rbib_guillera_arroita_et_al_2012 }} |
| R code/Tutorial | "An Introduction to Camera Trap Data Management and Analysis in R > Chapter 11 Occupancy" | | <https://bookdown.org/c_w_beirne/wildCo-Data-Analysis/occupancy.html> | {{ rbib_wildco_lab_2021c }} |
| Program | Program "PRESENCE" | "Relatively simple, but comprehensive, software dedicated to occupancy estimation. Linux version available. Can also be used for occupancy-based species richness estimation." (Wearn & Glover-Kapfer, 2017) | **Software**: <www.mbr-pwrc.usgs.gov/software/presence.html>;<br>**Help forum**: <www.phidot.org> | {{ rbib_hines_2006 }} |
| R package | Package "RPresence" | "The R counterpart to Presence. Cross-platform (Windows, Mac and Linux)." (Wearn & Glover-Kapfer, 2017) | <https://www.mbr-pwrc.usgs.gov/software/presence.shtml> | {{ rbib_hines_2006 }} |
| R package | R package "unmarked" | "Implements a wide variety of occupancy and count-based abundance models (the latter are mostly not appropriate for camera-trapping). Actively being developed and supported by a community of users. Cross-platform (Windows, Mac and Linux)." (Wearn & Glover-Kapfer, 2017) | <https://cran.r-project.org/web/packages/unmarked/index.html>;<br><https://groups.google.com/d/forum/unmarked,>;<br>https://hmecology.github.io/unmarked> | {{ rbib_kellner_et_al_2023 }}; <br><br>{{ rbib_fiske_chandler_2011 }} |
| R code/Tutorial | Multi-season Occupancy Models | | <https://darinjmcneil.weebly.com/multi-season-occupancy.html> | {{ rbib_mcneil_nd }} |
| R package | Package "detect" | R package for analyzing wildlife data with detection error | <https://github.com/psolymos/detect> | {{ rbib_solymos_2023 }} |
| R code/Tutorial | Occupancy Modeling | Easy to follow explanation of occupancy models with accompanying tutorial and R code. | <https://kevintshoemaker.github.io/NRES-746/Occupancy.html> | {{ rbib_burne_golden_2021 }} |
| Tutorial | occupancyTuts: Occupancy modelling tutorials with RPresence | Occupancy modelling tutorials with RPresence | <https://doi.org/10.1111/2041-210X.14285> | {{ rbib_donovan_et_al_2024 }} |
| R code/Tutorial | Implicit dynamics occupancy models in R | Implicit dynamics occupancy models with the R package RPresence. These models estimate occupancy probability when it changes through time without estimating colonization and extinction parameters.<br>The code and sample data from this tutorial are available on GitHub; <https://github.com/jamesepaterson/occupancyworkshop>. | <https://jamesepaterson.github.io/jamespatersonblog/2024-06-02_implicitdynamicsoccupancy.html> | {{ rbib_paterson_2024 }} |
| Tutorial | Using the mgcvmgcv package to create a generalized additive occupancy model in R | | <https://masonfidino.com/generalized_additive_occupancy_model> | {{ rbib_fidino_2021f }} |
| R Shiny app | Bias in single-season occupancy models | "Compute the relative bias (in %) in the maximum-likelihood estimator of the occupancy probability ψ in a single-season (aka static) occupancy model with constant parameters fitted with the package 'unmarked'." | **Repo**: <https://github.com/oliviergimenez/bias_occupancy_flexdashboard><br>**App**: <https://ecologicalstatistics.shinyapps.io/bias_occupancy> | {{ rbib_gimenez_2020a }} |
| R code | Bias in occupancy estimate for a static model | "R code to calculate bias in occupancy estimate as a function of the detection probability given various levels of occupancy probability, various number of sites and surveys." | <https://github.com/oliviergimenez/bias_occupancy> | {{ rbib_gimenez_2020b }} |
| R code/ Presentation | Species Distribution Modelling | 'Vernon Visser provided a brief introduction to SDMs. Below you can replace the lecture slides and R script from this seminar. Provided in these materials is:<br>- A step-by-step guide to running your own SDM<br>- Suggestions for best practices<br>- References that can help provide more detail on the methods<br>-An R script that is annotated to make its understanding and adaptability easier' | <https://science.uct.ac.za/seec/stats-toolbox-seminars-spatial-and-species-distribution-toolboxes/species-distribution-modelling> | {{ rbib_u_capetown_2024 }} || Single-season occupancy models using a Bayesian approach |
:::::::

:::::::{tab-item} Analytical tools & Resources 2
<div class="proportional-table5cols">

| Type | Name | Note | URL | Reference |
|:----------------|:-------------------------------|:----------------------------------------------------------------|:----------------------|:----------------------------------------|
| rJAGS/R code | mfidino/multi-state-occupancy-models | | <https://github.com/mfidino/multi-state-occupancy-models> | {{ rbib_fidino_2021a }} |
| JAGS/R code | A gentle introduction to an integrated occupancy model that combines presence-only and detection/non-detection data, and how to fit it in JAGS; <br>integrated-occupancy-model" | | <https://masonfidino.com/bayesian_integrated_model/>;<br><https://github.com/mfidino/integrated-occupancy-model> | {{ rbib_fidino_2021b }}; <br><br>{{ rbib_fidino_2021c }} |
| R package | Package "autoOcc" | An R package for fitting autologistic occupancy models | <https://github.com/mfidino/autoOcc> | {{ rbib_fidino_2023 }} |
| R code | mfidino/periodicity | Using Fourier series to predict periodic patterns in dynamic occupancy models | <https://github.com/mfidino/periodicity> | {{ rbib_fidino_magle_2017 }} |
| Spreadsheet | OccPower.xlsx | Spreadsheet to compute power to detect difference in 2 independent occupancy estimates using asymptotic approximations described in Guillera-Arroita et. al. (2012). | [Download the XLS](../09_downloads/OccPower.xlsx) | {{ rbib_guillera_arroita_et_al_2012 }} |
| R code/Tutorial | "An Introduction to Camera Trap Data Management and Analysis in R > Chapter 11 Occupancy" | | <https://bookdown.org/c_w_beirne/wildCo-Data-Analysis/occupancy.html> | {{ rbib_wildco_lab_2021c }} |
| Program | Program "PRESENCE" | "Relatively simple, but comprehensive, software dedicated to occupancy estimation. Linux version available. Can also be used for occupancy-based species richness estimation." (Wearn & Glover-Kapfer, 2017) | **Software**: <www.mbr-pwrc.usgs.gov/software/presence.html>;<br>**Help forum**: <www.phidot.org> | {{ rbib_hines_2006 }} |
| R package | Package "RPresence" | "The R counterpart to Presence. Cross-platform (Windows, Mac and Linux)." (Wearn & Glover-Kapfer, 2017) | <https://www.mbr-pwrc.usgs.gov/software/presence.shtml> | {{ rbib_hines_2006 }} |
| R package | R package "unmarked" | "Implements a wide variety of occupancy and count-based abundance models (the latter are mostly not appropriate for camera-trapping). Actively being developed and supported by a community of users. Cross-platform (Windows, Mac and Linux)." (Wearn & Glover-Kapfer, 2017) | <https://cran.r-project.org/web/packages/unmarked/index.html>;<br><https://groups.google.com/d/forum/unmarked,>;<br>https://hmecology.github.io/unmarked> | {{ rbib_kellner_et_al_2023 }}; <br><br>{{ rbib_fiske_chandler_2011 }} |
| R code/Tutorial | Multi-season Occupancy Models | | <https://darinjmcneil.weebly.com/multi-season-occupancy.html> | {{ rbib_mcneil_nd }} |
| R package | Package "detect" | R package for analyzing wildlife data with detection error | <https://github.com/psolymos/detect> | {{ rbib_solymos_2023 }} |
| R code/Tutorial | Occupancy Modeling | Easy to follow explanation of occupancy models with accompanying tutorial and R code. | <https://kevintshoemaker.github.io/NRES-746/Occupancy.html> | {{ rbib_burne_golden_2021 }} |
| Tutorial | occupancyTuts: Occupancy modelling tutorials with RPresence | Occupancy modelling tutorials with RPresence | <https://doi.org/10.1111/2041-210X.14285> | {{ rbib_donovan_et_al_2024 }} |
| R code/Tutorial | Implicit dynamics occupancy models in R | Implicit dynamics occupancy models with the R package RPresence. These models estimate occupancy probability when it changes through time without estimating colonization and extinction parameters.<br>The code and sample data from this tutorial are available on GitHub; <https://github.com/jamesepaterson/occupancyworkshop>. | <https://jamesepaterson.github.io/jamespatersonblog/2024-06-02_implicitdynamicsoccupancy.html> | {{ rbib_paterson_2024 }} |
| Tutorial | Using the mgcvmgcv package to create a generalized additive occupancy model in R | | <https://masonfidino.com/generalized_additive_occupancy_model> | {{ rbib_fidino_2021f }} |
| R Shiny app | Bias in single-season occupancy models | "Compute the relative bias (in %) in the maximum-likelihood estimator of the occupancy probability ψ in a single-season (aka static) occupancy model with constant parameters fitted with the package 'unmarked'." | **Repo**: <https://github.com/oliviergimenez/bias_occupancy_flexdashboard><br>**App**: <https://ecologicalstatistics.shinyapps.io/bias_occupancy> | {{ rbib_gimenez_2020a }} |
| R code | Bias in occupancy estimate for a static model | "R code to calculate bias in occupancy estimate as a function of the detection probability given various levels of occupancy probability, various number of sites and surveys." | <https://github.com/oliviergimenez/bias_occupancy> | {{ rbib_gimenez_2020b }} |
| R code/ Presentation | Species Distribution Modelling | 'Vernon Visser provided a brief introduction to SDMs. Below you can replace the lecture slides and R script from this seminar. Provided in these materials is:<br>- A step-by-step guide to running your own SDM<br>- Suggestions for best practices<br>- References that can help provide more detail on the methods<br>-An R script that is annotated to make its understanding and adaptability easier' | <https://science.uct.ac.za/seec/stats-toolbox-seminars-spatial-and-species-distribution-toolboxes/species-distribution-modelling> | {{ rbib_u_capetown_2024 }} || Single-season occupancy models using a Bayesian approach |

</div>
:::::::

:::::::{tab-item} References
{{ rbib_burton_et_al_2015 }}

{{ rbib_byrne_golden_2021 }}

{{ rbib_chatterjee_et_al_2021 }}

{{ rbib_clarke_et_al_2023 }}

{{ rbib_cove_2020a }}

{{ rbib_cove_2020b }}

{{ rbib_cove_2020c }}

{{ rbib_cove_2020d }}

{{ rbib_donovan_et_al_2024 }}

{{ rbib_efford_dawson_2012 }}

{{ rbib_fidino_2021d }}

{{ rbib_fidino_2021a }}

{{ rbib_fidino_2021b }}

{{ rbib_fidino_2021c }}

{{ rbib_fidino_2021e }}

{{ rbib_fidino_2021f }}

{{ rbib_fidino_2023 }}

{{ rbib_fidino_magle_2017 }}

{{ rbib_fiske_chandler_2011 }}

{{ rbib_gaston_et_al_2000 }}

{{ rbib_gimenez_2020a }}

{{ rbib_gimenez_2020b }}

{{ rbib_gimenez_2023 }}

{{ rbib_guillera_arroita_et_al_2011 }}

{{ rbib_guilleraarroita_2016 }}

{{ rbib_hines_2006 }}

{{ rbib_kellner_et_al_2023 }}

{{ rbib_mackenzie_et_al_2017 }}

{{ rbib_mcneil_nd }}

{{ rbib_murray_et_al_2021 }}

{{ rbib_neilson_et_al_2018 }}

{{ rbib_noon_et_al_2012 }}

{{ rbib_paterson_2024 }}

{{ rbib_proteus_2018 }}

{{ rbib_proteus_2019a }}

{{ rbib_proteus_2019b }}

{{ rbib_proteus_nd }}

{{ rbib_royle_dorazio_2008 }}

{{ rbib_sollmann_2018 }}

{{ rbib_solymos_2023 }}

{{ rbib_southwell_et_al_2019 }}

{{ rbib_steenweg_et_al_2018 }}

{{ rbib_stewart_et_al_2018 }}

{{ rbib_u_capetown_2024 }}

{{ rbib_weecology_2020 }}

{{ rbib_wildco_lab_2021c }}
:::::::

::::::::