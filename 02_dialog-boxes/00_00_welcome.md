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
(#toc_welcome)=
# Welcome to the Remote Camera Decision Support Tool! 
:::::::::{div} full-width
A free, online, interactive, visual study decision support system for remote camera projects
<br>

## How does it work!? 
This tool aims to support your decision-making process when designing a remote camera programs by guiding you through a series of decision points related to your study in the form of an interactive flow chart.
At each step, you will be able to access information related to the question in the “info popups”; information is provided with different levels of complexity (overview vs. advanced) and in formats that accommodate multiple learning styles (e.g., figures, videos, Shiny apps, etc.). Once you have answered all of the questions, study design recommendations will be generated from your selections, which will include the following:

:::{important} Appropriate modelling approach(es)
:class: dropdown

- **Species inventory** (Species inventory, presence)
- **Species diversity & richness**
    -   *\[FUTURE\]* Species diversity & richness \- Alpha richness (α)
    -   *\[FUTURE\]* Species diversity & richness \- Gamma richness (γ)
    -   *\[FUTURE\]* Species diversity & richness \- Beta-diversity (β)
    -   Occupancy (Occupancy / Species distribution)
- **Relative abundance indices**
    -   *\[FUTURE\]* Relative abundance indices \- Poisson
    -   *\[FUTURE\]* Relative abundance indices \- Zero-inflated poisson (ZIP)
    -   *\[FUTURE\]* Relative abundance indices \- Negative binomial (NB)
    -   *\[FUTURE\]* Relative abundance indices \- Zero-inflated negative binomial (ZINB)
    -   *\[FUTURE\]* Relative abundance indices \- Hurdle
- **Capture-recapture (CR) / Capture-mark-recapture (CMR)**
- **Spatial capture-recapture (SCR) / Spatially explicit capture recapture (SECR)**
- **Spatial mark-resight (SMR)**
- **Spatial count (SC) model / Unmarked spatial capture-recapture**
- **Spatial Partial Identity Model (Categorical SPIM; catSPIM)**
- **Spatial Partial Identity Model (2-flank SPIM)**
    -   *\[FUTURE\]* Royle-Nichols
    -   *\[FUTURE\]* N-mixture
- **Random encounter model (REM)**
- **Random encounter and staying time (REST)**
- **Time in front of the camera (TIFC)**
- **Distance sampling (DS)**
- **Time-to-event (TTE)**
- **Space-to-event (STE)**
- **Instantaneous sampling (IS)**
- **Behaviour**
    -   *\[FUTURE\]* More specific approaches related to behaviour
:::

:::{admonition} Sampling design
:class: important

Relevant to the appropriate modelling approach(es) identified
- Camera arrangement
- Camera spacing
- Number of camera days per camera location
- Number of cameras
- Survey duration
- Total number of camera days
:::

:::{admonition} Analysis considerations
:class: important

(e.g., variables to consider in your analysis to reduce bias)
:::

:::{admonition} It’s not an exact science
:class: warning
CAVEATS HERE / it's not perfect (or some other text here along these lines)
::::

::::::{dropdown} Information formats

Information is available in the following tabs of the "info pop-ups":
- **Overview** \- short, digestible information about the topic
- **Advanced** \- more “in the weeds” information for those who want to dig into the details
- **Visual resources** \- related figures and videos; you can watch videos within in tool itself, or 
- **Analytical tools & resources** \- resources for implementing analyses.
- **Executable Code** \- 
- **Shiny apps (if available)** \-
    -   **Integration of data/apps** - Currently, the integration of other apps such as Shiny app is limited to "illustrative" apps (integration of apps or tools for the purpose of illustrating a concept vs. attempting to incorporate simulated information into recommendations), with the exception of the (ADD INFO OCCUPANCY APP)
- **References** \- references for all of the content in this section

:::{note}
Information include in the info popups is always available in the **[Concept Library]( https://ab-rcsc.github.io/rc-decision-support-tool_concept-library/)**
:::
::::::

::::::{dropdown} 🚀 Future development
\
In addition to the modelling approaches mentioned above as \[FUTURE\]....

<!--
:::{dropdown} Illustrative vs. data-simulation app-integration
- **ILLUSTRATIVE app-integration**: integration of apps or tools for the sole purpose of illustrating a concept. The user may be able to toggle or adjust values (e.g., select for different camera configurations, spacing, or # of land cover types to see how these factors influence the layout of cameras), but these inputs/choices do not inform other parts of the decision-making process, tool, or resulting recommendations (i.e., once the app is closed, it’s like nothing ever happened).
- **DATA-SIMULATION app-integration**: integration of apps or tools for the purpose of performing calculations based on user inputs (e.g., ) that will inform other parts of the decision-making process, tool, and/or resulting recommendations
:::
-->
::::::


# Questions?
If you have questions or would like further information, please contact Cassie Stevenson, Alberta Remote Camera Steering Committee (RCSC) / Alberta Biodiversity Monitoring Institute (ABMI), <abwildlifecameras@gmail.com>; <cjsteven@ualberta.ca>.

***

:::::{grid} 5
:gutter: 1

::::{grid-item}
:::{image} ../03_images/02_logos/aca_ed.png
:align: center
:::
::::

::::{grid-item}
:::{image} ../03_images/02_logos/abgov_ed.png
:align: center
:::

::::

::::{grid-item}
:::{image} ../03_images/02_logos/eccc_ed.png
:align: center
:::

::::

::::{grid-item} 
:::{image} ../03_images/02_logos/fos_ed.png
:align: center
:::
::::

::::{grid-item} 
:::{image} ../03_images/02_logos/abmi_ed.png
:align: center
:::
::::
:::::

***

*This project was funded by the Alberta Conservation Association (ACA)m the Office of the Chief Scientist (OCS), and Environment and Climate Change Canada (ECCC). This project was provided in-kind support by the Alberta Remote Camera Steering Committee (RCSC), Alberta Environment and Protection Areas (EPA), Alberta Biodiversity Monitoring Institute (ABMI), and the University of Alberta Faculty of Science.*
:::::::::