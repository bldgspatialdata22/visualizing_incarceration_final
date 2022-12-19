# Visualizing Incarceration Final Project

## Intro

This project aimed to visualize the true scope of mass incarceration, not only by mapping prisons and jails but also by mapping those impacted by incarceration. The visualizaiton produced for this project maps those with am immediate family member (parent, sibling, child) that has been incarcerated in the state of Maryland using dot density. This was a trial of methods that will be expanded to the entire United States. Studies show that an estimated 1 in 2 people in the United States have a parent, partner or sibling that has been incarcerated, but this depends on different demographics including race and region, which were considered in this visualization.

## Data and Methods

While no spatial data on this existed, a study from researchers at Cornell published in 2019 created estimates associated with various demographics estimated how many people in the United States had an Immediate Family Member that was incarcerated. For this project, these estimates were visualized using a dot density map with 1 dot = 1 person. I was able to produce this visualization using the mapboxapi, leaflet, tidycensus, tidyverse, totalcensus, and tippecanoe packages along with data from the American Community Survey and the Decennial Census. 

The source for the estimates for how many people had an immediate family member that had been incarcerated was [The FamHIS Study](https://journals.sagepub.com/doi/10.1177/2378023119829332#articleCitationDownloadContainer). This study in conjunction with the 2018 5 year ACS (American Community Survey) block group level data were the foundation for the dots in the dot density map. For the purposes of this project and the accompanying time, money, space limitations the study area was limited to Maryland.

The prisons and jails dataset comes from the decennial census which I have fetched using R is based on [this script](https://www.gl-li.com/2018/02/05/map-prisons-in-the-united-states/).

The dot density map that was produced using the data from the ACS and Cornell study was stylized and hosted on mapbox using mapbox tiles and the final visualization was produced using leaflet.

## Learn More

[Cornell Study](https://journals.sagepub.com/doi/10.1177/2378023119829332#articleCitationDownloadContainer) | [Bail Funds by State](https://bailfunds.github.io/) | [Abolition Reading List](https://abolitionistfutures.com/full-reading-list)
