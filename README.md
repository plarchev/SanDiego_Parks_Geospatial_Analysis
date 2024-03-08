# San Diego Park-Income Geospatial Correlation
## Overview
In this project, I wanted to look into how the locations of parks are related and correlated to household income in San Diego. I computed buffers and enriched my data utilizing a service called ArcGIS Online, and I was then able to gather economic data on the areas inside the buffers. I had to find what the cryptic column names meant and cleaned my data otherwise. My data overall was very clean. I conducted my analysis by comparing the observed household high income distribution to the distribution generated by the national average household high income statistics. I then performed this same analysis for moderate and low income households. In the end, my analysis supports the idea that San Diego gardens are placed disproportionately close to high income households.

## Research Question
Are San Diego garden locations fair relative to household income? In San Diego, are there gardens nearer communities with high income? What quantifies high income and how does this relate to the proportion of households who have high income around a San Diego garden? Moderate Income? Low Income?

## Hypothesis
In San Diego, gardens are disproportionately placed nearer communities with higher income because of the idea that gardens can be privately funded and people with higher income have more disposable income.

Null Hypothesis: The proportion of high income households near a garden community in SD is 31.4% (the % of households in the US who make over 100k)

Alternative Hypothesis: The proportion of high income households near a garden community in SD is greater than 31.4%

## Conclusion & Discussion
In conclusion, there is a disproportionate amount of high income households around San Diego gardens. By performing a one sample sign test, we were able to uncover a very low p-value (**p-value = 4.5633687833186827e-11**), indicating that the distribution observed around SD gardens was very different than the distribution generated by the national average proportions. Thus, we go in favor of the alternative hypothesis which states that SD gardens are placed in loacations closer to higher income households. The limitation and hesitation about coming to this conclusion is that I am assuming that San Diego's income distribution is representative of the national income distribution. This may not be entirely true. This is a limitation because I was unable to successfully track the distribution of income in San Diego. I used national average numbers instead. **So, there is a disporportionate amount of high income households around San Diego gardens assuming that the San Diego income distribution is representative of the natinoal income distribution. Using this same assumption, there is a proportionate amount of moderate income households around SD gardens, and a disproportionately low amount of low income households around SD gardens**. Additional limitations include being unable to geoenrich the names of the parks using geometry (was not working for some reason) as well as being unable to extrapolate to other cities (this is an SD specific study). One thing to note is that I did choose a fair number of arbitrary thresholds and I did make key assumptions (such as bin bounds and standard deviations) during this analysis. In conclusion, my analysis supports my initial hypothesis.

Future steps: Future analysis would include performing location allocation (choosing where to put future, prospective gardens). This requires a LOT of work including publishing a multitide of layers and picking by hand prospective and suitable locations for parks. An easier and still effective method would be to compute some sort of suitability analysis utilizing rasters, and overlay that map with the map of income distribution, and choose a location that is both suitable and fair.
