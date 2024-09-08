---
jupytext:
  formats: md:myst
  text_reresentation:
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
(i_sp_rarity)=
# {{ title_i_sp_rarity }}

:::::::::{div} full-width
<!--**{{ title_i_sp_rarity }}**-->

:::::::{tab-set}

::::::{tab-item} Overview

**Species rarity categories are defined as follows**:
- **Common**:  probability of occupancy > ~0.75-0.8  (> 0.75 [{{ref_intext_kinnaird_obrien_2012}}; {{ref_intext_kays_et_al_2020}}]; > 0.8 [{{ref_intext_shannon_et_al_2014}}; {{ref_intext_wearn_gloverkapfer_2017}}])
- **Less common**: probability of occupancy 0.25 - 0.75
- **Rare**: probability of occupancy < 0.25 {{ref_intext_kays_et_al_2020}}
- **Very-rare**: probability of occupancy < 0.001 ({{ref_intext_wearn_gloverkapfer_2017}}; {{ref_intext_rowcliffe_et_al_2008}}; {{ref_intext_obrien_2010}})
- **Unknown**: select this option if you’re not sure of the rarity of your Target Species (single or multiple species)
- **Multiple**: select this option if your study includes multiple Target Species that vary in rarity.

**Species rarity** describes how many individuals present of the species, relative to the total number of individuals of all species (or how “represented” is the species when considering the total number of individuals of all species). Generally, species rarity can be thought of as the probability that the species occupies the site, for a given species (or study area, depending on the scale of interest) {{ref_intext_kays_et_al_2020}}. 

While technically “how rare” a species is will be fairly dynamic from place to place (e.g., will depend on geographic range, habitat specificity, local abundance, etc.; {{ref_intext_crisfield_et_al_2024}}), for the purposes of informing study design recommendations, ........

> Species rarity can be generally thought of as a species characteristic, however, “not in the same sense that hair colour or wing venation… it’ an emergent trait of a species' population and its environment rather than a trait of an individual organism” {{ref_intext_kunin_1997}}

::::::

::::::{tab-item} Advanced

Add some info here

::::::

::::::{tab-item} Visual resources
:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_figure1_ref_id  }}
```{figure} ../03_images/03_image_files/figure1_filename.png
:width: 300px
:align: center
```

<p>figure1_caption <p/>
::::

::::{grid-item-card} {{ ref_intext_figure2_ref_id }}
```{figure} ../03_images/03_image_files/figure2_filename.png
:width: 300px
:align: center
```

<p>figure2_caption <p/>
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

::::{grid-item-card} {{ ref_intext_figure4_ref_id }}
```{figure} ../03_images/03_image_files/figure4_filename.png
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
    src="https://www.youtube.com/embed/4gcmAUpo9TU?si=_S-JYDDskR8QbHs5"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

<p>Species accumulation and rarefaction curves<p/>
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
| Type | Name | Note | Reference |
|:----------------|:---------------------------------------|:----------------------------------------------------------------|:----------------------------------------------------------------|
| resource1_type | resource1_name | resource1_note | {{ ref_bib_resource1_ref_id }} |
| resource3_type | resource2_name | resource3_note | {{ ref_bib_resource2_ref_id }} |
| resource3_type | resource3_name | resource3_note | {{ ref_bib_resource3_ref_id }} |
| resource4_type | resource4_name | resource4_note | {{ ref_bib_resource4_ref_id }} |
| resource5_type | resource5_name | resource5_note | {{ ref_bib_resource5_ref_id }} |
| resource6_type | resource6_name | resource6_note | {{ ref_bib_resource6_ref_id }} |
| resource7_type | resource7_name | resource7_note | {{ ref_bib_resource7_ref_id }} |
| resource8_type | resource8_name | resource8_note | {{ ref_bib_resource8_ref_id }} |
| resource9_type | resource9_name | resource9_note | {{ ref_bib_resource9_ref_id }} |
| resource10_type | resource10_name | resource10_note | {{ ref_bib_resource10_ref_id }} |
| resource11_type | resource11_name | resource11_note | {{ ref_bib_resource11_ref_id }} |
::::::
::::::{tab-item} References
{{ ref_bib_chatterjee_et_al_2021 }}

{{ ref_bib_kinnaird_obrien_2012 }}

{{ ref_bib_kays_et_al_2020 }}

{{ ref_bib_shannon_et_al_2014 }}

{{ ref_bib_wearn_gloverkapfer_2017 }}

{{ ref_bib_rowcliffe_et_al_2008)

{{ ref_bib_southwell_et_al_2019 }}

{{ ref_bib_flather_sieg_2007 }}

{{ ref_bib_kunin_1997 }}
::::::

:::::::

:::::::::