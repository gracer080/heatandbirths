# Heat and Adverse Obstetric Outcomes
Project for CYPLAN255

# Interactive Heat Stress Vulnerability Index Map For Pregnant People (India)
Click to check out the [Heat Vulnerability Index for Pregnant People Interactive Map](interactive_map2.html) to explore the associations between extreme heat and adverse obstetric outcomes in India.


<img width="1509" alt="Screenshot 2024-05-06 at 10 01 15 PM" src="https://github.com/gracer080/heatandbirths/assets/79069159/ffbf363e-1826-45f9-a68a-94af3bd5fb77">



![cyp255 (1)](https://github.com/gracer080/heatandbirths/assets/79069159/cf42e4fb-62c2-404f-9a9d-f874498a35df)



# Introduction
  Climate change remains one of the most existential threats the planet has ever faced, not only threatening our natural world but also undermining decades of public health interventions across the globe. The natural consequences of anthropogenic climate change are leading to increasingly hostile environmental conditions, one of the most pressing of which is rising temperatures. The annual mean global near-surface temperature for the next five years is predicted to be between 1.1°C and 1.8°C higher than the 1850-1900 average[1]. The escalating frequency and severity of heatwaves and ambient temperatures present a substantial threat to overall human health, especially in populations with limited geopolitical or socioeconomic resources for adaptation [2]. This is exemplified by structural phenomena such as the Urban Heat Island effect, which demonstrates how the built environment and population density may further contribute to heat-related mortality, along with altered disease patterns, antibiotic resistance, water and food scarcity [3,4,5].
Emerging evidence establishes a link between heat exposure during pregnancy and adverse obstetric and neonatal outcomes, including preterm birth (PTB), low birth weight, and severe maternal morbidities like eclampsia [6,7]. In 2019, PTB complications were the leading cause of death for children under 5, with over 13 million babies born preterm and incidence rates still rising [8]. Exposure to extreme temperatures during the critical period of 34-37 gestational weeks alters the pulsatility index of the uterine artery, redistributing blood away from the placenta and initiating early labor [9].Much of the research surrounding heat exposure and adverse pregnancy outcomes has been conducted within high-income countries, highlighting inequities in climate research affecting low- and middle-income countries (LMICs).

  LMICs like India bear a disproportionate burden of the climate crisis, with increasing trends in more frequent heatwaves and less variation in temperatures between day and night, putting over 90% of the country at risk for hunger, loss of income, and premature death [10].A 2014 study in Ahmedabad found that heatwaves reaching temperatures of 47.8°C (118°F)  led to increased heat-related hospital admissions of newborns by 43% and more deaths among women overall[11]. Heat exposure also has a degenerative impact on social dynamics. A study found that every 1°C increase in the annual mean temperature was associated with a 4.49% increase in the prevalence of IPV in India, Nepal, and Pakistan [12] .Dual exposures to both increasing temperatures and associated elevated risk of IPV may intersect and exacerbate the risk of PTB, further highlighting women's vulnerability influenced by economic conditions contributing to a loss of income and increased caregiving responsibilities[13].

# Research Questions

What are the various sociodemographic factors that contribute to increased heat exposure and increased risk for adverse obstetric outcomes? How can we construct heat indicies better suited to address the needs of pregnant people?

![cyp255 (3)](https://github.com/gracer080/heatandbirths/assets/79069159/24c216eb-27db-44d6-891b-ff06a6a0b90d)


# Methods

This study examined data from the 2019-2021 DHS survey [14], which included 724,115 women from India, focusing on their birth histories, sociodemographic information, and health metrics like anemia and BMI, which may serve as coufounders for the outcomes of interest: preterm birth and low birthweight. All DHS surveys are representative on the district, state, and national level.  These outcomes were chosen as proxies for maternal health status as the biological pathways contirbuting to these outcomes slightly differ, allowing for a broader spectrum of possible physiological impacts of thermal stress exposure. The analysis was restricted to 147,084 most recent live singleton births between 2015 and 2019. To merge this demographic data with environmental factors, particularly heat stress, it was crucial that the dataset included precise birth dates and household locations that could access heat stress data from regions covered by the survey (N = 131,682).

For measuring heat stress, the Universal Thermal Climate Index (UTCI) was utilized. This index takes into account a broad range of meteorological conditions along with personal factors like activity levels and clothing, which is essential for assessing thermal stress in various climates. The UTCI values are derived from the High-spatial-resolution Thermal-stress Indices over South and East Asia (HiTiSEA) dataset [15], which offers detailed, gridded data on several thermal indices calculated from the ECMWF ERA5-Land and ERA5 reanalysis at a fine spatial resolution (0.1°×0.1°). This data set is available via Google Earth Engine, and all spatial analysis was completed utilizing the Python API for Google Earth Engine. 

The linking of the DHS data with the heat stress indices involved using GPS coordinates for each household grouping in the DHS survey, which helped to accurately cross-reference daily maximum and mean UTCI values from the HiTiSEA dataset for each geographic location recorded. This cross-referencing included the daily max and mean UTCI values for the 90-day period preceding each child's birth during the years 2015-2019. This methodological approach allowed for a precise analysis of the impact of maternal heat stress on adverse obstetric outcomes.
![cyp255 (5)](https://github.com/gracer080/heatandbirths/assets/79069159/c54d56c4-a629-4182-a11b-c8d5ef306b7c)

# Results

Descriptive Statistics:

The sociodemographic profile of the selected mothers predominantly falls within the age range of 20-25 years at birth. A substantial portion of these women have achieved at least a primary level of education, with the majority having secondary education. Most women (93.49%) accessed antenatal care services during their pregnancies. Regarding caste, 22% of the women belong to a scheduled caste, while smaller percentages belong to scheduled tribes (9.8%) and other backward castes (43%). The study also highlights a significant rural representation, with 72.9% of participants residing in rural areas. In terms of economic status, the distribution across wealth quintiles shows a considerable number of women in the lower economic brackets. Anthropometric data indicates that 58% of the women fall within the 'healthy weight' BMI category of 18.5-24.9. Additionally, biomarker data on hemoglobin levels shows that over half of the women (56.1%) were diagnosed as anemic, with conditions ranging from mild to severe. All these percentages were calculated using survey weights to accurately reflect the broader population’s characteristics.

![cyp255 (9)](https://github.com/gracer080/heatandbirths/assets/79069159/d84bae60-5e78-463e-8af9-2f9aeee6dc52)


When examining the distribution of health outcomes across the study population, it was found that approximately 13% of the participants experienced preterm births, while around 25% of the newborns were classified as having low birth weight. These figures align closely with existing population-level estimates, suggesting that the sample is representative of adverse obstetric outcomes. 

![cyp255 (7)](https://github.com/gracer080/heatandbirths/assets/79069159/14f2b216-3502-47c1-8e79-384fc7f9a72a)

Constructing Heat Stress Vulnerability Index for Pregnant People:

![cyp255 (11)](https://github.com/gracer080/heatandbirths/assets/79069159/cf6c33f6-5845-4a72-9222-23f5f5d1a1a2)

Bivariate analysis was conducted using the chi-squared test, F statistics, and Rao-Scott adjustment to determine which sociodemographic factors are significantly associated with the outcomes of interest and varying levels of heat exposure categorized as low, medium, and high. The analysis revealed that younger individuals, those with no education, lower wealth quintiles, rural residents, members of historically disadvantaged castes, and those without prenatal care were significantly associated with higher heat exposure and an increased risk of preterm birth and low birth weight. These findings informed the creation of a heat vulnerability index for pregnant individuals. This index, ranging from 1 to 5, scores higher for individuals with multiple sociodemographic risk factors and living in regions with historically higher temperatures. Those with a combination of these risk factors scored 5, indicating higher vulnerability, while those with fewer associated characteristics and lower heat exposure scored 1, indicating lower vulnerability.

Creating the Interactive Map:

The map was created by first loading heat stress data from HiTiSEA for each individual in the DHS data set into GeoDataFrames with  GeoPandas. This data included district level information on sociodemogrpahic factors and heat stress exposure which was then aggregated and visualized using Folium. Districts were color coded based on index values, illustrating variations in distribution of obstetric outcomes, sociodemographic factors, and heat stress. 

Click to check out the [Heat Vulnerability Index for Pregnant People Interactive Map](interactive_map2.html) to explore the associations between extreme heat and adverse obstetric outcomes in India.

![cyp255 (14)](https://github.com/gracer080/heatandbirths/assets/79069159/33c1ecfa-0147-4127-ad2c-9f1bde4a48b7)


# Conclusion

As the impacts of climate change intensify, understanding and mitigating their effects on vulnerable populations becomes crucial, particularly concerning obstetric outcomes. The development and application of a spatial Heat Stress Index are essential in this effort, serving as a vital tool for identifying regions and populations at increased risk due to rising temperatures. This index, which quantifies heat stress levels by incorporating temperature, humidity, and other climatic factors, is particularly valuable in resource limited LMIC settings. Here, limited resources and infrastructure often heighten vulnerabilities to climate extremes. If further developed to incorporate more updated and nuanced data, tools like heat vulnerability indicies can help inform early warning systems, public health surveillance, policy, and infrastructural development. Building resilience amongst pregnant populations can look like enacting heat action plans, tailored to their specific needs, increasing access to maternal cooling huts for field workers, closely monitoring maternal health status - such as nutrition and hydration during high heat events. This study seeks to highlight the need for more individualized and precision data collection and development of tools meant to highlight health and environmental inequities in some of the most vulnerable populations in the world. 

# References
1.Global temperatures set to reach new records in next five years. (2023, May 15). World Meteorological Organization. https://public.wmo.int/en/media/press-release/global-temperatures-set-reach-new-records-next-five-years
2.Borg, F. H., Greibe Andersen, J., Karekezi, C., Yonga, G., Furu, P., Kallestrup, P., & Kraef, C. (2021). Climate change and health in urban informal settlements in low- and middle-income countries - A scoping review of health impacts and adaptation strategies. Global Health Action, 14(1), 1908064. https://doi.org/10.1080/16549716.2021.1908064  
3.Heaviside, C., Vardoulakis, S., & Cai, X.-M. (2016). Attribution of mortality to the urban heat island during heatwaves in the West Midlands, UK. Environmental Health, 15(S1). https://doi.org/10.1186/s12940-016-0100-9 
4.T. Cuerdo-Vilches, J. Díaz, J.A. López-Bueno, M.Y. Luna, M.A. Navas, I.J. Mirón, C. Linares,
Impact of urban heat islands on morbidity and mortality in heat waves: Observational time series analysis of Spain's five cities,Science of The Total Environment,Volume 890,2023,164412,
ISSN 0048-9697,https://doi.org/10.1016/j.scitotenv.2023.164412.
5.Magnano San Lio, R., Favara, G., Maugeri, A., Barchitta, M., & Agodi, A. (2023). How antimicrobial resistance is linked to climate change: An overview of two intertwined global challenges. International Journal of Environmental Research and Public Health, 20(3), 1681. https://doi.org/10.3390/ijerph20031681 
6.Baharav, Y., Nichols, L., Wahal, A., Gow, O., Shickman, K., Edwards, M., & Huffling, K. (2023). The Impact of Extreme Heat Exposure on pregnant people and neonates: A state of the science review. Journal of Midwifery &amp; Women’s Health, 68(3), 324–332. https://doi.org/10.1111/jmwh.13502 
7.Jiao, A., Sun, Y., Avila, C., Chiu, V., Slezak, J., Sacks, D. A., Abatzoglou, J. T., Molitor, J., Chen, J.-C., Benmarhnia, T., Getahun, D., & Wu, J. (2023). Analysis of heat exposure during pregnancy and severe maternal morbidity. JAMA Network Open, 6(9), e2332780. https://doi.org/10.1001/jamanetworkopen.2023.32780 
8.World Health Organization: WHO. (2023, May 10). Preterm birth. World Health Organization: WHO. https://www.who.int/en/news-room/fact-sheets/detail/preterm-birth
9. Zhu, Y., He, C., Bell, M., Zhang, Y., Fatmi, Z., Zhang, Y., Zaid, M., Bachwenkizi, J., Liu, C., Zhou, L., Chen, R., & Kan, H. (2023). Association of ambient temperature with the prevalence of intimate partner violence among partnered women in low- and middle-income South Asian countries. JAMA Psychiatry, 80(9), 952. https://doi.org/10.1001/jamapsychiatry.2023.1958 
10.Debnath, R., Bardhan, R., & Bell, M. L. (2023). Lethal heatwaves are challenging India’s sustainable development. PLOS Climate, 2(4), e0000156. https://doi.org/10.1371/journal.pclm.0000156 
11.Kakkad, K., Barzaga, M. L., Wallenstein, S., Azhar, G. S., & Sheffield, P. E. (2014). Neonates in Ahmedabad, India, during the 2010 heat wave: A climate change adaptation study. Journal of Environmental and Public Health, 2014, 1–8. https://doi.org/10.1155/2014/946875 
12. Zhu, Y., He, C., Bell, M., Zhang, Y., Fatmi, Z., Zhang, Y., Zaid, M., Bachwenkizi, J., Liu, C., Zhou, L., Chen, R., & Kan, H. (2023). Association of ambient temperature with the prevalence of intimate partner violence among partnered women in low- and middle-income South Asian countries. JAMA Psychiatry, 80(9), 952. https://doi.org/10.1001/jamapsychiatry.2023.1958
13.Nagaraj, A. (2022, January 20). Incomes dip for South Asia’s women home workers as heat rises.Reuters.https://www.reuters.com/markets/commodities/incomes-dip-south-asias-women-home-workers-heat-rises-2022-01-20/ 
14.The DHS Program - India: Standard DHS, 2019-20. (https://dhsprogram.com/methodology/survey/survey-display-541.cfm). (Accessed March 23, 2024)   
15. Yan Y, Xu Y, Yue S. A high-spatial-resolution dataset of human thermal stress indices over South and East Asia. Scientific Data. 2021;8(1):1–14.     








