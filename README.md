# project-1
Group 1 Project for STAT400 @ CSU

Title: Stochastic Monte Carlo - Extension of Beggs et al. 

Project Description:

This project set out to replicate the stochastic monte carlo of Beggs et al. study that was investigating the transmission of airborne disease in indoor spaces. The goal was to replicate the stochastic monte carlo, pick an airborne disease that was not covered in the paper and see what the model would predict for probability and to see how the original airborne disease probabilities would change when room volume, exposure time, and number of infected individuals would change. 

Dependencies (libraries we needed to run code):
For reproducibility we set a seed to be 400. No reason other than the class being Stat-400.
The libraries we loaded in included:
- dplyr, stats, tidyr, tidyverse, broom, ggplot2, and tibble


Installation (what to run and where to find them):
The code can be found in “airMonte.Rmd”. 
The first chunk is labeled “setting”, and it was just there to test the function and make sure we were building the equation correctly and that we would get the results that we wanted.

The second chunk of code is unnamed and it uses the same structure as the code we just built, but I made the function take in more parameters. Before it was just taking the number of simulations, and now it is taking the mean quanta, standard deviation of the quanta, the room volume, and more because we expect those to change in the future of our code. 

The third code chunk we have is called “testing model”, and this is to test the function from the second code chunk and make it run for the TB, flu, and measles quanta. And we added SARS. The table being returned was the values that each randomly sampled variable had for each simulation.

The fourth chunk of code was reworking the third chunk function that we built. We needed a vector that was defined outside the for loop to take on the probabilities that each simulation was generating so at the end we can take the mean of it. 

The next few chunks are labeled as Flu, Measles, and SARs, and these code chunks are using the function and running the respective quantas of each disease through the simulation to get the estimation of probability of infection for susceptible individuals.

The code chunk labeled "summary results"...

The code chunk titled "graph" shows the distribution of the probability of all of the airborne diseases.

The code chunk titled "Scenario 1 TB" applies the changes we made to the room volume and the exposure time and predicted the probability of TB with it. 
This pattern was repeated for Flu and Measles. 
Then a graph was made to show the three diseases and their probability distribution.

The code chunk titled "Scenario 2 TB" applies the changes we made to the number of infected individuals.
This pattern was repeated for Flu and Measles.
Then a graph was made to show the three diseases and their probability distribution.

All the code is sequential and if you start from the top, everything should run fine.





















