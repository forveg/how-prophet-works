### Notes on Prophet

<img align="center" src="assets/image.png" width="700px" title="Picture to catch your attention" />

#### Why?

This is not supposed to be a tutorial or a guide, but patchy notes for myself to quickly recall how prophet works/ where to tweak it. 

#### Overview

In the first part I skim through the prophet code base, highlighting key computation steps. Second part is a small demo of how to extract preprocessed variables from prophet, fit it using another backend (numpyro) and then plug estimated parameters back into prophet for prediction. The purpose is to demonstrate the modeling logic, not to reproduce prophet perfectly.


#### Acknowledgements

My main inspiration has been this excellent post [1] from Ritchie Vink (creator of polars). I heavily borrowed from Nicolas Fauchereau's notebook [2] on alaysis of weather impact on cycling counts in Auckland, and used the same data. Finally, I thank developers of prophet [3]. Docs are helpful and code is easy to navigate. 


1. [Build Facebook's Prophet in PyMC3; Bayesian time series analyis with Generalized Additive Models](https://www.ritchievink.com/blog/2018/10/09/build-facebooks-prophet-in-pymc3-bayesian-time-series-analyis-with-generalized-additive-models/)
2. [The impact of weather conditions on cycling counts in Auckland, New Zealand](#https://github.com/nicolasfauchereau/Auckland_Cycling/blob/master/notebooks/Auckland_cycling_and_weather.ipynb)
3. https://github.com/facebook/prophet/tree/main