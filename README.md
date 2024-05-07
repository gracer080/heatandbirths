# Heat and Adverse Obstetric Outcomes
Project for CYPLAN255

![cyp255 (1)](https://github.com/gracer080/heatandbirths/assets/79069159/cf42e4fb-62c2-404f-9a9d-f874498a35df)

# Introduction
  Climate change remains one of the most existential threats the planet has ever faced, not only threatening our natural world but also undermining decades of public health interventions across the globe. The natural consequences of anthropogenic climate change are leading to increasingly hostile environmental conditions, one of the most pressing of which is rising temperatures. The annual mean global near-surface temperature for the next five years is predicted to be between 1.1°C and 1.8°C higher than the 1850-1900 average[1]. The escalating frequency and severity of heatwaves and ambient temperatures present a substantial threat to overall human health, especially in populations with limited geopolitical or socioeconomic resources for adaptation [2]. This is exemplified by structural phenomena such as the Urban Heat Island effect, which demonstrates how the built environment and population density may further contribute to heat-related mortality, along with altered disease patterns, antibiotic resistance, water and food scarcity [3,4,5].
Emerging evidence establishes a link between heat exposure during pregnancy and adverse obstetric and neonatal outcomes, including preterm birth (PTB), low birth weight, and severe maternal morbidities like eclampsia [6,7]. In 2019, PTB complications were the leading cause of death for children under 5, with over 13 million babies born preterm and incidence rates still rising [8]. Exposure to extreme temperatures during the critical period of 34-37 gestational weeks alters the pulsatility index of the uterine artery, redistributing blood away from the placenta and initiating early labor [9].Much of the research surrounding heat exposure and adverse pregnancy outcomes has been conducted within high-income countries, highlighting inequities in climate research affecting low- and middle-income countries (LMICs).

  LMICs like India bear a disproportionate burden of the climate crisis, with increasing trends in more frequent heatwaves and less variation in temperatures between day and night, putting over 90% of the country at risk for hunger, loss of income, and premature death [10].A 2014 study in Ahmedabad found that heatwaves reaching temperatures of 47.8°C (118°F)  led to increased heat-related hospital admissions of newborns by 43% and more deaths among women overall[11]. Heat exposure also has a degenerative impact on social dynamics. A study found that every 1°C increase in the annual mean temperature was associated with a 4.49% increase in the prevalence of IPV in India, Nepal, and Pakistan [12] .Dual exposures to both increasing temperatures and associated elevated risk of IPV may intersect and exacerbate the risk of PTB, further highlighting women's vulnerability influenced by economic conditions contributing to a loss of income and increased caregiving responsibilities[13].

# Research Questions

What are the various sociodemographic factors that contribute to increased heat exposure and increased risk for adverse obstetric outcomes? How can we construct heat indicies better suited to address the needs of pregnant people?

![cyp255 (3)](https://github.com/gracer080/heatandbirths/assets/79069159/24c216eb-27db-44d6-891b-ff06a6a0b90d)


# Methods

This study examined data from the 2019-2021 DHS survey, which included 724,115 women from India, focusing on their birth histories, sociodemographic information, and health metrics like anemia and BMI, which may serve as coufounders for the outcomes of interest: preterm birth and low birthweight. These outcomes were chosen as proxies for maternal health status as the biological pathways contirbuting to these outcomes slightly differ, allowing for a broader spectrum of possible physiological impacts of thermal stress exposure. The analysis was restricted to 147,084 most recent live singleton births between 2015 and 2019. To merge this demographic data with environmental factors, particularly heat stress, it was crucial that the dataset included precise birth dates and household locations that could access heat stress data from regions covered by the survey (N = 131,682).

For measuring heat stress, the Universal Thermal Climate Index (UTCI) was utilized. This index takes into account a broad range of meteorological conditions along with personal factors like activity levels and clothing, which is essential for assessing thermal stress in various climates. The UTCI values are derived from the High-spatial-resolution Thermal-stress Indices over South and East Asia (HiTiSEA) dataset, which offers detailed, gridded data on several thermal indices calculated from the ECMWF ERA5-Land and ERA5 reanalysis at a fine spatial resolution (0.1°×0.1°). This data set is available via Google Earth Engine, and all spatial analysis was completed utilizing the Python API for Google Earth Engine. 

The linking of the DHS data with the heat stress indices involved using GPS coordinates for each household grouping in the DHS survey, which helped to accurately cross-reference daily maximum and mean UTCI values from the HiTiSEA dataset for each geographic location recorded. This cross-referencing included the daily max and mean UTCI values for the 90-day period preceding each child's birth during the years 2015-2019. This methodological approach allowed for a precise analysis of the impact of maternal heat stress on adverse obstetric outcomes.
![cyp255 (5)](https://github.com/gracer080/heatandbirths/assets/79069159/c54d56c4-a629-4182-a11b-c8d5ef306b7c)

# Results

Descriptive Statistics:


