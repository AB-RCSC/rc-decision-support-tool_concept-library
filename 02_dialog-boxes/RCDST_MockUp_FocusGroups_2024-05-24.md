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

# Capture-recapture (CR) / Capture-mark-recapture (CMR)

```````{div} full-width

``````{admonition} Click here for more information
:class: dropdown

{{ key1 }}

{{ key2 }}

[number_of_images](/09_glossary_ref/09_01_glossary2.ipynb#number_of_images)

{hoverxref}`like this <#number_of_images>`

**Capture-recapture (CR) model / Capture-mark-recapture (CMR) model (Karanth, 1995; Karanth & Nichols, 1998)**: A method of estimating the abundance or density of marked populations using the number of animals detected and the likelihood animals will be detected (detection probability). CR (Karanth, 1995; Karanth & Nichols, 1998) can be used to estimate vital rates where all newly detected unmarked animals become marked and are distinguishable in future (Efford, 2022). Spatially explicit capture-recapture (SECR; Borchers & Efford, 2008; Efford, 2004; Royle & Young, 2008) models have largely replaced CR and CMR models and provide more accurate density estimates (Blanc et al., 2013, Obbard et al., 2010, Sollmann et al., 2011).

:::::{dropdown} **Assumptions, Pros, Cons**
::::{grid} 3
:::{grid-item-card}  **Assumptions**
-   Demographic closure (i.e., no births or deaths)<sup>1</sup>

-   Geographic closure (i.e., no immigration or emigration)<sup>1</sup>

-   All individuals have at least some probability of being detected<sup>2</sup>

-   Sampled area encompasses the full extent of individuals’ movements<sup>2,10</sup>

-   Activity centres are randomly dispersed<sup>12</sup>

-   Activity centres are stationary<sup>12</sup>

:::
:::{grid-item-card}  **Pros** 
-   May be used as a [relative abundance index](#mods_relative_abundance) that controls for [imperfect detection](#imperfect_detection)<sup>1</sup>

-   Easy-to-use software exists to implement (e.g., CAPTURE); MARK Implements more complicated models with covariates (and must be used for [mark-resight modelling](#mods_marked__resight))<sup>1</sup>

-    Can use the robust design with “open” models to obtain recruitment and survival rate estimates<sup>1</sup>

:::
:::{grid-item-card}  **Cons**
-   Requires that individuals are distinguishable.<sup>1</sup> However, CR<sup>10,11</sup> has also been used to estimate abundance of species that lack natural markers but that have phenotypic and/or environment-induced characteristics<sup>2,13,14</sup>

-   When the sample size is large enough to reliably estimate [density](#density)  with CR,<sup>10,11</sup> individuals are unlikely to have a unique marker<sup>2,13,14</sup>

-   Dependent on the surveyed area, which is difficult to track and calculate<sup>1</sup>

-   Requires a minimum number of captures and recaptures<sup>1</sup>

-   Relatively stringent requirements for study design (e.g., no “holes” in the trapping grid)<sup>1</sup>

-   Geographic closure at the plot level, which is often unrealistic<sup>1</sup>

-   Assumes a specific relationship between abundance and detection<sup>1</sup>

-   [Density](#density) cannot be explicitly estimated because the true area animals occupy is never measured (only approximated)<sup>16</sup>
:::
::::
:::::

`````{tab-set}
:selected: true
````{tab-item}   Overview

```{image} ./03_images/00_demo/CR_EMBED_LAYMAN_EXAMPLE1.png
:width: 80%
:align: center
```
```{image} ./03_images/00_demo/CR_EMBED_LAYMAN_EXAMPLE2.png
:width: 90%
:align: center
```
````
````{tab-item} Advanced
\
To estimate density using camera trap CR, we must first estimate population size 𝑁. CR models use individuals’ detection histories – that is, the record of when each individual was photographed or not photographed (i.e., (re)captured or not (re)captured) – to solve for 𝑁 (Figure 3; Royle 2020). Population-level detection histories look like a matrix of 1s and 0s, where 1s signify that an individual was captured during a given sampling occasion 𝑘, and 0s signify that the individual was not captured during that occasion (Royle 2020, Royle et al. 2014). The number of individuals photographed at least once over the course of the study (i.e., the count of animals captured) is 𝑛.  
Importantly, the count of animals is not the same as the size of the population (i.e., 𝑛 ≠ 𝑁). Some individuals will never be photographed during a study, even though they are present and able to be detected (i.e., they are in 𝑁 but not in 𝑛; Royle 2020). Using the matrix of detection histories, we must therefore calculate the likelihood animals will be detected by an array of camera traps – that is, detection probability p (Royle 2020). 
Taking this information together, we can calculate population size 𝑁 as:

```{image} ./03_images/00_demo/Clarke-et-al_2023_eqn_cr1.png
:width: 80px
:align: center
```

which is often referred to as the canonical estimator of population size (Royle 2020). Population size 𝑁 can then be divided by an estimate of the area of the sampling frame 𝐴 to obtain density. 
CR models have important limitations – notably that they do not consider the spatial configuration of camera traps or the spatial pattern of animal detections. This gives rise to two major issues: 
The sampling frame 𝐴 is not known (Chandler and Royle, 2013). In other words: the true area animals occupy is never measured, only approximated using adhoc approaches (e.g., using a buffer strip around the trap array; Rich et al., 2014, Sollmann, 2018). Consequently, density cannot be calculated explicitly (Chandler and Royle, 2013), and CR-derived density estimates are somewhat arbitrary and difficult to compare across studies (Green et al., 2020, Royle et al., 2014, Sollmann, 2018). 
Detection probability is assumed to be the same across all individuals and sampling occasions, even though the likelihood a given individual is detected at a given camera trap will change with its proximity to that trap. An animal that occupies territory far away from a trap is less likely to be detected there than one that lives nearby, for example (Morin et al. 2022). 
The standard CR model has largely been phased out with the advent of spatially-explicit CR models (see 2.1.2 Spatial Capture-Recapture; Burton et al. 2015, Sollmann 2008), which address the shortcomings of CR and have been shown to produce more accurate density estimates (e.g., Blanc et al. 2013, Obbard et al. 2010, Sollmann et al. 2011).

````

````{tab-item} Visual Resources
::::{grid} 3

:::{grid-item-card}
:header: J. Andrew Royle,"Spatial Capture-Recapture Modelling" ✨
:padding: 0
:margin: 0
:::{iframe} https://www.youtube.com/embed/4HKFimATq9E
:width: 100%
:::

:::{grid-item-card}
:header: PAWS: Spatial Capture Recapture Data Analysis Part 1 ✨
:::{iframe} https://www.youtube.com/embed/aTbk-jWyMcU
:width: 100%
:::

:::{grid-item-card}
:header: PAWS: Spatial Capture Recapture Data Analysis Part 2 ✨
:padding: 0
:margin: 0
:::{iframe} https://www.youtube.com/embed/IHVez1a_hqg
:width: 100%
:::
::::

::::{grid} 3

:::{grid-item-card}

```{image} ../03_images/03_image_files/Rowcliffe-et-al_2008_Fig1.png
:width: 100%
:align: center
```
<p style="text-align:center">*(Rowcliffe et al, 2008)* </p>

:::

:::{grid-item-card}

```{image} ../03_images/03_image_files/Wearn_GloverKapfer_2018_Fig2.png
:width: 100%
:align: center
```
<p style=""text-align:center"">*(Wearn & Glover-Kapfer, 2019)* </p>

:::


:::{grid-item-card}
ta da
:::


::::


````
````{tab-item} Analytical tools & resources
| Name | URL | Note | Reference |
| -- | -- | -- | -- |
| R package - “RMark” | <https://cran.r-project.org/web/packages/RMark/index.html> | "The R counterpart to MARK, allowing complex models to be fit using just a few lines of code. With some work, it is possible to get RMark functioning on Mac and Linux (see RMark documentation)." (Wearn & Glover-Kapfer, 2017) | Laake J (2013). “RMark: An R Interface for Analysis of Capture-Recapture Data with MARK.” AFSC Processed Rep. 2013-01, Alaska Fish. Sci. Cent., NOAA, Natl. Mar. Fish. Serv., Seattle, WA. https://apps-afsc.fisheries.noaa.gov/Publications/ProcRpt/PR2013-01.pdf. |
| R package - “multimark” | <https://cran.r-project.org/web/packages/multimark/index.html> | Conventional capture-recapture using multiple marks - Conventional capture-recapture (and mark-resight) "Allows for an integrated analysis of data on two individuallyidentifiable animal marks (e.g. left and right flanks of animals), as might be obtained from capture-recapture surveys which do not use paired cameras. Also implements standard models using a single mark." (Wearn & Glover-Kapfer, 2017) | McClintock BT (2015). “multimark: an R package for analysis of capture–recapture data consisting of multiple “noninvasive” marks.” Ecology and Evolution, 5(21), 4920–4931. https://doi.org/10.1002/ece3.1676. |
| Program - “MARK” | <www.phidot.org/software/mark/downloads> | Conventional capture-recapture (and mark-resight) "Relatively complex and comprehensive software with a steep learning curve. Also implements occupancy models. Fits models using maximum likelihood methods (unlike CAPTURE), allowing for model selection and hypothesis testing. Good support available from an active community." (Wearn & Glover-Kapfer, 2017) | White, G. C., & Burnham, K. P. (1999). Program MARK: Survival estimation from populations of marked animals. Bird Study, 46(sup1), S120–S139. https://doi.org/10.1080/00063659909477239 |
| Program - “CAPTURE” | <www.mbr-pwrc.usgs.gov/software/capture.shtml> | "Software for making abundance and density estimates using a limited range of conventional capture-recapture models. Inference is based on the models in White et al. (1978), rather than modern maximum likelihood estimation." (Wearn & Glover-Kapfer, 2017) |  |

````
````{tab-item} References
<font size="1">

Ahumada, J. A., Fegraus, E., Birch, T., Flores, N., Kays, R., O'Brien, T. G., Palmer, J., Schuttler, S., Zhao, J. Y., Jetz, W., Kinnaird, M., Kulkarni, S., Lyet, A., Thau, D., Duong, M., Oliver, R., & Dancer, A. (2019). Wildlife Insights: A Platform to Maximize the Potential of Camera Trap and Other Passive Sensor Wildlife Data for the Planet. *Environmental Conservation*, 47(1), 1-6. <https://doi.org/10.1017/s0376892919000298>

Ahumada, J. A., Silva, C. E. F., Gajapersad, K., Hallam, C., Hurtado, J., Martin, E., McWilliam, A., Mugerwa, B., O'Brien, T., Rovero, F., Sheil, D., Spironello, W. R., Winarni, N., & Andelman, S. J. (2011). Community Structure and Diversity of Tropical Forest Mammals: Data from a Global Camera Trap Network. *Philosophical Transactions: Biological Sciences, 366*(1578), 2703-2711. <https://doi.org/10.1098/rstb.2011.0115>

Alberta Biodiversity Monitoring Institute [ABMI] (2021). *Terrestrial ARU and Remote Camera Trap Protocols:* Edmonton, Alberta. <https://abmi.ca/home/publications/551-600/599>




</font>\
````

````{tab-item} Glossary
**\*Access Method**
:   The method used to reach the camera location (e.g., on "Foot," "ATV," "Helicopter," etc.).

**\*Adult**
:   Animals that are old enough to breed; reproductively mature.

````
`````

``````

```````