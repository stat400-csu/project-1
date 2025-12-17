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
The code can be found in “airMonte.Rmd”. The first chunk is labeled “setting”, and it was just there to test the function and make sure we were building the equation correctly and that we would get the results that we wanted.
The second chunk of code is unnamed and it uses the same structure as the code we just built, but I made the function take in more parameters. Before it was just taking the number of simulations, and now it is taking the mean quanta, standard deviation of the quanta, the room volume, and more because we expect those to change in the future of our code. 
The third code chunk we have is called “testing model”, and this is to test the function from the second code chunk and make it run for the TB, flu, and measles quanta. And we added SARS. The table being returned was the values that each randomly sampled variable had for each simulation.
The fourth chunk of code was reworking the third chunk function that we built. We needed a vector that was defined outside the for loop to take on the probabilities that each simulation was generating so at the end we can take the mean of it. 





Usage (what to expect when running certain code and why it’s important):

























