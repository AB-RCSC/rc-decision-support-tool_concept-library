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
(i_sp_behav)=
# {{ title_i_sp_behav }}

:::::::::{div} full-width
<!--**{{ title_i_sp_behav }}**-->
:::::::{tab-set}

::::::{tab-item} Overview
<br>
It's important to consider how your Target Species may react to the camera being placed.<br>
While remote cameras are fairly non-invasive survey method, their presence on the landscape, in and of itself, can alter the behaviour of the species you aim to measure (potential attraction to, or avoidance of, the camera), ultimately interfering with detection rates / detection probability ({{ ref_intext_meek_et_al_2014) (e.g., “trap-shy” tigers are thought to avoid cameras due to the white flash emitted ({{ ref_intext_wegge_et_al_2004 }}; {{ ref_intext_sharma_et_al_2010 }}).

Examples of comparable species that can be used to select the most appropriate option:

- **Exploratory**: (e.g., moose, coyote)

- **Neutral**: [INSERT HERE]

- **Avoidant**: (e.g., lynx)

- **I'm not sure**: select this option if you’re not sure of the investigative behaviour of your Target Species (single or multiple species)

- **Variable**: select this option if you’re targeting multiple species and you expect that the investigative behaviour of these species is variable (e.g., you’re targeting coyote and lynx).

::::::

::::::{tab-item} Advanced

Notes for later
- How much sound and illumination (or flash) is emitted will depend on the users’ settings, and the camera make and model (type of flash available; xenon light, white LED or infrared LED illumination). However, the extent to which the camera interferes with behaviour will also depend upon the physical and behavioural characteristics of the species (e.g., perceptive range of hearing, boldness, etc.).
- Many modelling approaches need to incorporate aspects of time as it relates to the animals’ presence at the camera location (e.g., the amount of time spent in the camera’s field-of-view), and thus, you might imagine the bias in the resulting estimates (e.g., density) becomes increasingly problematic for species that are particularly avoidant or exploratory (e.g., moose spend considerable time investigating, which affects effective detection distance in TIFC models; {{ ref_intext_becker_et_al_2022 }}). Such models usually have the assumption that animals’ behaviour is unbiased by the camera.

::::::

::::::{tab-item} Visual resources
:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_meek_et_al_2014b }}
```{figure} ../03_images/03_image_files/meek_et_al_2014_fig11.png
:width: 100%
:align: center
```

<p>**Figure 11.** Comparison of the predicted hearing range of the red fox in relation to the outputs of HC600 camera traps and as a function of frequency <p/>
::::

::::{grid-item-card} {{ ref_intext_becker_et_al_2022 }}
```{figure} ../03_images/03_image_files/becker_et_al_2022_fig4.png
:width: 100%
:align: center
```

<p>NULL <p/>
::::

::::{grid-item-card} {{ ref_intext_figure3_ref_id }}
```{figure} ../03_images/03_image_files/figure3_filename.png
:width: 100%
:align: center
```

<p>figure4_caption <p/>
::::
:::::

:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_figure4_ref_id }}
```{figure} ../03_images/03_image_files/figure4_filename.png
:width: 100%
:align: center
```

<p>figure5_caption <p/>
::::

::::{grid-item-card} {{ ref_intext_figure5_ref_id }}
```{figure} ../03_images/03_image_files/figure5_filename.png
:width: 100%
:align: center
```
<p>figure5_caption<p/>
::::

::::{grid-item-card} {{ ref_intext_figure6_ref_id }}
```{figure} ../03_images/03_image_files/figure6_filename.png
:width: 100%
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
::::::{tab-item} Analytical tools & resources
| Type | Name | Note | URL |Reference |
|:----------------|:---------------------------------------|:----------------------------------------------------------------|:----------------------------------------------------------------|:----------------------------------------------------------------|
| Correction factors (Marcus) | resource1_name | resource1_note | resource1_url | {{ ref_bib_resource1_ref_id }} |
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

::::::{tab-item} *Shiny
Check back in the future!
::::::

::::::{tab-item} References
  
{{ ref_bib_meek_et_al_2014 }}

{{ ref_bib_sharma_et_al_2010 }}

{{ ref_bib_wegge_et_al_2004 }}


 
::::::
:::::::

:::::::::