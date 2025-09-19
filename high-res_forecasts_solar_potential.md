---
cover-image: https://raw.githubusercontent.com/triebnigg/public-narratives/triebnigg/evapotranspiration-monitoring-2/assets/triebnigg/solar-potential-1749907032353.webp
domain: Energy Transition
tags:  photovolatic, remote sensing, STRAHLGRID

---

# High-resolution Forecasts of Solar Potential

High quality data on solar radiation is an essential input for a wide range of applications in the context of energy and mobility transitions, sustainable energy planning and climate change adaption.<br>
These solar potential forecasts offer significant benefits for energy management and grid stability. Forecasted radiation data can enable predictive control of heat pumps and thermal storage systems, improve conditions for selling surplus energy and support better planning for electric vehicle charging. The 30-hour forecasts also contribute to grid stability by allowing for the regulation of PV peaks through other power plants or supplementary loads. In the long term, this information could also enhance transaction optimization at electricity markets.<br>
Furthermore, warnings can be developed and integrated to notify when a covering layer (such as snow or dust) is likely to affect the PV performance.

## Product description

The starting point for calculating the solar potential is the GeoSphere Austria radiation model *STRAHLGRID*. *STRAHLGRID* calculates direct and diffuse radiation (and their sum, global radiation) on horizontal and real surfaces in the spectral range of 0.3 to 3 µm. The model accounts for atmospheric turbidity effects (e.g. water vapor and aerosols), cloud cover and horizon shading. The cloud parametrization is derived from the calibration of satellite cloud data with ground based radiation measurements. For the calculations, a high-quality digital elevation model is used to account for topographic effects, alongside meteorological input data (integrated water vapor content, air pressure and cloud cover) to adress atmospheric effects. For the meteorological input data, forecast data from AROME/INCA is used as initial data. 

![infodienst_solar_step1](https://github.com/user-attachments/assets/d85df220-58a1-400d-9faa-bbcb1cd1e664)

_Fig 1: Example output of global solar radiation from *STRAHLGRID*. 1300 UTC of an arbitrary day._

![infodienst_solar_step2](https://github.com/user-attachments/assets/04db3bc8-5907-4b3c-8cfd-250d26366a81)
_Fig 2: Example output of global solar radiation from *STRAHLGRID*. 1400 UTC of an arbitrary day._ 

The output of this radiation model is then going to be converted into solar power generation potential by the method of *Jerez et al (2015)*.  The output is the potential for the generated power. To obtain the power at the installed system, this value must be multiplied by the nominal installed watts.

![infodienst_solar_potential_step1](https://github.com/user-attachments/assets/dcf92c00-ab12-46e0-b433-601469fb58d7)
_Fig 3: Example output of solar potential. 1300 UTC of an arbitrary day._

![infodienst_solar_potential_step2](https://github.com/user-attachments/assets/5e93041a-39d0-4d48-9469-5c1a86939032)
_Fig 4: Example output of solar potential. 1400 UTC of an arbitrary day._

And addiation feature of this product is, that not only the solar potential can be calculated, but also warnings on snow and dust covers can be provided. These warnings are genereted through the integration of GeoSphere Austria's operational snow model *SNOWGRID*, and dust forecasts from *WRF-Chem*.

## Technical features

|                       |               |
| --------------------- | -------------: |
| spatial resolution    | 100(0) m         |
| temporal resolution   | 1 hour        |
| forecast range        | +30 hours     |
| forecast time         | 00 UTC        |
| snow cover            | yes/no        |
| dust cover      | yes/no              |

The model chain for Austria is implemented as default. The model can be adapted to other regions with some additional effort. 

# Offene Fragen...

* Welche Vorhersagedauer ist relevant?
* Wann wird die Information benötigt? (Immer zu speziellen Uhrzeiten oder zB verstärkt in der Früh?)
* In welcher Form ist die Information von Intersse? (In der Fläche? Als Zeitreihen?)
* Sind Vergleiche mit einer Klimatologie relevant? (zB Hab ich morgen mehr als im langjährigen Mittel?)


# Organizational details and contact

![GSA_Basislogo_Positiv_RGB_XXS](https://github.com/user-attachments/assets/e4a90124-22af-4c13-b659-f91991b36d0d)

**Contact**: [APOLIS-Team](mailto:apolis@geosphere.at)

## Available services

* **Free Version** <br>
Example forecasts for selected Austrian cities during project runtime. Long term strategy TBD.
* **Commercial Service**<br>
Service on demand. Please contact: Kundenservice GeoSphere Austria

# References

1. [Goebel et al, 2022 - Development of a very high resolution solar radiation cadaster for estimating solar energy potential across the entire federal state of Salzburg, Austria](https://doi.org/10.5194/ems2022-396)
2. [Seitner et al, 2024 - STRAHLGRID: A solar radiation model with applications across different spatial scales](https://doi.org/10.5194/ems2024-366)
3. [Jerez et al, 2015 - The impact of climate change on photovoltaic power generation in Europe](https://www.nature.com/articles/ncomms10014)
4. Publication of model algorithm in progress. 
