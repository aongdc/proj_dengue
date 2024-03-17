## Class Presentation for COMM2550 Data Project

### Presentation
This folder contains the pdf file of our presentation slides.

The presentation covers:
  1. What is your research question and hypothesis?
  2. What data did you use, how did you acquire and clean it and what are its dimensions?
  3. What analyses did you carry out?
  4. What are your key findings so far?
  5. Next steps before final submission.

In particular:

1. Research questions and hypotheses
 
**RQ1: What is the relationship between trends of Google search terms for dengue and the number of reported dengue cases in Singapore?**  
```
H1: The number of dengue-related Google searches is positively correlated with the number of reported dengue cases in Singapore.  

H2: An increase in dengue-related Google searches will be followed by a slightly delayed increase (within 0-2 weeks) in the number of reported dengue cases in Singapore.  

H3: An increase in the number of reported dengue cases in Singapore will be followed by a slightly delayed increased (within 0-2 weeks) in dengue-related Google searches  
(H3 was added after conducting exploratory analysis for H2)
```

**RQ2: What is the relationship between various weather measures and dengue cases in Singapore?**
```
H4: Precipitation rate is positively correlated with the number of dengue cases in Singapore.

H5: Relative humidity is positively correlated with the number of dengue cases in Singapore.

H6: Hours of sunshine is positively correlated with the number of dengue cases in Singapore.
```

**RQ3: What is the relationship between various weather measures and trends of Google search terms for dengue in Singapore?**
```
H7: Precipitation is positively correlated with the number of dengue-related Google searches in Singapore.

H8: Humidity is positively correlated with the number of dengue-related Google searches in Singapore.

H9: Hours of sunshine is positively correlated with the number of dengue-related Google searches in Singapore.
```

  2. Data and data sources
  
- Weather:
    - daily hours of sunshine: open-meteo.com
    - relative humidity: open-meteo.com
    - daily temperature: open-meteo.com
    - rainfall: open-meteo.com

- Google search trends:
    - using Google Trends (platform)
    - 9 keywords: dengue fever, dengue, fever, bone pain, mosquito bite, mosquito, rain, rash and rashes
    - year by year data
    - relative values

- Dengue: data.gov
    - weekly data
  
3. The main form of analysis was correlation.
  
4. Key findings as of the presentation time:

- RQ1 was explored in depth

    **H1**
    - aggregated dengue-related Google searches produced a weak, positive correlation with the number of dengue cases
    - individual search terms produced slightly stronger correlations
    - when terms that are closely-related are grouped, slightly stronger correlations were found
    - terms that directly contained 'dengue' had stronger and positive correlations, as compared to terms indirectly related to dengue (e.g weather terms)

    **H2**
    - strength of correlation decreases when lags of 1 and 2 weeks are introduced
    - there are stronger correlations between timely Google searches and dengue cases

    **H3**
    - reversing the order of time lags (more reports of dengue cases before an increase in Google searches) did not increase the strength of correlations

5. Next steps:
  
 - Cleaning up weather data
 - Conducting data analysis for RQ2 and RQ3
 - Cleaning up the notebooks
 
6. Feedback: Since Google Trends data is relative, we should calculate the coefficients of each year and then find the average coefficient.  
    - **Due to this feedback, we have changed our approach in the RQ1 notebook, which is why different values are reported in the presentation.**