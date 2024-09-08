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
myst:
  substitutions:
    glossary: "https://ab-rcsc.github.io/rc-decision-support-tool_concept-library/02_dialog-boxes/09_gloss_ref/09_glossary.html"
---
(i_sp_det_prob_cat)=
# {{ title_i_sp_detprob_cat }}

::::::::{div} full-width

:::::::{tab-set}

::::::{tab-item} Overview

**Detection probability categories are defined as follows:**

- **Low**: 
    - < 0.1 ({{ ref_intext_tobler_powell_2013 }})
    - < 0.05 ({{ ref_intext_shannon_et_al_2014 }})
    - 0–0.37 ({{ ref_intext_chatterjee_et_al_2021 }})

- **Medium**: 
    - 0.37–0.67 ({{ ref_intext_chatterjee_et_al_2021 }})

- **High**:
    - 0.67–1 ({{ ref_intext_chatterjee_et_al_2021 }})
    - \> 0.5 ({{ ref_intext_mackenzie_royle_2005 }})

- **Unknown**: select this option if you’re not sure of the detection probability of your Target Species (single or multiple species)

- **Multiple**: select this option if your study include multiple Target Species.

:::{admonition} How this relates to survey design
:class: tip

{{ term_detection_probability }}**: {{ term_def_detection_probability }}

We use this information to adjust the recommended [camera days per camera location](./09_gloss_ref/09_glossary#camera_days_per_camera_location) and [total number of camera days](./09_gloss_ref/09_glossary#total_number_of_camera_days). For example, if the species is hard to detect, you may have to deploy cameras for longer to ensure you’ve sampled long enough to say that the species truly was not there (*vs.* it was there, but you did not detect it; “missed detections”, e.g., high cover of shrubs impeding your ability to see the species).

You may need to consult previous studies to get a sense of which category is the most appropriate for your  

>Select “Unknown” if you’re not sure.
:::

**How does that work?** 

Individuals and/or species are not always detected when they are present (i.e., detected "imperfectly”; MacKenzie et al., 2004). Missed detections occur or many reasons, including due characteristics of the environment (e.g., due to cover of vegetation), the time period (e.g., seasons), characteristics of the species (e.g., cryptic nature or small size), etc. **The question here is asking about detection probability as it relates to the characteristIcs of the species (not the species in a particular habitat type or during a specific season).**

:::{image} ../03_images/03_image_files/det.gif
:width: 400px
:align: center
:::

**Why do we care?**

We care about this because when you fail to detect an individual/species that was, in fact, present, this is called a “false absence”, which may lead to incorrect conclusions from the data. Understanding and correcting for sources of this type of error is often thought of in terms of probabilities (i.e., "detection probability" aka detectability).

:::{admonition} It’s not an exact science
:class: warning

Since detectability is affected by many other processes, detectability is best incorporated from models that use your data since this will result in the best suited infromation to inform your design; however, when you are first designing your study, this is not possible…..\[\[insert more here\]\]
:::

:::{admonition} Analysis aside
:class: seealso
\
Many sources of detection error can be accounted for in analysis; this is done by assessing the relationships between the characteristics of the environment that we might expect to affect detection (e.g., cover of shrubs in front of the camera), and information on where (and when) the species was and was not detected. For example, there were consistently fewer detections on cameras placed in high shrub cover. 

By assessing the relationships at locations repeatedly sampled over time, we begin to unravel the relationship between the environmental characteristics and missed detections on your cameras. We can then use this information to determine if we have sampled long enough (i.e., do we have enough information to differentiate between missed detections and true absences) and/or correct for this error in analysis by incorporating these effects in our models. 
:::

::::::

::::::{tab-item} Advanced
\
Before study design choices are made, there is one critical concept to understand in remote camera research, which may impact study design choices at all levels of the data hierarchy. Reliable use of remote cameras to detect wildlife species hinges on the [assumption](./09_gloss_ref/09_glossary#mods_modelling_assumption) that what is captured on the cameras accurately reflects what is present on the landscape. However, species are often detected "imperfectly," meaning that they are not always detected when they are present (i.e., [imperfect detection](./09_gloss_ref/09_glossary#imperfect_detection); e.g., due to cover of vegetation, cryptic nature or small size) (MacKenzie et al., 2004). [Imperfect detection](./09_gloss_ref/09_glossary#imperfect_detection) can occur because the camera failed to capture an individual present at the site or because the animal was simply not present during the [survey](./09_gloss_ref/09_glossary#survey) period (Martin et al., 2005).

[Imperfect detection](./09_gloss_ref/09_glossary#imperfect_detection) results in “false absences” and may lead to incorrect conclusions from the data. Understanding and correcting for sources of “false absences” is often thought of in terms of probabilities. [Detection probability](./09_gloss_ref/09_glossary#detection_probability) is the probability (likelihood) that an individual from the population of interest is included in the count at time or location *i* (MacKenzie & Kendall, 2002). [Detection probability](./09_gloss_ref/09_glossary#detection_probability) can be influenced through multiple processes and at multiple scales. Understanding the sources of “false absences” and factors that affect [detection probabilities](./09_gloss_ref/09_glossary#detection_probability) is an essential step when designing a study, deploying cameras and analyzing camera data.

The detection probability of an animal by a camera depends on three **conditional probabilities (Pr) of detection** that may operate alone or potentially in combination ([Figure 1](./09_gloss_ref/09_glossary#TOC_surv_guidelines_fig_1)).

(TOC_surv_guidelines_fig_1)=

```{figure} ../03_images/03_image_files/rcsc_et_al_2024_detection_probability_2023_05_04.png
:height: 700px
:align: center
```  

**Figure 1.** Three conditional probabilities (Pr) of detection that may impact the [detection probability](./09_gloss_ref/09_glossary#detection_probability) of an animal (or species) by a camera (adapted from Moeller et al. \[2023\], Hofmeester et al. \[2019\], and Findlay et al. \[2020\]).

Detection probability can be affected by species-specific characteristics, [Camera Model](./09_gloss_ref/09_glossary#camera_model) specifications and set-up, and environmental variables (Hofmeester et al., 2019). For example, **species-specific characteristics** (individuals or populations), such as body size (e.g., O'Brien et al., 2011), behaviour (e.g., Caravaggi et al., 2020; Rowcliffe et al., 2011), and rarity can influence [detection probability](./09_gloss_ref/09_glossary#detection_probability), with larger, bolder and more common species generally having higher [detection rates](./09_gloss_ref/09_glossary#detection_rate). [**Camera Model**](./09_gloss_ref/09_glossary#camera_model), specifications and set-up, such as the [Trigger Sensitivity](./09_gloss_ref/09_glossary#settings_trigger_sensitivity), [**Camera Height**](./09_gloss_ref/09_glossary#camera_height), or [**angle**](./09_gloss_ref/09_glossary#camera_angle) may affect [detection probability](./09_gloss_ref/09_glossary#detection_probability) in that smaller species might not be detected or identifiable if the [Trigger Sensitivity](./09_gloss_ref/09_glossary#settings_trigger_sensitivity) is low, or the [Camera Height](./09_gloss_ref/09_glossary#camera_height) or [angle](./09_gloss_ref/09_glossary#camera_angle) is too high. The [**Camera Direction**](./09_gloss_ref/09_glossary#camera_direction) could impact the probability of an animal triggering a camera if it is directed towards an object that impedes the [Field of View (FOV)](./09_gloss_ref/09_glossary#field_of_view) or image quality (e.g. due to sun glare). **Environmental factors** (e.g., vegetation cover, snow depth) may affect [detection probability](./09_gloss_ref/09_glossary#detection_probability) and occurrence (e.g., Becker et al., 2022; Hofmeester et al., 2019; Iknayan et al., 2014; Steenweg et al., 2019). For example, a low number of detections in a densely vegetated site might be because of poor camera visibility or avoidance of this habitat by the species of interest.

Hofmeester et al. (2019) suggested there are **six scales (orders) that may impact [detection probability](./09_gloss_ref/09_glossary#detection_probability)** and that should be considered within an explicit time period (adapted from Hofmeester et al. \[2019\]; [Figure 2](./09_gloss_ref/09_glossary#TOC_surv_guidelines_fig_2)):

1)  **Distribution range** (1st order; i.e., the physical or geographical range of a species)

2)  **Landscape** (2nd order; i.e., the location of an individual’s home range within the geographic range)

3)  **Habitat patch** (3rd order; i.e., usage of habitat components within an individual’s home range)

4)  **Microsite** (4th order; usage of microhabitats such as food items/feeding patches/nest sites/movement trails, etc. within a habitat)

5)  **Camera specification / set-up** (5th order; i.e., factors that affect the probability that an animal [triggers](./09_gloss_ref/09_glossary#trigger_event) the camera if present)

6)  **Image** (6th order; i.e., factors that affect correct identification of animals or individuals)

(TOC_surv_guidelines_fig_2)=

```{figure} ../03_images/03_image_files/rcsc_et_al_2024_detectionprob_hofmeester_et_al_2019_fig1.png
:scale: 70%
:align: center
```  

**Figure 2.** Spatial scales (1-6) and processes that determine the [detection probability](./09_gloss_ref/09_glossary#detection_probability) (Hofmeester et al., 2019; abbreviated figure caption).

It is important to consider how all these factors and scales will impact study design. Unmeasured variation in [detection probability](./09_gloss_ref/09_glossary#detection_probability) can result in the inability to differentiate the effects of [detection probability](./09_gloss_ref/09_glossary#detection_probability) *vs.* habitat preference (Jennelle et al., 2002) and, in turn, cause erroneous estimates of occurrence and abundance (Burton et al., 2015; Dénes et al., 2015; Kays et al., 2021).

Factors that influence [detection probability](./09_gloss_ref/09_glossary#detection_probability) at the microsite and camera specification / set-up scales are likely to result in the largest biases and thus warrant the most consideration (see Hofmeester et al. \[2019\] for details). Therefore, it is particularly important to consider *how* to place cameras to avoid such biases. Deploying cameras in a consistent fashion (e.g., carefully ensuring that cameras are always set at the same [Camera Height](./09_gloss_ref/09_glossary#camera_height), orientation ([direction](./09_gloss_ref/09_glossary#camera_direction)), and [angle](./09_gloss_ref/09_glossary#camera_angle) is essential.

::::::

::::::{tab-item} Visual resources
:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_rcsc_et_al_2024 }}
```{figure} ../03_images/03_image_files/rcsc_et_al_2024_detection_probability_2023_05_04.png
:width: 300px
:align: center
```

::::

::::{grid-item-card} {{ ref_intext_rcsc_et_al_2024 }}
```{figure} ../03_images/03_image_files/rcsc_et_al_2024_detectionprob_hofmeester_et_al_2019_fig1.png
:width: 300px
:align: center
```

::::

::::{grid-item-card} {{ ref_intext_tourani_et_al_2020 }}
```{figure} ../03_images/03_image_files/tourani_et_al_2020_fig1.png
:width: 300px
:align: center
```

<p>NULL <p/>
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

<p>figure5_caption <p/>
::::

::::{grid-item-card} {{ ref_intext_figure5_ref_id }}
```{figure} ../03_images/03_image_files/figure5_filename.png
:width: 300px
:align: center
```
<p>figure5_caption<p/>
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

::::{grid-item-card} {{ ref_intext_vid1_ref_id }}

<iframe 
    width="300"
    height="200"
    src="vid1_url"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

<p>vid1_caption<p/>
::::

::::{grid-item-card} {{ ref_intext_vid2_ref_id }}

<iframe 
    width="300"
    height="200"
    src="vid2_url"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

<p>vid2_caption<p/>
::::

::::{grid-item-card} {{ ref_intext_vid3_ref_id }}

<iframe 
    width="300"
    height="200"
    src="vid3_url"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

<p>vid3_caption<p/>
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
    src="vid4_url"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

<p>vid4_caption<p/>
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

<p>vid5_caption<p/>
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

<p>vid6_caption<p/>
::::

:::::

::::::

::::::{tab-item} Shiny apps/Widgets
Check back in the future!
::::::

::::::{tab-item} Analytical tools & resources
| Type | Name | Note | URL |Reference |
|:----------------|:---------------------------------------|:----------------------------------------------------------------|:----------------------------------------------------------------|:----------------------------------------------------------------|
| resource1_type | resource1_name | R package for analyzing wildlife data with detection error | <https://github.com/psolymos/detect><br><https://peter.solymos.org/detect> | {{ ref_bib_resource1_ref_id }} |
| resource3_type | resource2_name | resource3_note | resource3_url | {{ ref_bib_resource2_ref_id }} |
| resource3_type | resource3_name | resource3_note | resource3_url | {{ ref_bib_resource3_ref_id }} |
| resource4_type | resource4_name | resource4_note | resource4_url | {{ ref_bib_resource4_ref_id }} |
| resource5_type | resource5_name | resource5_note | resource5_url | {{ ref_bib_resource5_ref_id }} |
| resource6_type | resource6_name | resource6_note | resource6_url | {{ ref_bib_resource6_ref_id }} |
| resource7_type | resource7_name | resource7_note | resource7_url | {{ ref_bib_resource7_ref_id }} |
| resource8_type | resource8_name | resource8_note | resource8_url | {{ ref_bib_resource8_ref_id }} |
| resource9_type | resource9_name | resource9_note | resource9_url | {{ ref_bib_resource9_ref_id }} |
| resource10_type | resource10_name | resource10_note | resource10_url | {{ ref_bib_resource10_ref_id }} |
| resource11_type | resource11_name | resource11_note | resource11_url | {{ ref_bib_resource11_ref_id }} |
::::::

::::::{tab-item} References
{{ ref_bib_rcsc_et_al_2024 }} 

{{ ref_bib_chatterjee_et_al_2021 }}

{{ ref_bib_mackenzie_kendall_2002 }}

{{ ref_bib_mackenzie_royle_2005 }}

{{ ref_bib_shannon_et_al_2014 }}

{{ ref_bib_tobler_powell, 2013 }}

{{ ref_bib_mackenzie_kendall_2002 }}

{{ ref_bib_mackenzie_royle_2005 }} 
::::::

:::::::

::::::::