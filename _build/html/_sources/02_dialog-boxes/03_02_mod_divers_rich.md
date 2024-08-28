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
(i_mod_divers_rich)=
# {{ name_mod_divers_rich }}

:::::::::{div} full-width

::::::{dropdown} Assumptions, Pros, Cons

:::::{dropdown} Species richness (Alpha diversity)
::::{grid}
:::{grid-item-card} Assumptions
- {{ mod_divers_rich_alpha_assump_01 }}
- {{ mod_divers_rich_alpha_assump_02 }}
- {{ mod_divers_rich_alpha_assump_03 }}
- {{ mod_divers_rich_alpha_assump_04 }}
:::
:::{grid-item-card} Pros
- {{ mod_divers_rich_alpha_pro_01 }}
- {{ mod_divers_rich_alpha_pro_02 }}
- {{ mod_divers_rich_alpha_pro_03 }}
:::
:::{grid-item-card} Cons
- {{ mod_divers_rich_alpha_con_01 }}
- {{ mod_divers_rich_alpha_con_02 }}
- {{ mod_divers_rich_alpha_con_03 }}
:::
::::
:::::

:::::{dropdown} Species diversity (Beta diversity)
::::{grid}
:::{grid-item-card} Assumptions
- {{ mod_divers_rich_beta_assump_01 }}
- {{ mod_divers_rich_beta_assump_02 }}
- {{ mod_divers_rich_beta_assump_03 }}
:::
:::{grid-item-card} Pros
- {{ mod_divers_rich_beta_pro_01 }}
- {{ mod_divers_rich_beta_pro_02 }}
- {{ mod_divers_rich_beta_pro_03 }}
:::
:::{grid-item-card} Cons
- {{ mod_divers_rich_beta_con_01 }}
- {{ mod_divers_rich_beta_con_02 }}
- {{ mod_divers_rich_beta_con_03 }}
:::
::::
:::::

:::::{dropdown} Species diversity (Gamma diversity)
::::{grid}
:::{grid-item-card} Assumptions
- {{ mod_divers_rich_gamma_assump_01 }}
- {{ mod_divers_rich_gamma_assump_02 }}
- {{ mod_divers_rich_gamma_assump_03 }}
:::
:::{grid-item-card} Pros
- {{ mod_divers_rich_gamma_pro_01 }}
- {{ mod_divers_rich_gamma_pro_02 }}
:::
:::{grid-item-card} Cons
- {{ mod_divers_rich_gamma_con_01 }}
- {{ mod_divers_rich_gamma_con_02 }}
- {{ mod_divers_rich_gamma_con_03 }}
:::
::::
:::::
::::::

:::::::{tab-set}
::::::{tab-item} Overview

**{{ term_mod_divers_rich }}**: {{ term_def_mod_divers_rich }}
<br>
“Species richness is simply the number of species in a community. 

Species diversity is more complex, and includes a measure of the number of species in a community, and a measure of the abundance of each species. Species diversity is usually described by an index, such as Shannon's Index H'.” {{ ref_intext_pyron_2010 }}

```{figure} ../03_images/03_image_files/pyron_2010_fig1.png
:align: center
:scale: 60%
```

::::::

::::::{tab-item} Advanced
<br>
Parameters:
- **α-richness (alpha richness)**: species richness at the level of an individual camera location
-  **γ-richness (gamma richness)**: species richness across a whole study area
- **β-diversity (betadiversity)**: the differences between the communities or, more formally, the variance among the communities
<br>

**Observed *vs* estimated species richness** (from {{ ref_intext_wearn_gloverkapfer_2019 }}):
- **Observed species richness**: the sum of the number of species seen (e.g. {{ ref_intext_kitamura_et_al_2010 }}; {{ ref_intext_pettorelli_et_al_2010 }}; {{ ref_intext_ahumada_et_al_2011 }}; {{ ref_intext_samejima_et_al_2012 }})
- Observed species richness will not, in general, be a reliable index of actual species richness because, even if sampling effort is strictly controlled, the detectability of species will vary across samples
-  **Estimated species richness** (e.g. {{ ref_intext_tobler_et_al_2008 }}; {{ ref_intext_kinnaird_obrien_2012 }}; {{ ref_intext_brodie_et_al_2015 }}; {{ ref_intext_yue_et_al_2015 }}; {{ ref_intext_wearn_et_al_2016 }})
  -   Species richness estimation involves attempting to correct for “imperfect detection”, i.e. the fact that some species in a given sample may have been missed (Box 6-1).
<br>

The **two principal ways of estimating species richness from camera trap dat ** are (from {{ ref_intext_wearn_gloverkapfer_2019 }}):<br> 
- non-parametric estimators ({{ ref_intext_gotelli_chao_2013 }}), which use information about the rarest species in the sample to provide a minimum estimate of the number of true species (e.g. {{ ref_intext_tobler_et_al_2008 }}), 
- or 2) occupancy models ({{ ref_intext_mackenzie_et_al_2006 }})
<br>
::::::

::::::{tab-item} Visual resources

:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_pyron_2010 }}
```{figure} ../03_images/03_image_files/pyron_2010_fig1_clipped.png 
:width: 300px
:align: center
```

<p>**Figure 1: Species evenness and species richness for animalcule communities**<br>
Both communities contain five species of animalcules. Species richness is the same. The community on the left is dominated by one of the species. The community on the right has equal proportions of each species. Evenness is higher when species are present in similar proportions. Thus the community on the left has higher species diversity, because evenness is higher. <p/>
::::

::::{grid-item-card} {{ ref_intext_pyron_2010 }}
```{figure} ../03_images/03_image_files/pyron_2010_fig1.png 
:width: 300px
:align: center
```

<p>NULL <p/>
::::

::::{grid-item-card} {{ ref_intext_figure3_ref_id }}
```{figure} ../03_images/03_image_files/figure3_filename.png 
:width: 300px
:align: center
```

<p>figure4_caption <p/>
::::

:::::

:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_molloy_2018 }}
```{figure} ../03_images/03_image_files/molloy_2018_fig9.png 
:width: 300px
:align: center
```

<p>figure5_caption <p/>
::::

::::{grid-item-card} {{ ref_intext_figure5_ref_id }}
```{figure} ../03_images/03_image_files/figure5_filename.png 
:width: 300px
:align: center
```
<p>figure5_caption <p/>
::::

::::{grid-item-card} {{ ref_intext_figure6_ref_id }}
```{figure} ../03_images/03_image_files/figure6_filename.png
:width: 300px
:align: center
```
<p>figure6_caption <p/>
::::

:::::

:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_project_dragonfly_2019 }}

<iframe 
    width="300"
    height="200"
    src="https://www.youtube.com/embed/ghhZClDRK_g?si=khprL1u5NJrFduTb"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

<p>Abundance, species richness, and diversity<p/>
::::

::::{grid-item-card} {{ ref_intext_mecks100_2018 }}

<iframe 
    width="300"
    height="200"
    src="https://www.youtube.com/embed/4gcmAUpo9TU?si=_S-JYDDskR8QbHs5"
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

<p>Species accumulation and rarefaction curves<p/>
::::

::::{grid-item-card} {{ ref_intext_riffomonas_project_2022a }}

<iframe 
    width="300"
    height="200"
    src="https://www.youtube.com/embed/wq1SXGQYgCs?si=Re5tglERblfkCNhDl"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

<p>Using vegan to calculate alpha diversity metrics within the tidyverse in R (CC196)<p/>
::::
:::::

:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_vsn_international_2022 }}

<iframe 
    width="300"
    height="200"
    src="https://www.youtube.com/embed/wBx7f4PP8RE?si=D6mtAMNMLlk3aH8H"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

<p>Species abundance tools in Genstat<p/>
::::

::::{grid-item-card} {{ ref_intext_baylor_tutoring_center_2021 }}
 
<iframe 
    width="300"
    height="200"
    src="https://www.youtube.com/embed/UXJ0r4hjbqI?si=gYR6rOmIMgyibyvR"
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

<p>Species Diversity and Species Richness<p/>
::::

::::{grid-item-card} {{ ref_intext_styring_2020a }}

<iframe 
    width="300"
    height="200"
    src="https://www.youtube.com/embed/KBByV3kR3IA?si=RPcG1lFQ-v0Shwaw"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

<p>Field Ecology - Diversity Metrics in R<p/>
::::

:::::

::::::

::::::{tab-item} Shiny
:::::{card}
**Visualizing Biodiversity in \[U.S.\] National Parks**

<!-- https://shiny.posit.co/r/gallery/life-sciences/biodiversity-national-parks/-->

<iframe 
    width="100%"
    height="1100"
    src="https://abenedetti.shinyapps.io/bioNPS/"
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

:::::
::::::

::::::{tab-item} Analytical tools & resources

| Type | Name | Note | URL |Reference |
|:----------------|:---------------------------------------|:----------------------------------------------------------------|:----------------------------------------------------------------|:----------------------------------------------------------------|
| R package | Chapter 9 Community composition | \- | <https://bookdown.org/c_w_beirne/wildCo-Data-Analysis/composition.html#estimated-richnes> | {{ ref_bib_wildco_lab_2021b }} |
| Program | R package “vegan | Dedicated software for estimating diversity, using asymptotic or rarefaction methods. Mac version available | <https://www.robertkcolwell.org/pages/1407> | {{ ref_bib_oksanen_et_al_2024 }} |
| Program | EstimateS | Dedicated software for estimating diversity, using asymptotic or rarefaction methods. Mac version available | <https://www.robertkcolwell.org/pages/1407> | {{ ref_bib_colwell_2022 }} |
| R package | Package ‘iNEXT’ - Interpolation and Extrapolation for Species Diversity | The iNext package (INterpolation and EXTrapolation of species richness) - is both easy to use and rapid to compute. It also comes with a wealth of plotting functions - see the iNext Quick Introduction for a great walk through tutorial. Its core functionality is based on: Chao, Anne, et al. “Rarefaction and extrapolation with Hill numbers: a framework for sampling and estimation in species diversity studies.” Ecological monographs 84.1 (2014): 45-67. | >https://cran.r-project.org/web/packages/iNEXT/iNEXT.pdf> | {{ ref_bib_hsieh_et_al_2015 }} |
| Exercise/Tutorial | 2.2: Measuring Species Diversity | Easy to interpet explanation of species richness vs evenness, species area curves, rarefaction, and how to calculate diversity | <https://bio.libretexts.org/Courses/University_of_California_Davis/BIS_2B%3A_Introduction_to_Biology_-_Ecology_and_Evolution/02%3A_Biodiversity/2.02%3A_Measuring_Species_Diversity> | {{ ref_bib_gerhartbarley_nd }} |
| R package / Tutorial | Species Accumulation Curves with vegan, BiodiversityR and ggplot2 | Software for interpolation and extrapolation of species diversityRarefied Species Accumulation Curves (the simple way) | <https://rpubs.com/Roeland-KINDT/694021> | {{ ref_bib_resource6_ref_id }} |
| resource7_type | resource7_name | resource7_note | resource7_url | {{ ref_bib_resource7_ref_id }} |
::::::

::::::{tab-item} References
{{ ref_bib_ahumada_et_al_2011 }}

{{ ref_bib_baylor_tutoring_center_2021 }}

{{ ref_bib_brodie_et_al_2015 }}

{{ ref_bib_colwell_2022 }}

{{ ref_bib_gerhartbarley_nd }}

{{ ref_bib_gotelli_colwell_2001 }}

{{ ref_bib_gotelli_colwell_2011 }}

{{ ref_bib_hsieh_et_al_2015 }}

{{ ref_bib_iknayan_et_al_2014 }}

{{ ref_bib_kinnaird_obrien_2012 }}

{{ ref_bib_kitamura_et_al_2010 }}

{{ ref_bib_mackenzie_et_al_2006 }}

{{ ref_bib_mecks100_2018 }}

{{ ref_bib_oksanen_et_al_2024 }}

{{ ref_bib_pettorelli_et_al_2010 }}

{{ ref_bib_project_dragonfly_2019 }}

{{ ref_bib_pyron_2010 }}

{{ ref_bib_riffomonas_project_2022a }}

{{ ref_bib_samejima_et_al_2012 }}

{{ ref_bib_styring_2020a }}

{{ ref_bib_tobler_et_al_2008 }}

{{ ref_bib_vsn_international_2022 }}

{{ ref_bib_wearn_et_al_2016 }}

{{ ref_bib_wildco_lab_2021b }}

{{ ref_bib_yue_et_al_2015 }}
::::::

:::::::

:::::::::