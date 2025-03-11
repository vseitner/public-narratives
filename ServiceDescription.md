# Heat Risk Maps

## Problem & Needs
## List <!--{ as="div" }-->
- Heat extremes at daytime and no cooling at nighttime: climate change poses a rising threat to urban life. Austria’s cities experienced almost a tripling of heat days and tropical nights – with the trend still increasing.
- Exposure to heat causes significant stress on humans – especially for vulnerable groups, like children or elderly, the health consequences of prolonged exposure are serious.
- High population densities and the urban heat island effect force cities to adapt and take action to tackle the rising threat. But adaptation measures are often only locally effective, and funds are limited.
- The pressing question is: where to act? Where are heat-reducing measures the most effective to protect vulnerable groups? 
- … and where to start? Which adaption measures should be prioritized due to the risk at hand?
- Not only is this an acute concern for cities and municipalities, but also for companies and organizations required to assess future heat risks.
- This highlights the need for heat risk maps, which take vulnerable groups into account and effectively locate high risk areas.



## Solution Capability
Risk – based on the IPCC definition – is a combination of hazard, exposure, and vulnerability. Well-founded risk assessment is the first step to locate measures where needed, shape future developments, and direct impactful investments. Various data from different disciplines need to be comprehensively compiled and connected. But how to combine the available information in a meaningful way and create scientifically sound heat risk maps? 
The developed heat-risk-algorithm merges state-of-the-art satellite information, like building structure, degree of soil sealing or tree cover, with population statistics, as well as high-resolution climate data tailored to Austria. The blend of open-source data with important area-specific datasets does not only allow to create customized heat risk maps for a selected city or municipality, but also ensures high quality and reliable results. The methodology allows the heat risk maps to be calculated regularly when new or updated datasets are available, making the effects of adaptation measures and urban development visible. It also offers the possibility to incorporate future spatial planning scenarios or demographic developments and helps to anticipate future impacts. The aim of the heat risk map is to present the information visually and in an easy-to-understand manner making the maps universally applicable for a wide range of use-cases.

## Use-case examples
## Use-case examples <!--{ as="div" }-->

-	Heat action and heat protection plans: Integration of heat risk maps can support to tailor actions to the areas at risk.
-	Urban development concepts: Heat Risk Maps provide valuable information to spatial development and city planners in making their city liveable for the future.
-	Prioritization of adaptation measures: The heat risk concept allows to compare areas within cities and quantify adaptation measures customized to high-risk places.
-	Update current heat risk information: Changing climate conditions, development of urban areas and changed population statistics make outdated maps unusable. The developed algorithm allows updates on the fly.
-	Finding locations with future risks: Organizations and companies dealing with vulnerable groups, can identify locations with high or low current and future heat risk, which is crucial for planning operation centres and deployments.

## Benefits of Heat Risk Maps within GTIF
1.	Update frequency: HRM are not a single product or service, but can be updated if relevant input data changes (e.g. building stock, population density, updated climate models)
2.	Consistency: HRM use VDI conformal urban climate analysis and can thus either incorporate already available data or provide climatope information by the algorithm itself.
3.	Data availability: HRM uses open-source data that can easily be replaced if higher quality datasets are available.

## Heat Risk Maps
## Heat Risk Maps <!--{ as="div" }-->
- Target resolution: 50-250 m (any)
- The data sources in detail:
  -	Population density and age structure
  -	Building stock
  - Land use data from Copernicus (Earth observation component of the European Union Space Programme)
  - Latest high-resolution climate scenarios (CMIP6 downscaled)


## Map Tour <!--{ as="eox-map" mode="tour" }-->

### <!--{ layers='[{"type":"Tile","properties":{"id":"osm"},"source":{"type":"OSM"}}]' center=[15,48] zoom="5" animationOptions="{duration:500}" }-->
#### INTERACTIVE MAP ILLUSTRATION (TBD)
 Satellite image is gradually overlaid with data layers (3 layers) so that the risk is mapped with higher resolution bit by bit. 


## HRM APIs
The HRM map is delivered via two different Application Programming Interfaces (APIs): (1) the OGC Web Map Service (WMS), a Web-standard portrayal and streaming interface for cascaded integration into widely used Geographical Information Systems such as QGIS, and (2) a RESTful machine-to-machine (M2M) API for integration with special end-user IT environments. Both APIs will be access-controlled for an authorized group of users.

CHARACTERIZATION RESTful API: [...]

## WebGIS Visualization
The WebGIS will be access-controlled for an authorized group of users.

WEBGUI ILLUSTRATION:  [...]

## Download
HRM Maps can also be offered for download as files from an access controlled sFTP Server as GeoPackage (GPKG), an open, non-proprietary, platform-independent standard, building on existing standards, for storing geospatial data (vector and raster data) in a file. 

## Delivery Process
The delivery process for the HRM Capability involving Customer and Provider(s) is shown in the following workflow.





# Workflow <!--{ as="img" data-fallback-src="https://raw.githubusercontent.com/Itsman-AT/public-narratives/Itsman-AT/heat-risk-according-to-climate-scenarios/assets/Itsman-AT/workflow-1741688297522.jpg" mode="hero" src="https://raw.githubusercontent.com/GTIF-Austria/public-narratives/625e1f41a907e0b7106d307d2d60d805bee47c9f/assets/workflow-1741688297522.jpg" }-->
### by AIT <!--{ style="font-size:1rem;opacity:0.7;margin-top:1rem;" }-->


## About: Provider Entities
The following entities are, or may be, involved in the provision of the HRM Capability:

AIT - Austrian Institute of Technology (Center for Energy/DRC)
- The HRM Model is a copyright of AIT. The model is closed source.
- AIT may be engaged commercially to provide further HRM Models optimized to other AoI based on Customer-provided in-situ - contact [XXX]
