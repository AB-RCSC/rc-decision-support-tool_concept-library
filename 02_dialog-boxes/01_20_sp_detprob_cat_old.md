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
(i_sp_det_prob_cat)=
# {{ name_sp_det_prob_cat }}

:::::::::{div} full-width

:::::::{tab-set}

::::::{tab-item} Overview

<br>**Detection probability categories are defined as follows:**

- **Low**:
    -    < 0.1 ({{ ref_intext_tobler_powell_2013 }})
    -    < 0.05 ({{ ref_intext_shannon_et_al_2014 }})
    -     0–0.37 ({{ ref_intext_chatterjee_et_al_2021 }})

- **Medium**: 
    -    0.37–0.67 ({{ ref_intext_chatterjee_et_al_2021 }})

- **High**:
    -    0.67–1 ({{ ref_intext_chatterjee_et_al_2021 }})
    -    \> 0.5 ({{ ref_intext_mackenzie_royle_2005 }})

- **Unknown**: select this option if you’re not sure of the detection probability of your [Target Species](/09_glossary.md#target_species) (single or multiple species)

- **Multiple**: select this option if your study include multiple [Target Species](/09_glossary.md#target_species).

:::{admonition} How this question relates to study design
:class: tip

{{ term_detection_probability }}**: {{ term_def_detection_probability }}

We use this information to adjust the recommended [camera days per camera location](09_glossary.md#camera_days_per_camera_location) and [total number of camera days](09_glossary.md#total_number_of_camera_days). For example, if the species is hard to detect, you may have to deploy cameras for longer to ensure you’ve sampled long enough to say that the species truly was not there (*vs.* it was there, but you did not detect it; “missed detections”, e.g., high cover of shrubs impeding your ability to see the species).

You may need to consult previous studies to get a sense of which category is the most appropriate for your study and Target Species.

> Select “Unknown” if you’re not sure.
:::

:::{admonition} How does that work?
:class: note

**How does that work? **
\
Individuals and/or species are not always detected when they are present (i.e., detected "imperfectly”; ({{ ref_intext_mackenzie_et_al_2004 }}). Missed detections occur or many reasons, including due characteristics of the environment (e.g., due to cover of vegetation), the time period (e.g., seasons), characteristics of the species (e.g., cryptic nature or small size), etc. **The question here is asking about detection probability as it relates to the characteristIcs of the species (not the species in a particular habitat type or during a specific season).**

```{image} ../03_images/03_image_files/det.gif
:width: 200px
:align: center
```

:::{image} ../03_images/03_image_files/det.gif
:width: 400px
:align: center
:::


**Why do we care?**
\
We care about this because when you fail to detect an individual/species that was, in fact, present, this is called a “false absence”, which may lead to incorrect conclusions from the data. Understanding and correcting for sources of this type of error is often thought of in terms of probabilities (i.e., "detection probability" aka detectability).

:::

:::{admonition} It’s not an exact science
:class: warning

\
Since detectability is affected by many other processes, detectability is best incorporated from models that use your data since this will result in the best suited infromation to inform your design; however, when you are first designing your study, this is not possible…..[insert more here]
:::

:::{admonition} Analysis aside
:class: seealso

\
Many sources of detection error can be accounted for in analysis; this is done by assessing the relationships between the characteristics of the environment that we might expect to affect detection (e.g., cover of shrubs in front of the camera), and information on where (and when) the species was and was not detected. For example, there were consistently fewer detections on cameras placed in high shrub cover. 

By assessing the relationships at locations repeatedly sampled over time, we begin to unravel the relationship between the environmental characteristics and missed detections on your cameras. We can then use this information to determine if we have sampled long enough (i.e., do we have enough information to differentiate between missed detections and true absences) and/or correct for this error in analysis by incorporating these effects in our models.
:::::::::

::::::{tab-item} Advanced
\
Before study design choices are made, there is one critical concept to understand in remote camera research, which may impact study design choices at all levels of the data hierarchy. Reliable use of remote cameras to detect wildlife species hinges on the [assumption](/09_glossary.md#mods_modelling_assumption) that what is captured on the cameras accurately reflects what is present on the landscape. However, species are often detected "imperfectly," meaning that they are not always detected when they are present (i.e., [imperfect detection](/09_glossary.md#imperfect_detection); e.g., due to cover of vegetation, cryptic nature or small size) ({{ ref_intext_mackenzie_et_al_2004 }}). [Imperfect detection](/09_glossary.md#imperfect_detection) can occur because the camera failed to capture an individual present at the site or because the animal was simply not present during the [survey](/09_glossary.md#survey) period ({{ ref_intext_martin_et_al_2005 }}).

[Imperfect detection](/09_glossary.md#imperfect_detection) results in “false absences” and may lead to incorrect conclusions from the data. Understanding and correcting for sources of “false absences” is often thought of in terms of probabilities. [Detection probability](/09_glossary.md#detection_probability) is the probability (likelihood) that an individual from the population of interest is included in the count at time or location *i* ({{ ref_intext_mackenzie_kendall_2002 }}). [Detection probability](/09_glossary.md#detection_probability) can be influenced through multiple processes and at multiple scales. Understanding the sources of “false absences” and factors that affect [detection probabilities](/09_glossary.md#detection_probability) is an essential step when designing a study, deploying cameras and analyzing camera data.

The [detection probability](/09_glossary.md#detection_probability) of an animal by a camera depends on three **conditional probabilities (Pr) of detection** that may operate alone or potentially in combination ([Figure 1](#TOC_surv_guidelines_fig_1)).

(TOC_surv_guidelines_fig_1)=

```{figure} ../03_images/03_image_files/rcsc_et_al_2024_detection-probability-2023-05-04.png
:height: 700px
:align: center
```  

**Figure 1.** Three conditional probabilities (Pr) of detection that may impact the [detection probability](/09_glossary.md#detection_probability) of an animal (or species) by a camera (adapted from Moeller et al. \[2023\], Hofmeester et al. \[2019\], and Findlay et al. \[2020\]).

[Detection probability](/09_glossary.md#detection_probability) can be affected by species-specific characteristics, [Camera Model](/09_glossary.md#camera_model) specifications and set-up, and environmental variables ({{ ref_intext_hofmeester_et_al_2019 }}). For example, **species-specific characteristics** (individuals or populations), such as body size (e.g., {{ ref_intext_obrien_et_al_2011 }}), behaviour (e.g., {{ ref_intext_caravaggi_et_al_2020 }}; {{ ref_intext_rowcliffe_et_al_2011 }}), and rarity can influence [detection probability](/09_glossary.md#detection_probability), with larger, bolder and more common species generally having higher [detection rates](/09_glossary.md#detection_rate). [**Camera Model**](/09_glossary.md#camera_model) **specifications and set-up**, such as the [Trigger Sensitivity](/09_glossary.md#settings_trigger_sensitivity), [Camera Height](/09_glossary.md#camera_height), or [angle](/09_glossary.md#camera_angle) may affect [detection probability](/09_glossary.md#detection_probability) in that smaller species might not be detected or identifiable if the [Trigger Sensitivity](/09_glossary.md#settings_trigger_sensitivity) is low, or the [Camera Height](/09_glossary.md#camera_height) or [angle](/09_glossary.md#camera_angle) is too high. The [Camera Direction](/09_glossary.md#camera_direction) could impact the probability of an animal triggering a camera if it is directed towards an object that impedes the [Field of View (FOV)](/09_glossary.md#field_of_view) or image quality (e.g. due to sun glare). **Environmental factors** (e.g., vegetation cover, snow depth) may affect [detection probability](/09_glossary.md#detection_probability) and occurrence (e.g., {{ ref_intext_becker_et_al_2022 }}; {{ ref_intext_hofmeester_et_al_2019 }}; {{ ref_intext_iknayan_et_al_2014 }}; {{ ref_intext_steenweg_et_al_2019 }}). For example, a low number of detections in a densely vegetated site might be because of poor camera visibility or avoidance of this habitat by the species of interest.

Hofmeester et al. (2019) suggested there are **six scales (orders) that may impact** [detection probability](/09_glossary.md#detection_probability) and that should be considered within an explicit time period (adapted from Hofmeester et al. \[2019\]; [Figure 2](#TOC_surv_guidelines_fig_2)):

1)  **Distribution range** (1st order; i.e., the physical or geographical range of a species)

2)  **Landscape** (2nd order; i.e., the location of an individual’s home range within the geographic range)

3)  **Habitat patch** (3rd order; i.e., usage of habitat components within an individual’s home range)

4)  **Microsite** (4th order; usage of microhabitats such as food items/feeding patches/nest sites/movement trails, etc. within a habitat)

5)  **Camera specification / set-up** (5th order; i.e., factors that affect the probability that an animal [triggers](/09_glossary.md#trigger_event) the camera if present)

6)  **Image** (6th order; i.e., factors that affect correct identification of animals or individuals)

(TOC_surv_guidelines_fig_2)=

```{figure} ../03_images/03_image_files/rcsc_et_al_2024_detectionprob_hofmeester_et_al_2019_fig1.png
:scale: 70%
:align: center
```  

**Figure 2.** Spatial scales (1-6) and processes that determine the [detection probability](/09_glossary.md#detection_probability) ({{ ref_intext_hofmeester_et_al_2019 }}; abbreviated figure caption).

It is important to consider how all these factors and scales will impact study design. Unmeasured variation in [detection probability](/09_glossary.md#detection_probability) can result in the inability to differentiate the effects of [detection probability](/09_glossary.md#detection_probability) *vs.* habitat preference ({{ ref_intext_jennelle_et_al_2002 }}) and, in turn, cause erroneous estimates of occurrence and abundance ({{ ref_intext_burton_et_al_2015 }}; {{ ref_intext_denes_et_al_2015 }}; {{ ref_intext_kays_et_al_2021 }}).

Factors that influence [detection probability](/09_glossary.md#detection_probability) at the microsite and camera specification / set-up scales are likely to result in the largest biases and thus warrant the most consideration (see Hofmeester et al. [2019] for details). Therefore, it is particularly important to consider *how* to place cameras to avoid such biases. Deploying cameras in a consistent fashion (e.g., carefully ensuring that cameras are always set at the same [Camera Height](/09_glossary.md#camera_height), orientation ([direction](/09_glossary.md#camera_direction)), and [angle](/09_glossary.md#camera_angle) is essential.

::::::

::::::{tab-item} Visual resources
:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_rcsc_et_al_2024 }}
```{figure} ../03_images/03_image_files/rcsc_et_al_2024_detection_probability_2023_05_04_clipped.png
:height: 300px
:align: center
```

**Figure 1.** Three conditional probabilities (Pr) of detection that may impact the detection probability of an animal (or species) by a camera (adapted from Moeller et al. [2023], Hofmeester et al. [2019], and Findlay et al. [2020]).
::::

::::{grid-item-card} {{ ref_intext_rcsc_et_al_2024 }}
```{figure} ../03_images/03_image_files/rcsc_et_al_2024_detectionprob_hofmeester_et_al_2019_fig1_clipped.png 
:width: 300px
:align: center
```
**Figure 2.** Spatial scales (1-6) and processes that determine the detection probability (Hofmeester et al., 2019; abbreviated figure caption).
::::

::::{grid-item-card} {{ ref_intext_tourani_et_al_2020 }}
```{figure} ../03_images/03_image_files/tourani_et_al_2020_fig1.png 
:width: 300px
:align: center
```
NULL
::::

:::::

:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_iknayan_et_al_2014 }}
```{figure} ../03_images/03_image_files/iknayan_et_al_2014_fig2.png 
:width: 300px
:align: center
```
NULL
::::

::::{grid-item-card} {{ ref_intext_oconnell_et_al_2011 }}
```{figure} ../03_images/03_image_files/oconnell_et_al_2011_fig6_1.png 
:width: 300px
:align: center
```
figure5_caption
::::

::::{grid-item-card} {{ ref_intext_findlay_2020 }}
```{figure} ../03_images/03_image_files/findlay_2020_fig1.png
:width: 300px
:align: center
```
figure6_caption
::::
:::::
:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext vid3_ref_id }}
<iframe 
    width="300"
    height="200"
    src="https://www.youtube.com/embed/WBgWOQBlNoI?si=h16_LVMHmwT0ntPd"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

Probability of Detection: Eg 01
::::

::::{grid-item-card} {{ ref_intext vid2_ref_id }} 
<iframe 
    width="300"
    height="200"
    src="vid2_url"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

vid2_caption
::::

::::{grid-item-card} {{ ref_intext vid3_ref_id }}
<iframe 
    width="300"
    height="200"
    src="vid3_url"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

vid3_caption
::::
:::::

:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext vid4_ref_id }} 

<iframe 
    width="300"
    height="200"
    src="vid4_url"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

vid4_caption 
::::

::::{grid-item-card} {{ ref_intext_vid5_ref_id }}

<iframe 
    width="300"
    height="200"
    src="vid5_url"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

vid5_caption
::::

::::{grid-item-card} {{ ref_intext vid6_ref_id }}
<iframe 
    width="300"
    height="200"
    src="vid6_url"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

vid6_caption
::::

:::::

::::::


::::::{tab-item} Shiny apps/Widgets
:::::{card}
**Probabilistic detection calculator (online application) **

Online application used as an aid in sampling planning; calculates the probability of detecting disease (or other similar feature) with the given within-group prevalence and sample size for both finite and infinite group sizes. The detection means that at least one of the samples is detected positive. The sensitivity of the testing method can also be taken into account in the case of an imperfect test. <br><br> Additional information can be found here: <https://zenodo.org/records/13120206>

<iframe 
    width="100%"
    height="900"
    src="https://detcal-shiny.2.rahtiapp.fi/"
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

:::::

::::::

::::::{tab-item} Analytical tools & resources

Error! Not a valid filename.
| R package | detect: analyzing wildlife data with detection error  | The R package implements models to analyze site occupancy and count data models with detection error. The package development was supported by the Alberta Biodiversity Monitoring Institute and the Boreal Avian Modelling (BAM) Project. | 
<https://github.com/psolymos/detect>
<https://peter.solymos.org/detect>
 | {{ ref_bib_solymos_et_al_2024 }} |
| R Shiny app | Probabilistic detection calculator (online application) | Online application used as an aid in sampling planning; calculates the probability of detecting disease (or other similar feature) with the given within-group prevalence and sample size for both finite and infinite group sizes.<br><br> Additional information can be found here: <https://zenodo.org/records/13120206>.  | 
Shiny app: < https://detcal-shiny.2.rahtiapp.fi/>
Related documents: <https://zenodo.org/records/13120206>
 | {{ ref_bib_mikkela_2024 }} |
| resource3_type | resource3_name | resource3_note | resource3_url | {{ ref_bib_resource3_ref_id }} |
| resource4_type | resource4_name | resource4_note | resource4_url | {{ ref_bib_resource4_ref_id }} |
| resource5_type | resource5_name | resource5_note | resource5_url | {{ ref_bib_resource5_ref_id }} |
| resource6_type | resource6_name | resource6_note | resource6_url | {{ ref_bib_resource6_ref_id }} |
| resource7_type | resource7_name | resource7_note | resource7_note | {{ ref_bib_resource7_ref_id }} |
::::::
