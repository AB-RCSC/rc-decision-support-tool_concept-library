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
(i_mod_rai)=
# {{ name_mod_rai }}
<!--**{{ name_mod_rai }}**
*{{ mod_appl_mod_rai }}*
**{{ term_mod_rai }}**: {{ term_def_mod_rai }}-->

::::::::::{div} full-width

:::::{dropdown} **Assumptions, Pros, Cons**
::::{grid} 3
:::{grid-item-card} **Assumptions**
- {{ mod_rai_assump_01 }}
:::
:::{grid-item-card} **Pros** 
- {{ mod_rai_pro_01 }}
- {{ mod_rai_pro_02 }}
- {{ mod_rai_pro_03 }}
:::
:::{grid-item-card} **Cons**
- {{ mod_rai_con_01 }}
- {{ mod_rai_con_02 }}
- {{ mod_rai_con_03 }}
:::
::::
:::::

::::::{tab-set}
:selected: true
:::::{tab-item} Overview

**{{ term_mod_rai }}**: {{ term_def_mod_rai }} 
<br/><p>
Add some info here

<p><br/>
:::::
:::::{tab-item} Advanced
<br/><p>
In ecology, relative abundance (RA) is any count of animals or animal sign (e.g., number of deer sighted, number of bird vocalizations per unit time, number of moose tracks per kilometer of transect) that is assumed to correlate with absolute abundance (O’Brien 2011). RA is a controversial index for two reasons: 1) there is often no documented relationship between the number of animals or signs observed and population size (i.e., index validation), and 2) detection probability is assumed to be constant between the areas, times or species being compared (O’Brien 2011, Thompson et al. 1998). <br>
<br>
To the first point: the relationship between the number of animals or signs and abundance is rarely established (Burton et al. 2015). Researchers often assume that counts and population size scale linearly – but many other kinds of relationships are possible. When the assumed relationship between counts and abundance diverges from the actual relationship, inferences from RA are not very meaningful (Thompson et al. 1998). Validating a count-abundance relationship requires comparison with a robust, accurate estimate of absolute density (e.g., Krebs et al. 1987, Rovero and Marshall 2009, Villette et al. 2016). <br>
<br>
To the second point: consider the canonical equation,<br>

```{figure} ../03_images/03_image_files/clarke_et_al_2023_eqn_rai1.png
:width: 80px
:align: center
```  
<br>

where *𝑁* is population size, *𝐶* is the count of animals or signs and *𝑝* is detection probability (Anderson 2001, Brennan 2019). This equation underlies many estimators of abundance, including capture-recapture (CR; see *2.1.1 Capture-Recapture*) and distance sampling (DS; see *2.2.2 Distance Sampling*) methods (O’Brien 2011). RA comparisons assume that detection probability 𝑝 is constant across space, time or species, and can therefore be ignored (Anderson 2001, O’Brien 2011, Sollmann et al. 2013b), such that: 

```{figure} ../03_images/03_image_files/clarke_et_al_2023_eqn_rai2.png
:width: 80px
:align: center
```  
<br>
so count essentially becomes a surrogate for population size. <br>
<br>
Assuming constant detection probability *𝑝* is problematic, since the likelihood an animal or sign is counted during a survey will vary with observational, environmental, and habitat- and species-specific factors, which in turn can vary with time (Anderson, 2001). For example: at site A, animals may be difficult to spot in dense vegetation, while at site B, animals may be easy to spot in open grassland; and the effects of vegetation on observability may differ seasonally. If the effects of vegetation on detectability are not accounted for, how can we be sure that differences in animal counts at site A and B are due to true differences in abundance, and not simply artefacts of detection bias (Sollmann et al., 2013b)? 
In a camera trapping context, RA is the comparison of detection rates across space, time or species – where detection rates are typically reported as the number of images per 100 trap days, but can also be reported in terms of the total number of detections, other units of effort (e.g., camera trap hours), proportion of stations with detections, etc. (Burton et al., 2015). As with other kinds of RA surveys, comparisons of camera trap detection rates can confound abundance with animal behaviour and observability (Anderson 2001, Burton et al. 2015). <br>
<br>
RA has been criticized as an abundance estimator. Anderson (2001) condemned the index as “unprofessional,” while O’Brien (2011) called it a “metric of last resort.” Sollmann et al. (2013b) used simulations to determine that camera trap RA analyses did not detect changes in big cat density, and called use of the index for wildlife management “alarming.” Nevertheless, some researchers have had success with the method and/or have argued for its conceptual and practical advantages (e.g., Carbone et al., 2001, Johnson, 2008, Palmer et al., 2018, Rovero and Marshall 2009). Broadley et al. (2019) used simulations to show that RA could be sensitive to density-dependent movement, but generally tracked abundance well. Banks-Leite (2014) emphasized the importance of careful sampling design and protocols to control for variation in detectability, arguing that researchers should not solely rely on statistical corrections. <br>
<br>
Ultimately, there is no “silver bullet” and researchers must carefully consider their inferential objectives and potential sources of sampling and estimation bias when choosing response variables and modelling frameworks for camera trap data. <br>
<p><br/>
:::::
:::::{tab-item} Visual Resources
:::::{grid} 3
:gutter: 1
::::{grid-item-card}
:header: **{{ ref_intext_figure1_ref_id }}**
```{figure} ../03_images/03_image_files/gilbert_et_al_2019_fig3.png
:height: 200px
:align: center
```
<p>{{ Modified from Gilbert et al., 2021 }}<p/>
::::
::::{grid-item-card}
:header: {{ ref_intext_denes_et_al_2015 }}
:align: center
```{figure} ../03_images/03_image_files/dénes_et_al_2015_fig1.png 
:height: 200px
:align: center
```
<p>{{ dénes_et_al_2015_fig1.png }}<p/>
::::
::::{grid-item-card}
:header: {{ ref_intext_blasco_moreno_2019 }}
```{figure} ../03_images/03_image_files/blasco_moreno_2019_fig1.jpg 
:height: 200px
:align: center
```
<p>{{ blasco_moreno_2019_fig1.jpg }}<p/>
::::
:::::
:::::{grid} 3
:gutter: 1
::::{grid-item-card}
:header: {{ ref_intext_figure4_ref_id }}
```{figure} ../03_images/03_image_files/zi_models_unknown1.png 
:height: 200px
:align: center
```
<p>{{ figure4_caption }}<p/>
::::
::::{grid-item-card}
:header: {{ ref_intext_figure5_ref_id }}
```{figure} ../03_images/03_image_files/zip_models_mindmap.png 
:height: 200px
:align: center
```
<p>{{ https://www.mdpi.com/2673-4591/39/1/38 }}<p/>
::::
::::{grid-item-card}
:header: {{ ref_intext_figure6_ref_id }}
```{figure} ../03_images/03_image_files/figure6_filename.png
:height: 200px
:align: center
```
<p>{{ figure6_caption }}<p/>
::::
:::::
:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0
::::{grid-item-card}
:header: {{ ref_intext vid3_ref_id }}
:padding: 0
:margin: 0
:::{iframe} vid1_url 
:height: 180px
:align: center
:::
<br/><p>{{ vid1_caption }}<p/>
::::
::::{grid-item-card}
:header: {{ ref_intext vid2_ref_id }} 
:::{iframe} vid2_url
:height: 180px
:align: center
:::
<br/><p>{{ vid2_caption }}<p/>
::::
::::{grid-item-card}
:header: {{ ref_intext vid3_ref_id }}
:::{iframe} vid3_url
:height: 180px
:align: center
:::
<br/><p>{{ vid3_caption }}<p/>
::::
:::::
:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0
::::{grid-item-card}
:header: {{ ref_intext vid4_ref_id }} 
:padding: 0
:margin: 0
:::{iframe} vid4_url 
:height: 180px
:align: center
:::
<br/><p>{{ vid4_caption }}<p/>
::::
::::{grid-item-card}
:header: {{ ref_intext_vid5_ref_id }}
:::{iframe} vid5_url
:height: 180px
:align: center
:::
<br/><p>{{ vid5_caption }}<p/>
::::
::::{grid-item-card}
:header: {{ ref_intext vid6_ref_id }}
:::{iframe} vid6_url
:height: 180px
:align: center
:::
<br/><p>{{ vid6_caption }}<p/>
::::
:::::
:::::
:::::{tab-item} Analytical tools & resources

| **Type**       | **Name**       | **Note**       | **URL**       | **ref_id**       |
|----------------|----------------|----------------|---------------|------------------|
| resource1_type | Chapter 6 Modeling Relative Abundance | resource1_note | <https://cornelllabofornithology.github.io/ebird-best-practices/abundance.html> | resource1_ref_id |
| resource2_type | resource2_name | resource2_note | resource2_url | resource2_ref_id |
| resource3_type | resource3_name | resource3_note | resource3_url | resource3_ref_id |
| resource4_type | resource4_name | resource4_note | resource4_url | resource4_ref_id |
| resource5_type | resource5_name | resource5_note | resource5_url | resource5_ref_id |
| resource6_type | resource6_name | resource6_note | resource6_url | resource6_ref_id |
| resource7_type | resource7_name | resource7_note | resource7_url | resource7_ref_id |
:::::
:::::{tab-item} References
<font size="3">
  refs
</font>\
:::::
::::::
::::::::
::::::::::