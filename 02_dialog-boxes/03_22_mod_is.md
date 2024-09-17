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
(i_mod_is)=
# {{ name_mod_is }}

<!--**{{ name_mod_is }}**
*{{ mod_appl_mod_is }}*<p/>
**{{ term_mod_is }}**: {{ term_def_mod_is }}-->

:::::::::{div} full-width

:::::{dropdown} **Assumptions, Pros, Cons**
::::{grid} 3
:::{grid-item-card} **Assumptions**
- {{ mod_is_assump_01 }}
- {{ mod_is_assump_02 }}
- {{ mod_is_assump_03 }}
- {{ mod_is_assump_03 }}
- {{ mod_is_assump_05 }}
:::
:::{grid-item-card} Pros
- {{ mod_is_pro_01 }}
- {{ mod_is_pro_02 }}
:::
:::{grid-item-card} Cons
- {{ mod_is_con_01 }}
- {{ mod_is_con_02 }}
- {{ mod_is_con_03 }}
:::
::::
:::::

:::::::{tab-set}

::::::{tab-item}Overview

**{{ term_mod_is }}**: {{ term_def_mod_is }}

Overview test here

```{figure} ../03_images/03_image_files/clarke_et_al_2023_eqn_tifc1.png
:width: 80px
:align: center
```

::::::

::::::{tab-item}Advanced

<p>The time in front of the camera (TIFC) model is based on quadrat sampling. Typically, quadrats are used to sample slow- or non-moving organisms at a moment in time; as a simple example, a researcher lays a quadrat on the ground, counts the number of mussels in it and divides the count by the quadrat area. TIFC treats the camera viewshed like a vertical quadrat ({{ ref_intext_becker_et_al_2022 }}; {{ ref_intext_dickie_2022 }}). Unlike a conventional quadrat, however, the camera viewshed samples highly mobile organisms in a relatively small sliver of space and over long periods time ({{ ref_intext_becker_et_al_2022 }}; {{ ref_intext_dickie_2022 }}). The count of animals in the camera viewshed “quadrat,” then, can be thought of in “animal time” and the area covered by the quadrat in “area-time,” such that: </p><br>

```{figure} ../03_images/03_image_files/clarke_et_al_2023_eqn_tifc1.png
:width: 80px
:align: center
```  

*Clarke et al. (2023) - Figure 8*. A) Still from 中島啓裕’s (2021) video series. Example of overlaying a video recording of an animal on a reference image of the focal area (faint triangle) to determine staying time *T*. B) Still from Appendix S2 from Palencia et al. (2021). Example of superimposing the focal area on an image capture.
<br>
<p>where the numerator, animal-time, is the number of animals *N* multiplied by the time those animals spend in the viewshed *T<sub>O</sub>*, summed over all detections; and the denominator, area-time, is the area of the viewshed *A<sub>V</sub>* multiplied by the total camera operating time *T<sub>O</sub>* ({{ ref_intext_becker_et_al_2022 }}). Using this equation, density must be calculated for each species at each camera station, then averaged across the camera network. 

To calculate *A<sub>V</sub>*: in the field, markers (e.g., poles) must be placed at known distances from the camera to divide the viewshed into distance bins; during analysis, the proportion of detections in each bin is determined ({{ ref_intext_becker_et_al_2022 }}). The camera angle of view – which varies with make and model – is also needed to solve for *A<sub>V</sub>*. In most cases, *T<sub>O</sub>* will be the time from initial camera deployment to final camera collection ({{ ref_intext_becker_et_al_2022 }}). In case of displacement, damage or failure, cameras should be programmed to take time-lapse images, so end-of-operation time can be traced back to a specific day or hour ({{ ref_intext_becker_et_al_2022 }}).</p></br>

```{figure} ../03_images/03_image_files/clarke_et_al_2023_fig9_clipped.png
:width: 80px
:align: center
```  
<br>
*Clarke et al. (2023) - Figure 9*. Examples of behaviours that increase time in the viewshed (*𝑇~𝑣~*). A) A mule deer inspects a camera trap. &copy Cole Burton, Wildlife Coexistence Lab. B) A black bear pulls on the lock securing a camera trap to a tree. &copy Michael Procko, Wildlife Coexistence Lab. 
<br>

## Simulations and Field Experiments (Clarke et al., 2023) 
</p>The TIFC model has been field-tested on several different species. For moose, TIFC produced similar density estimates as aerial distance sampling (DS) after TIFC-derived estimates were corrected for the time animals spent investigating equipment (camera and 5 m pole; {{ ref_intext_becker_et_al_2022 }})). This study used image data collected in Alberta at 2,990 camera stations over the course of 6 years; despite the large sample size and long study duration, estimates were not very precise.<br>
<br>
A study of five ungulate species (moose, bison, elk, mule and white-tailed deer) in two enclosed parks in Alberta found that TIFC- and aerial survey-derived density estimates were similar for moose and bison, but that TIFC significantly overestimated elk density compared with aerial surveys ({{ ref_intext_foca_2021 }}). Two potential reasons for the discrepancy in elk density are: 1) that aerial surveys underestimated density, since elk in the study area occupy forested habitats, do not form large herds during the survey period, and estimates were not corrected for sightability; and 2) cameras may have been disproportionately set in areas elk prefer ({{ ref_intext_foca_2021 }}). Group travelling behaviour may also have affected elk TIFC estimates, since detection probability and time in the viewshed (*T<sub>V</sub>*) can change with group size ({{ ref_intext_foca_2021 }}). Estimates of mule and white-tailed deer densities could not be compared with aerial survey results, since deer are not surveyed by air in this area. Foca’s (2021) TIFC analyses produced the first density estimates for deer in both parks.<br>
<br>
In Uganda, TIFC-derived estimates of antelope were comparable to results from camera trap spatial capture-recapture (SCR; {{ ref_intext_brownlee_et_al_2022 }}; {{ ref_intext_warbington_boyce_2020 }}). The model performed inconsistently for black bears, caribou, white-tailed deer and other species, however, compared to camera-based spatial count (SC), DNA markre capture and aerial survey methods (Fisher et al. in review).</p><br>

::::::

::::::{tab-item} Visual resources
:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_clarke_et_al_2023  }}
```{figure} ../03_images/03_image_files/clarke_et_al_2023_eqn_tifc1.png
:width: 100%
:align: center
```

<p>figure1_caption <p/>
::::

::::{grid-item-card} {{ ref_intext_clarke_et_al_2023 }}
```{figure} ../03_images/03_image_files/clarke_et_al_2023_fig9_clipped.png
:width: 100%
:align: center
```

<p>figure2_caption <p/>
::::

::::{grid-item-card} {{ ref_intext_becker_2024 }}
```{figure} ../03_images/03_image_files/becker_2024_slide8.png
:width: 100%
:align: center
```

<p>[FROM MARCUS PPT SLIDE 8; NEED PERMISSION <p/>
::::
:::::

:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_becker_2024 }}
```{figure} ../03_images/03_image_files/becker_2024_slide9a.png
:width: 100%
:align: center
```

<p>FROM MARCUS PPT SLIDE 12; NEED PERMISSION <p/>
::::

::::{grid-item-card} {{ ref_intext_becker_2024 }}
```{figure} ../03_images/03_image_files/becker_2024_slide12.png
:width: 100%
:align: center
```
<p>FROM MARCUS PPT SLIDE 12; NEED PERMISSION<p/>
::::

::::{grid-item-card} {{ ref_intext_figure6_ref_id }}
```{figure} ../03_images/03_image_files/figure6_filename.png
:width: 100%
:align: center
```
<p>figure6_caption <p/>
::::
:::::

:::::{grid} 2
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_becker_2024 }}

<center>
<iframe src="https://drive.google.com/file/d/1IdxQScbzkHd2griu-dEYM4FTFjaXalKe/preview" width="640" height="360" allow="autoplay"></iframe>
</center>

<p>How to estimate density using TIFC; 
Video clip from presentation titled “Comparisons between moose densities with aerial surveys and integrated camera projects”

FROM MARCUS PPT; NEED PERMISSION<p/>
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
:::::
    
:::::{grid} 2
:gutter: 1
:padding: 0
:margin: 0

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
:::::
    
:::::{grid} 2
:gutter: 1
:padding: 0
:margin: 0

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
| resource1_type | Estimating animal density using TIFC (Time In Front of Camera) | resource1_note | <https://github.com/mabecker89/tifc-method> | {{ ref_bib_resource1_ref_id }} |
| resource3_type | Animal Density from Camera Data: Time in the camera field of view | resource3_note | resource3_url | {{ ref_bib_resource2_ref_id }} |
| resource3_type | Animal Density from Camera Data:  | resource3_note | resource3_url | {{ ref_bib_resource3_ref_id }} |
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

{{ ref_bib_becker_et_al_2022 }}

::::::

:::::::

:::::::::