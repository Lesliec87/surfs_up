# surfs_up

## Overview of the analysis: 

In this analysis we have came up with a plan of setting up a Surf n Shake in Oahu,Hawaii. Knowing we would need an investor backing us up, we put up a business plan and then reached out to investor W. Avy. 

W. Avy asks us to run some analytics on weather data set and request more information about temperature trends before opening the surf shop. Specifically, he wants temperature data for the months of June and December in Oahu, in order to determine if the surf and ice cream shop business is sustainable year-round.

## Results:

### Summary Statistics for June:

![June statistics](https://github.com/Lesliec87/surfs_up/blob/main/Results_June.png)

### Summary Statistics for December:

![December Statistics](https://github.com/Lesliec87/surfs_up/blob/main/Results_December.png)

- The average weather in the month of June: 74.94 F
- The average weather in the month of December: 71.04 F
- The minimum weather for both months: 
  - June: 64 F
  - December: 56 F  
- The maximum weatehr for both months: 
  - June: 85 F
  - December: 83 F

## Summary:

- For both June and December the weather seems to be on average good enough for tourist to visit as a year-round vacaton spot.
- December is the month that might have some cooler weather that might cause a drop in tourist. 
- Another query that might be useful is to find the precipitation to be able to analyse how much rain will be expected for both June and December.
  - For June: session.query(Measurement.prcp).filter(extract('month', Measurement.prcp)==6).all()
  - For December: session.query(Measurement.prcp).filter(extract('month', Measurement.prcp)==12).all()
