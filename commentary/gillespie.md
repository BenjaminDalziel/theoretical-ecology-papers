# Comments on Gillespie 2007

## Rachael 

A chemical kinetics system is not necessarily deterministic. A RRE (reaction-rate equation) may not be very accurate in smaller systems where stochasticity is important. Stochastic chemical kinetics attempts to describe changes over time in well-stirred systems. Gillespie reviews some theoretical foundations and some advances in this area of study. In terms of theoretical foundations, the takeaways that seemed the most important were that the overall goal is to estimate the vector of counts for each species at time t (boldface X(t) is (X_1(t),..., X_N(t)). The main estimation problem is to infer the P(X(t) = x, given that X(0) = some initial x vector). Since fluctuations can't be ignored, Gillespie presents SSA as an accurate modeling framework in a setting where randomness is important to the system's evolution. There have been a couple improvements in SSA efficiency, but it is still slow. So, it might be useful to use tau-leaping, which takes the number of times reaction channel (still not solid on what a reaction channel is) R_j fires in the interval [t, t + tau] to be a Poisson RV with scale parameter (a_j(x) * tau). Then the system at the next step is x + {sum over j} (k_j * nu_j). 


## Noah

Gillespie discusses systems where ordinary differential equations break down and cannot predict the behavior of systems.
Though Gillespie was working in chemical equations, these types of systems are important biologically because there are many times when an ordinary differential equation fails to capture what might happen.
Just like the paper last week discussed, discrete-ness matters.
And that is what Gillespie does: offers a system where discrete events impact the behavior of the system.
In this case, it comes from the probabilities of molecules colliding, or changing their form so a reaction can happen.

To do this, Gillespie thinks of, and models, each of the molecules individually.
At any given point, reactants can change to products at some kind of rate (for a single molecule reaction, the simplest).
Since these reactions are occuring randomly, we can model them and I think the example in equations 11-14b reall show how cool and useful this can be.
In the end, each molecule is modeled by a Bernoulli random variable, since it changes or not.
Add these all together and you get the solution for a binomial random variable, as seen in the equations 14a and 14b.
The tau-leap method gives us even further computational power by allowing larger leaps forward in time.
Gillespie discusses how this happens because for some interval, the propensity functions do not change and therefore the probabilities that things happen don't change either.
Since this is the case, we can estimate the number of 'events' that occur using a Poisson random variable with the term $a(x)\tau$, accounting for more events happening in that period.

Connecting ODE methods but also allowing for stochastic extinction in systems is really important for my research.
The Gillespie approximation of SIR models can give a better sense for how likely an infection is to die out in a system, instead of the ODE model which always has the infection causing a outbreak.
Very cool stuff.
