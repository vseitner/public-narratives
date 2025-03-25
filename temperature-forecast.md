------
cover-image: ![Stadt](https://github.com/user-attachments/assets/9825e748-1c21-4cbe-8a3c-b2ea13e2a349) 
------ 
![Stadt](https://github.com/user-attachments/assets/9825e748-1c21-4cbe-8a3c-b2ea13e2a349)
# High-resolution extreme temperature forecasts for cities

Rising temperatures and increasing heat stress pose significant challenges for city population and vegetation, particularly during summer and require urban planners to transform cities into resilient and climate-adapted living spaces. Cities, with built-up areas and extensive sealed surfaces, create heat hotspots, exacerbating thermal discomfort and health risks. Vulnerable groups - such as the elderly, children, and individuals with chronic health conditions - are especially affected, facing an increased risk of heat-related illnesses and mortality. At the same time, fluctuating temperatures drive dynamic energy demands. The growing need for cooling in summer and heating in winter places additional pressure on energy infrastructure, requiring more efficient supply management and forecasting, based on accurate temperature forecasts.

## the challenge
### forecast air temperature on a spatial scale that is representing urban features

Accurate, high-resolution urban weather forecasts are essential for mitigating health risks, optimizing energy distribution, and enhancing overall urban resilience. Unfortunately, current weather forecast models, based on regional-scale meteorological data, lack the spatial resolution necessary to capture the fine-scale temperature variations caused by urban morphology. On a 3-dimensional grid, these models are computing values that are "representative" for each model grid box. What does that mean in practice?
For downtown Vienna, the yellow lines represent the 2.5km model grid 

![Wien_2-5km_Gitter_klein](https://github.com/user-attachments/assets/ac1d4e95-2ab2-4fe2-8b54-c65145228b87)

and this is the temperature forecast for 16th of August 2022, 13UTC for the center grid cell
![t2m_AROME_innerestadt_2020081613](https://github.com/user-attachments/assets/6d1af711-3891-4c64-813f-23ac922fe4f9)
based on GeoSphere Austria's current weather forecast model.

## our solution
### tailor-made high-resolution temperature forecasts for your city

GeoSphere Austria provides the latest technology to forecast urban weather phenomena more detailed than typically available, with a fine spatial scale of 100 meters. Unlike standard weather models, this approach incorporates urban-specific data to deliver detailed forecasts at the district level. For the example of Vienna, this means that you will get that information for the center grid cell
![t2m_25x25_innerestadt_2020081613](https://github.com/user-attachments/assets/277e4db9-0779-4cf5-a666-b5685f0fc696)

This advanced modelling approach can support a wide range of stakeholders, including:

•	**Public authorities** and **crisis managers** to enhance disaster preparedness and response.  
•	**Urban planners** and **policymakers** to design heat-resilient and energy-efficient cities.  
•	**Energy providers** to optimize heating and cooling operations with more precise demand forecasting.

By improving weather information at an urban scale, we empower cities to better adapt to weather and climate extremes.

### workflow

By integrating precise satellite-based data, air temperature (and derived variables) can be calculated on a 100-meter grid to simulate and forecast their spatial and hourly variations providing a database for informed decision-making. The model integrates multiple high-resolution datasets to enhance forecast accuracy:  
›	**Satellite-based land cover data** (e.g., Sentinel-2) to map surface properties and urban structures.  
›	**Building density and surface material analysis** to account for urban heat storage and emission.  
›	**Vegetation and green space influence** to assess cooling effects from parks and tree canopies.  
›	**Anthropogenic heat emissions** from industry and residential heating/cooling.  




### technical features 

|                       |               |
| --------------------- | ------------- |
| spatial gridding      | 100m          |
| temporal gridding     | 1 hour        |
| forecast range        | +30 hours     |
| forecast time         | 00 UTC        |

The model domain is either based on data created by us or based on your data that you can provide from your city.

## use cases

›	Heat-health related high-resolution temperature forecasting    
o	Identification of heat hotspots at a neighbourhood level to detect areas affecting vulnerable groups.  
o	Generation of temperature forecasts for heatwaves and extreme cold events.  
o	Support of urban planning for adaptation strategies (e.g. designing green spaces).  


X

Figure 2:

›	High resolution meteorological information for energy demand forecasting  
o	High-resolution temperature data to optimize district-level heating and cooling supply.  
o	Enhanced demand-side management to improve energy efficiency and reduce peak loads.  

X

Figure 3:

## Available services

1. **Free version:** During project runtime, example forecasts are available for selected Austrian cities. Long term strategy T.B.D. 
2. **Commercial version:** upon request, please contact [Gerhard Wotawa](mailto:gerhard.wotawa@geosphere.at), [Bernhard Niedermoser](mailto:bernhard.niedermoser@geosphere.at)

## Organizational details and legal information

![GSA_Basislogo_Positiv_RGB_XXS](https://github.com/user-attachments/assets/e4a90124-22af-4c13-b659-f91991b36d0d)

Contact points: [Brigitta Hollosi](mailto:brigitta.hollosi@geosphere.at), [Stefan Schneider](mailto:stefan.schneider@geosphere.at)

