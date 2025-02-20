# Regional and Gender Differences in Youth Not in Education, Employment, or Training (NEET) Rates in Italy

**Author:** Mariia Starodubtseva  
**Contact:** mariia.starodubtseva@studenti.unitn.it

---

## 📌 **Introduction**
Youth disengagement from education, employment, or training (NEET) is a significant socio-economic challenge in many countries, including Italy, which consistently records the highest NEET rates in Europe [1]. The NEET phenomenon often leads to long-term issues such as economic dependency, social exclusion, and a diminished workforce. Understanding the spatial and demographic variations in NEET rates, as well as the factors influencing them, is crucial for developing effective policies to address this problem.

Various studies have analyzed NEET rates in Italy using diverse methodologies, focusing on trends over time, socio-economic impacts, predictive factors, and comparative studies across Europe. However, few studies have specifically addressed regional differences in NEET rates and gender disparities within each region. This project aims to fill this gap using the most recent data from 2023.

---

## 🎯 **Research Objectives**
The study aims to answer the following research questions:

1. How do youth NEET rates differ across Italian regions?
2. What spatial patterns emerge in NEET rates, particularly among neighboring regions?
3. How do gender differences in NEET rates vary across regions?
4. How are youth NEET rates related to general unemployment rates across Italian regions?
5. How are gender differences in NEET related to gender differences in unemployment?

---

## 📂 **Data Description**
The datasets used in this analysis are sourced from ISTAT (Italian National Institute of Statistics) and are stored in the `data` folder of the project repository.

- **Administrative Boundaries Dataset:** Provides geometries of Italy’s regions and other territorial units, used for spatial analysis with a projected CRS (EPSG:32632).
- **NEET Statistics (2023):** Percentage of individuals aged 18-29 classified as NEET, broken down by gender and region.
- **Unemployment Rates (2023):** Unemployment statistics for individuals aged 15-74, allowing for a comparison with NEET data.

---

## ⚙️ **Methodology**
The analysis involves the following steps:
1. **Descriptive Statistics:**
- Calculate descriptive statistics (mean, standard deviation, minimum, maximum, kurtosis, skewness) for NEET and unemployment rates.
- Create histograms to visualize the distribution of NEET and unemployment rates.
2. **Spatial Visualization:**
- Generate choropleth maps to visualize NEET and unemployment rates, as well as their gender difference across Italian regions.
3. **Spatial Autocorrelation:**
- Compute Moran’s I statistic to identify spatial clusters of neighboring regions with similar NEET rates.
4. **Correlation and Regression Analysis:**
- Analyze the relationship between NEET and unemployment rates using Pearson's correlation coefficient.
- Analyze the relationship between gender gaps in NEET and unemployment using Pearson's correlation coefficient.
- Perform linear regression to model the association between NEET rates (dependent variable) and unemployment rates (independent variable).
- Perform linear regression to model the association between NEET gender difference (dependent variable) and unemployment gender gap (independent variable).
5. **Residual Analysis:**
- Perform Moran’s I test on the residuals to assess spatial dependence not explained by the models.

---

## Requirements
You can install all required packages using the provided `requirements.txt` file.

    ```
    pip install -r requirements.txt
    ```

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

## 📑 **References**
1. Eurostat. (2021, July 14). Over 1 in 6 young adults not in employment or education. European Commission. https://ec.europa.eu/eurostat/web/products-eurostat-news/-/edn-20210714-2
2. Amendola, S. (2021). Trends in rates of NEET (not in education, employment, or training) subgroups among youth aged 15 to 24 in Italy, 2004-2019. Journal of Public Health, 1-9.
3. Brunetti, I., & Ferri, V. (2018). Essere NEET in Italia: i principali fattori di rischio.
4. Lovaglio, P. G., & Berta, P. (2024). Personal and regional risk factors of being a NEET: a comparative study in Italy, France and Germany with LFS microdata. Quality & Quantity, 1-32.
5. Odoardi, I., Quaglione, D., D’Ingiullo, D., Furia, D., & Cascioli, P. (2022). The increase in the gender gap with age: an analysis on Italian NEETs. Global & Local Economic Review, 26(2), 99-124.
6. Cascioli, R. (2011). I Neet. Disparità territoriali e il difficile ingresso dei giovani italiani nel mercato del lavoro. la Rivista delle Politiche Sociali, 3, 61-81.
7. ISTAT. (2024). Limiti amministrativi delle regioni italiane (geometry data) [Data file]. Italian National Institute of Statistics. https://www.istat.it/storage/cartografia/confini_amministrativi/generalizzati/2024/Limiti01012024_g.zip
8. ISTAT. (2023). NEET statistics for individuals aged 18-29 in Italy (Query ID: 66674) [Online database]. Italian National Institute of Statistics. Retrieved from http://dati.istat.it//Index.aspx?QueryId=66674
9. ISTAT. (2023). Unemployment rates for individuals aged 15-74 in Italy (Query ID: 66677) [Online database]. Italian National Institute of Statistics. Retrieved from http://dati.istat.it//Index.aspx?QueryId=66677
