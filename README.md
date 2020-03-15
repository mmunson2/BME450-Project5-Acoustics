# BME450-Project5-Acoustics
#### Matthew Munson
#### 3/11/2020
#### Professor Shima Abadi


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

The signal with the highest bandwidth was the marine mammal vocalization, with a vertical bar reaching from almost 0 to 20 kHz. The airgun burst was considerably smaller, with frequencies ranging from 0 to 200 Hz. Finally, the earthquake had the smallest and lowest bandwith of between 0 and 100 Hz. 

![alt text](https://github.com/mmunson2/BME450-Project5-Acoustics/blob/master/AdditionalResources/WenzCurve.png
"WenzCurve") 

The Wenz curve displayed above details the frequency ranges of various sources of ocean noise. Marine mammal vocalization falls under the "biologics" category. My data for a marine mammal call would fit into the lower end of this range, which extends from 10 Hz to 100,000 Hz. 

While airgun bursts aren't explicitly featured in the Wenz curve, they likely fall under the category of industrial activity, which ranges in frequency from 10 Hz to 10,000 Hz. One departure from the Wenz curve is the SPL of the airgun blasts, which at 120 dB are beyond the level of industrial and ship noise. This is likely because airgun blasts are intentionally designed to be extraordinarily loud, compared to ships and drilling rigs which may have acoustic dampening measures in place.

Finally, earthquakes are specifically featured in the Wenz curve and range in frequency from 0 to 100 Hz with a peak SPL of over 120 dB at 10 Hz. This corresponds exactly with my data, which has peaks of 128 dB between 0 and 40 Hz. 


# Conclusion:

This assignment provided insight into the effects of wind, rain, earthquakes, marine mammals, and airgun blasts on noise in shallow and deep water. The first section revealed an interesting correlation in how wind tends to increase SPL for lower frequencies, while rain depends on its drop size, but generally affects higher frequencies. It also followed the expected pattern in which surface conditions had a greater effect on noise in shallow water compared to at depth.

The second section of this assignment viewed three specific instances of underwater noise and compared their frequencies. The excessively loud signal of the airgun blast was greater than any other noise on the Wenz curve, save for earthquakes. This highlights the importance of reducing underwater noise pollution wherever possible.


# References:


M. Aguilera, “Ocean Noise Has Increased Considerably Since 1960s, According to New Scripps Analysis,” Scripps Institution of Oceanography, Aug. 2006.

S. S. Murugan, “Noise Model Analysis and Estimation of Effect due to Wind Driven Ambient Noise in Shallow Water,” International Journal of Oceanography, Dec. 2011.

J. A. Nystuen, “Listening to Raindrops from Underwater: An Acoustic Disdrometer,” Journal of Atmospheric and Oceanic Technology, Mar. 2001.



