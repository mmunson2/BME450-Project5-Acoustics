# BME450-Project5-Acoustics
## Matthew Munson
#### 3/11/2020
## Professor Shima Abadi


# Introduction:

The study of ocean noise is an area of increasing importance, as the level of noise in the ocean has increased 10 to 12  decibels since the 1960s [1]. This increase is mainly attributed to the explosion in global shipping, but other sources of noise including sonar and oil exploration are likely influences. This assignment tasked students with analyzing noise caused by natural sources such as wind, rain, marine mammals, and earthquakes. We also studied the effect of airgun blasts; commonly used to search for oil deposits beneath the seabed. These acoustic profiles can be used to gauge what is 'normal' and create a baseline which future recordings can be compared to. 


# How I Did It:

Much of this assignment involved adapting a provided code file for my own analysis. I created two functions, one for calculating and plotting power spectral density, and the other for plotting a spectrogram. These functions relied on code written and provided by Professor Shima Abadi. I then retrieved data from my meteorology project to determine four combinations of weather conditions for the Oregon Offshore and the Oregon Shelf hydrophones. These conditions are rainy and windy, not rainy or windy, rainy but not windy, and windy but not rainy. This allows us to compare the effect of each weather phenomenon on ocean noise.

For the second half of the assignment I used the Ocean Observatories website to find periods of marine mammal vocalization, airgun blasts, and an earthquake. I then fed this data into the spectrogram function to plot its frequency spectrum. 

# Results:

## Section 1: Wind and Rain Noise

### Oregon Offshore:

#### Not Windy or Rainy:
![alt text](https://github.com/mmunson2/BME450-Project5-Acoustics/blob/master/Results/Oregon%20Offshore/NotWindyOrRainy.png "NotWindyOrRainy") 

#### Rainy and Windy:
![alt text](https://github.com/mmunson2/BME450-Project5-Acoustics/blob/master/Results/Oregon%20Offshore/RainyAndWindy.png "RainyAndWindy") 

#### Rainy but not Windy:
![alt text](https://github.com/mmunson2/BME450-Project5-Acoustics/blob/master/Results/Oregon%20Offshore/RainyNotWindy.png "RainyNotWindy") 

#### Windy but not Rainy
![alt text](https://github.com/mmunson2/BME450-Project5-Acoustics/blob/master/Results/Oregon%20Offshore/WindyNotRainy.png "WindyNotRainy") 


### Oregon Shelf:

#### Not Windy or Rainy:
![alt text](https://github.com/mmunson2/BME450-Project5-Acoustics/blob/master/Results/Oregon%20Shelf/NotWindyOrRainy.png "NotWindyOrRainy") 

#### Rainy and Windy:
![alt text](https://github.com/mmunson2/BME450-Project5-Acoustics/blob/master/Results/Oregon%20Shelf/RainyNotWindy.png "RainyAndWindy") 

#### Rainy but not Windy:
![alt text](https://github.com/mmunson2/BME450-Project5-Acoustics/blob/master/Results/Oregon%20Shelf/WindyAndRainy.png "RainyNotWindy") 

#### Windy but not Rainy
![alt text](https://github.com/mmunson2/BME450-Project5-Acoustics/blob/master/Results/Oregon%20Shelf/WindyNotRainy.png "WindyNotRainy")


## Section 2: Airgun, Marine Mammals, and Earthquake/Volcano Noise

### Marine Mammal Vocalization

![alt text](https://github.com/mmunson2/BME450-Project5-Acoustics/blob/master/Results/MarineMammal.png
"MarineMammal") 


### Airgun Blasts

![alt text](https://github.com/mmunson2/BME450-Project5-Acoustics/blob/master/Results/AirgunBlasts.png
"AirgunBlasts") 

### Earthquake

![alt text](https://github.com/mmunson2/BME450-Project5-Acoustics/blob/master/Results/Earthquake.png
"Earthquake") 

# Analysis: (Section 1)

### What is the effect of wind and rain on underwater noise? Explain any behavior you observe in your result.

In general, wind and rain increased the PSD, and an increase of 20 dBm per Hz is visible in the Oregon Shelf plot between not windy or rainy and rainy. 

Determining a clear correlation between the individual effects of wind and rain on noise was difficult with my data set, so I conducted some research on the effects of each phenomenon. A study conducted in 2011 on constructing a model for wind noise in shallow water provided a useful comparison.

![alt text](https://github.com/mmunson2/BME450-Project5-Acoustics/blob/master/AdditionalResources/NoiseSprectrum.jpg
"Noise Spectrum") 

Plot Credit: [2]

This plot displays the increase in PSD as wind velocity increases. There's a hyperbolic trend with lower frequencies having very high dBm per Hz compared to higher frequencies. Another plot from the same source illustrates which frequencies are most affected by wind speed.

![alt text](https://github.com/mmunson2/BME450-Project5-Acoustics/blob/master/AdditionalResources/NoiseLevelPerFrequency.jpg
"NoiseLevelPerFrequency") 

Plot Credit: [2]

This plot displays how lower frequencies increase with wind speed, while higher frequencies increase slightly or remain the same. 

With some background research complete, I can attribute the increase in lower frequencies in the Oregon Shelf Windy but not Rainy plot to the increased wind speed. This trend is less visible in the Oregon Offshore plot, possibly because of a relatively smaller wind velocity or the deeper hydrophone position.

To determine the impact of rain on underwater noise, I once again conducted outside research. I found that rain noise is a result of drops hitting the surface as well as the bubbles they create. The noise generated by the bubbles is dependent on the size of the raindrops. Smaller drops produce high frequency noise in the range of 13-25 kHz and large drops make noise as low as 1 kHz.[3]

With background research conducted, I attribute the spikes between 10 and 15 kHz on the Oregon Shelf Rainy and Windy and Rainy but not Windy plots as a result of the rainfall. These bumps are not visible in the recordings when it was not raining, and indicate that the raindrops were relatively small. Once again, this trend is less visible in the Oregon Offshore plot, and is likely due to the hydrophone being located further from the surface.

### Which one has the highest impact? Rain or wind?

Wind appears to have the greatest impact on ocean noise, with a PSD increase up to 20 dBm per Hz. While rain creates spikes in certain frequencies, the increase in PSD isn't as significant and only affects that frequency as opposed to the entire curve.

### What are the main reasons for observing different spectral levels in Oregon shelf compared to Oregon offshore?

The main difference for comparing the two locations is the change in depth. The Oregon Shelf package is located 80 meters beneath the surface while the Offshore device is 580 meters deep. This has a considerable impact on the effect of wind and rain on the noise. This is shown in my results, where the Oregon Shelf data is influenced by wind and rain, but the Oregon Offshore is relatively unchanged.


# Analysis: (Section 2)


### Compare the bandwidth of these three signals (1 point). Are they consistent with what is shown in the Wenz curve?





# Conclusion:


# References:


https://scripps.ucsd.edu/news/2594

https://www.hindawi.com/journals/ijocean/2011/950838/

https://journals.ametsoc.org/doi/full/10.1175/1520-0426%282001%29018%3C1640%3ALTRFUA%3E2.0.CO%3B2



