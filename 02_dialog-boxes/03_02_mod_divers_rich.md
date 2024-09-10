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

**{{ term_mod_divers_rich_rich }}**: {{ term_def_mod_divers_rich_rich }}
**{{ term_mod_divers_rich_divers }}**: {{ term_def_mod_divers_rich_divers }}

Note that there are multiple “levels” to Species diversity & richness, these include:
- **{{ term_mod_divers_rich_alpha }}**: {{ term_def_mod_divers_rich_alpha }}
- **{{ term_mod_divers_rich_beta }}**: {{ term_def_mod_divers_rich_beta }}
- **{{ term_mod_divers_rich_gamma }}**: {{ term_def_mod_divers_rich_gamma }}

<br>
“Species richness** is simply “the total number of species in an assemblage or a sample” ({{ ref_intext_gotelli_chao_2013 }}.

Species richness in an assemblage is difficult to estimate reliably from sample data because it is very sensitive to the number of individuals and the number of samples collected. Species richness is a diversity of order 0 (which means it is completely insensitive to species abundances).

Species diversity is more complex, and includes a measure of the number of species in a community, and a measure of the abundance of each species. Species diversity is usually described by an index, such as Shannon's Index H'.” {{ ref_intext_pyron_2010 }}

```{figure} ../03_images/03_image_files/pyron_2010_fig1_clipped.png
:align: center
:scale: 60%
```

:::{note}
This section is still in progress
:::

::::::

::::::{tab-item} Advanced
:::{note}
This section is still in progress
:::

Parameters:
- **α-richness (alpha richness)**: species richness at the level of an individual camera location {{ ref_intext_wearn_gloverkapfer_2019 }}
-  **γ-richness (gamma richness)**: species richness across a whole study area {{ ref_intext_wearn_gloverkapfer_2019 }}
- **β-diversity (betadiversity)**: the differences between the communities or, more formally, the variance among the communities {{ ref_intext_wearn_gloverkapfer_2019 }}
<br>

**Observed *vs* estimated species richness** (from {{ ref_intext_wearn_gloverkapfer_2019 }}):
- **Observed species richness**: the sum of the number of species seen (e.g. {{ ref_intext_kitamura_et_al_2010 }}; {{ ref_intext_pettorelli_et_al_2010 }}; {{ ref_intext_ahumada_et_al_2011 }}; {{ ref_intext_samejima_et_al_2012 }})
    -  Observed species richness will not, in general, be a reliable index of actual species richness because, even if sampling effort is strictly controlled, the detectability of species will vary across samples

-  **Estimated species richness**: when the “sum of the number of species seen” is adjusted based on corrections for “imperfect detection” (i.e. the fact that some species in a given sample may have been missed)
    -  (e.g. {{ ref_intext_tobler_et_al_2008 }}; {{ ref_intext_kinnaird-&-obrien-2012 }}; {{ ref_intext_brodie_et_al_2015 }}; {{ ref_intext_yue_et_al_2015 }}; {{ ref_intext_wearn_et_al_2016 }})
    -  The **two principal ways of estimating species richness from remote camera data ** are (from {{ ref_intext_wearn_gloverkapfer_2019 }}):<br> 
        -   non-parametric estimators ({{ ref_intext_gotelli_chao_2013 }}), which use information about the rarest species in the sample to provide a minimum estimate of the number of true species (e.g. {{ ref_intext_tobler_et_al_2008 }}), 
        -   or 2) occupancy models ({{ ref_intext_mackenzie_et_al_2006 }})
::::::

::::::{tab-item} Visual resources
:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_pyron_2010 }}
```{figure} ../03_images/03_image_files/pyron_2010_fig1_clipped.png
:height: 300px
:align: center
```

**Pyron (2010) – Fig. 1**: Species evenness and species richness for animalcule communities
<!-- Both communities contain five species of animalcules. Species richness is the same. The community on the left is dominated by one of the species. The community on the right has equal proportions of each species. Evenness is higher when species are present in similar proportions. Thus the community on the left has higher species diversity, because evenness is higher. -->
::::

::::{grid-item-card} {{ ref_intext_gotelli_chao_2013 }}
```{figure} ../03_images/03_image_files/gotelli_chao_2013_fig1_clipped.png 
:width: 300px
:align: center
```
**Gotelli & Chao (2013) – Fig. 1** Species richness sampling in a hypothetical walk through the woods. Each different symbol represents one of 20 distinct species, and each row contains 20 characters, representing the first 20 individual trees that might be encountered in a random sample. Community A is maximally even, with each of the 20 species comprising 5% of the total abundance. In this assemblage, the two samples of 20 individual trees yielded 15 and 13 species, respectively. Community B is highly uneven, with one species (the open circle) representing 81% of the total abundance, and the remaining 19 species contributing only 1% each. In this assemblage, the two samples of 20 individual trees yielded only three and four species, respectively.
::::

::::{grid-item-card} {{ ref_intext_gotelli_chao_2013 }}
```{figure} ../03_images/03_image_files/gotelli_chao_2013_fig6_clipped.png 
:width: 300px
:align: center
```
**Gotelli & Chao (2013) – Fig. 6** Diversity profile for assemblages of differing evenness. The x-axis is the order *q* in the Hill number (eqn [23a]), and is illustrated for values of *q* from 0 to 5. The y-axis is the calculated Hill number (the equivalent number of equally abundant species). Each of the four assemblages has exactly 100 species and 500 individuals, but they differ in their relative evenness: (1) completely even assemblage (black solid line): each species is represented by five individuals; (2) slightly uneven assemblage (red dashed line): 50 species each represented by seven individuals and 50 species each represented by three individuals (this structure is denoted as {50 x 7, 50 x 3}); (3) moderately uneven assemblage (green dotted line): {22 x 10, 28 x 5, 40 x 3, 10 x 2}; (4) highly uneven assemblage (blue dash–dot line): {1 x 120, 1 x 80, 1 x 70, 1 x 50, 3 x 20, 3 x 10, 90 x 1}. For *q*=0, the Hill number is species richness, which is equal to 100 for all assemblages. Because Hill numbers represent the equivalent number of equally abundant species, the curve for the perfectly even assemblage (black solid line) does not change as q is increased. Larger values of q place progressively more weight on common species, so the equivalent number of equally abundant species is much lower for the more uneven assemblages than for more even assemblages.
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

Abundance, species richness, and diversity
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

Species accumulation and rarefaction curves
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

Using vegan to calculate alpha diversity metrics within the tidyverse in R (CC196)
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

Species abundance tools in Genstat 
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

Species Diversity and Species Richness
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

Field Ecology - Diversity Metrics in R
::::

:::::


:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_riffomonas_project_2022b }} 

<iframe 
    width="300"
    height="200"
    src="https://www.youtube.com/embed/ywHVb0Q-qsM?si=_xJ5jbFc6MDEQlAh "
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

Generating a rarefaction curve from collector's curves in R within the tidyverse (CC198)
::::

:::::

::::::

::::::{tab-item} Shiny apps/Widgets
:::::{card}
**iNext Online**

 Software for interpolation and extrapolation of species diversity.

<iframe 
    width="100%"
    height="900"
    src="https://chao.shinyapps.io/iNEXTOnline"
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
| R package | R package “vegan | \- | <https://cran.r-project.org/web/packages/vegan/index.html> | {{ ref_bib_oksanen_et_al_2024 }} |
| Program | EstimateS | Dedicated software for estimating diversity, using asymptotic or rarefaction methods. Mac version available | <https://www.robertkcolwell.org/pages/1407> | {{ ref_bib_colwell_2022 }} |
| R package | Package ‘iNEXT’ - Interpolation and Extrapolation for Species Diversity | The iNext package (INterpolation and EXTrapolation of species richness) - is both easy to use and rapid to compute. It also comes with a wealth of plotting functions - see the iNext Quick Introduction for a great walk through tutorial. Its core functionality is based on: Chao, Anne, et al. “Rarefaction and extrapolation with Hill numbers: a framework for sampling and estimation in species diversity studies.” Ecological monographs 84.1 (2014): 45-67. | <https://cran.r-project.org/web/packages/iNEXT/iNEXT.pdf> | {{ ref_bib_chao_et_al_2016 }} |
| Exercise/Tutorial | 2.2: Measuring Species Diversity | Easy to interpet explanation of species richness vs evenness, species area curves, rarefaction, and how to calculate diversity | <https://bio.libretexts.org/Courses/University_of_California_Davis/BIS_2B%3A_Introduction_to_Biology_-_Ecology_and_Evolution/02%3A_Biodiversity/2.02%3A_Measuring_Species_Diversity> | {{ ref_bib_gerhartbarley_nd }} |
| R package / Tutorial | Species Accumulation Curves with vegan, BiodiversityR and ggplot2 | Software for interpolation and extrapolation of species diversity | <https://rpubs.com/Roeland-KINDT/694021> | {{ ref_bib_roeland_2020 }} |
::::::

::::::{tab-item} References
<font size="3">

{{ ref_bib_ahumada_et_al_2011 }}

{{ ref_bib_baylor_tutoring_center_2021 }}

{{ ref_bib_brodie_et_al_2015 }}

{{ ref_bib_chao_et_al_2016 }}

{{ ref_bib_chao_et_al_2014 }}

{{ ref_bib_colwell_2022 }}

{{ ref_bib_gerhartbarley_nd }}

{{ ref_bib_gotelli_chao_2013 }}

{{ ref_bib_gotelli_colwell_2001 }}

{{ ref_bib_gotelli_colwell_2010 }}

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

{{ ref_bib_riffomonas_project_2022b }}

{{ ref_bib_samejima_et_al_2012 }}

{{ ref_bib_styring_2020a }}

{{ ref_bib_styring_2020b }}

{{ ref_bib_tobler_et_al_2008 }}

{{ ref_bib_vsn_international_2022 }}

{{ ref_bib_wearn_et_al_2016 }}

{{ ref_bib_wildco_lab_2021b }}

{{ ref_bib_yue_et_al_2015 }}
</font>
::::::

:::::::

:::::::::