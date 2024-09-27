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
(i_mod_behaviour)=
# {{ name_mod_behaviour }}

**{{ name_mod_behaviour }}**: {{ term_def_mod_behaviour }}

::::::{dropdown} Assumptions, Pros, Cons
:::::{grid}

::::{grid-item-card} Assumptions
- {{ mod_behaviour_assump_01 }}
- {{ mod_behaviour_assump_02 }}
::::
::::{grid-item-card} Pros
- {{ mod_behaviour_pro_01 }}
- {{ mod_behaviour_pro_02 }}
- {{ mod_behaviour_pro_03 }}
- {{ mod_behaviour_pro_04 }}
::::
::::{grid-item-card} Cons
- {{ mod_behaviour_con_01 }}
- {{ mod_behaviour_con_02 }}
- {{ mod_behaviour_con_03 }}
::::
:::::
::::::

:::::::{tab-set}

::::::{tab-item} Overview
This section will be available soon!

```{figure} ../03_images/03_image_files/00_coming_soon.png
:width: 300px
:align: center
```
::::::

::::::{tab-item} Advanced
This section will be available soon!

```{figure} ../03_images/03_image_files/00_coming_soon.png
:width: 300px
:align: center
```
::::::

::::::{tab-item} Visual resources
:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_caravaggi_et_al_2017 }}
```{figure} ../03_images/03_image_files/caravaggi_et_al_2017_fig1_clipped.png
:class: img_grid
```
**Caravaggi et al. (2017) - Fig. 1.** Examples of animal behaviour captured by camera traps,
:::{dropdown}
(A) Scent marking by an American black bear (*Ursus americanus*); (B) intraspecific competition in moose (*Alces alces*); (C) interspecific interactions between a European hare (*Lepus europaeus*; anti-predator response), a common buzzard (*Buteo buteo*; avoidance and attempted predation) and a hooded crow (*Corvus cornix*; anti-predator behaviour) captured on video (available at 10.6084/m9.figshare.4508369); (D) predation of a European rabbit (*Oryctolagus cuniculus*) by a red fox (*Vulpes vulpes*); (E) investigation of a squirrel feeding station by a pine marten (*Martes martes*); (F) nut caching by a grey squirrel (*Sciurus carolinensis*). Images provided by A.C. Burton (a, b), A. Caravaggi (c, d) and C.M.V. Finlay (e, f).
:::
::::

::::{grid-item-card} {{ ref_intext_caravaggi_et_al_2020 }}
```{figure} ../03_images/03_image_files/caravaggi_et_al_2020_fig1_clipped.png 
:class: img_grid
```
**Caravaggi et al. (2020) - Fig 1.** Examples of mammals detecting camera traps and/or olfactory cues associated with camera traps.
:::{dropdown}
(a) Chimpanzee, *Pan troglodytes*; (b) African elephant, *Loxodonta africana*; (c) sitatunga, *Tragelaphus spekii*; (d) moose, *Alces alces*; (e) Eurasian lynx, *Lynx lynx*; (f) polar bear, *Ursus maritimus*; (g) roe deer, *Capreolus capreolus*; (h) African leopard, *Panthera pardus*; (i) mountain gorilla, *Gorilla beringei*; (j) red fox, *Vulpes vulpes*; (k) wolverine, *Gulo gulo*; (l) grizzly bear, *Ursus arctos*; (m) spotted hyena, *Crocuta crocuta*; (n) red deer, *Cervus elaphus*; (o) grey wolf, *Canis lupus*. Images provided by Ammie K. Kalan (a–c,i), T. R. H. (d,e), D. R. (f,o), S. G. (g,n), A. C. (h,j), J. T. F. (k,l), A. G. (m). Visit <https://doi.org/10.6084/m9.figshare.c.4593902.v1> for selected source video.
:::
::::

:::::

::::::

::::::{tab-item} Shiny apps/Widgets
:::::{card}
**Diel.Niche Shinyapp **

RShiny implementation of Diel.Niche. See Gerber et al. A model-based hypothesis framework to define and estimate the diel niche via the `Diel.Niche' R package.

<iframe 
    width="100%"
    height="900"
    src="https://shiny.uri.edu/bgerber/DielNiche/"
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>
:::::
::::::

::::::{tab-item} Analytical tools & resources

| Type | Name | Note | URL |Reference |
|:----------------|:-------------------------------|:----------------------------------------------------------------|:----------------------|:----------------------------------------|
| Paper | A model-based hypothesis framework to define and estimate the diel niche via the ‘Diel.Niche’ R package |  | <https://www.biorxiv.org/content/10.1101/2023.06.21.545898v1> | {{ ref_bib_gerber_et_al_2023 }} |
| R package | Diel-Niche-Modeling | “An R package to evaluate hypotheses of diel phenotypes based on empirical data and estimate the probabilitiy of activity during the crepuscular, daytime, and nighttime periods.” | <https://github.com/diel-project/Diel-Niche-Modeling> | {{ ref_bib_gerber_et_al_2023 }} |
| R Shiny | Diel.Niche Shinyapp | “RShiny implementation of Diel.Niche. See Gerber et al. A model-based hypothesis framework to define and estimate the diel niche via the `Diel.Niche' R package.” | <https://shiny.celsrs.uri.edu/bgerber/DielNiche/> | {{ ref_bib_gerber_et_al_2023 }} |
| Tutorial | An Introduction to Camera Trap Data Management and Analysis in R > Chapter 14 Behavior |     | <https://bookdown.org/c_w_beirne/wildCo-Data-Analysis/behavior.html> | {{ ref_bib_wildco_lab_2021d }} |
::::::

::::::{tab-item} References
{ ref_bib_caravaggi_et_al_2017 }}

{{ ref_bib_caravaggi_et_al_2020 }}

{{ ref_bib_gerber_et_al_2023 }}

{{ ref_bib_meek_et_al_2014b }}

{{ ref_bib_wildco_lab_2021d }}
::::::

:::::::