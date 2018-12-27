# MCMC_MusicGenerator
Generate music in artist's style using Metropolis-Hastings Markov chains approximation.

## Overview
This project intends to use a variation of Monte-Carlo Markov Chain modeling to create a short music piece in the style of Bach. MCMC sampling methods are most commonly used to create samples of a target distribution that is computationally intractable to calculate for sampling purposes. This is often because the sample space is exponentially large, and the normalizing constant to calculate the probability distribution would be too large to sum against. Instead, the Metropolis-Hastings variant of MCMC sampling uses an “acceptance ratio” of two states’ probabilities to either accept or reject a random sample, with this acceptance ratio probability proportional to the distribution. 
    In the context of music generation, one method is to compare the transitions between two consecutive notes on two qualities: note duration and note pitch. By generating music that matches approximately these two qualities for a certain style of music, we hypothesize that it is possible to emulate the style through MCMC sampling. Repeated sampling from a transition matrix distribution will eventually create samples (sequences of notes, or melodies) that on expectation approximate the distributions of rhythm and pitch in Bach’s music.


## Result (sample)

![figure](generated.png)
                                              
