# Machine learning for chaotic time-series data generated from simple food webs


## Generating the data
[MakeData.ipynb](MakeData.ipynb): This is where all the data is generated for the machine learning experiment using non-linear differential equations described in the report. The calculations were optimized using Python's built-in Runge-Kutta integration to ensure that the time step is always small enough.

## Visualizing the data
[coexistence.ipynb](coexistence.ipynb): To begin to analyze the results of the simulation, I attempt to visualize at which death rates species tend to survive or parish statistically based on the simulations.

[reduce_data_analysis.ipynb](reduce_data_analysis.ipynb): Testing how many time steps are necessary to achieve accurate results.

![pictures/pic1.png](pictures/pic1.png)

## Analyzing the data
[foodweb_vs_random.ipynb](foodweb_vs_random.ipynb) and [foodweb_vs_random_v2.ipynb](foodweb_vs_random_v2.ipynb): By creating some randomly changing time series data that is similar to real data except completely random, we can do a comparison agaisnt the real data to find what kind of features make the data recognizable by the AI. All the data is input into a binary classifier, and then the filter is visualized to look for hidden features that were picked up during the training.


## Machine learning
[single_species_classification.ipynb](single_species_classification.ipynb): By looking at time series data produced from 3 different food web structures, the AI learns to classify not only which food web structure the line comes from but also which individual species and level in the food web that it came from, even when the data is chaotic.

<img src="pictures/pic4.png" alt="pic" width="500"/>

Thank you for reading, see the final [report](report.pdf)
