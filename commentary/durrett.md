# Comments on Durrett and Levin 1994

## Liz
This paper explores 4 different ways to model spatially distinct discrete individuals (hawks and doves). They compare mean field approaches (I think ordinary differential equations?), patch models, reaction-diffusion equations, and interacting particle systems. 1) Mean field approach = each individual has equal probabiltiy to interact with every other indiviudal. 2) Patch models = discrete individuals into patches with no other spatial structure. 3) Reaction - diffusion = infinitesimal individuals diffues in space and only local interactions. 3) Interacting particle systems = individuals are discrete and space is explicit. All four approaches reach the same conclusion that if there is a positive density of both dove and hawk ,there will be a unique equilibrium. But when the two compete for the same resource then spoatial and non-spatial models disagree and intial densities matter. They also see that hawks reproduce faster than doves but a population of only hawks dies out which I think makes a lot of sense biologically. Notable quotes: "_We leave it to others more skilled in the study of these models to resolve this mystery"_ and "_...this figure might seem to indicate a much more exotic (or, gasp, chaotic) behavior..._".


## Rachael

The authors discuss how to model a spatially distributed system over time (which level of granularity is appropriate?). ODEs model change in larger levels of organization (e.g., proportion state variable) leave out granularity below that. Models that add a spatial component to that (the RDE) or stochasticity are  investigated alonside the mean field approach in three cases where the parameters of a hawk-dove system are changed. In case 1 of parameters in the payoff matrix (ode has globally-attracting fixed point):

Mean field approach (deterministic, non-spatial) - proportion hawks will tend to p_0.

Reaction diffusion equation (deterministic, spatial) - conjecture 1.2 states that as long as hawks and doves are are non-zero at spot x at time 0, as t goes to infinity, the hawks and doves will converge to their equilibrium values at that spot x - same conclusion as mean field approach.

Patch model(non-deterministic, non-spatial) with 2500 patches - simulation shows that numbers of hawks and doves per patch settles at 2 and 2.7.

Interacting particle system(non-deterministic, spatial) - haw and dove numbers converge exponentially fast to their equilibrium values of 2 and 2.7 per site. 

However, in the other (4-dimensional) parameter values - these four methods don't necessarily agree! 

Tangential thought: different modeling groups emphasize different approaches and reach different conclusions about the same system... Sharing modeling frameworks is important. 

## Bryan

Here, the authors compare four different models with four different appraoches to spacial dynamics (or lack thereof): ODE, Reaction Diffusion, Patch models, and interacting particle systems. I like that the emphasis on the important role of spacial structure. Selfishly because I think my own research (and a tragedy occuring in a nonspacial structure) also supports those ideas. My major take home messages are: i) space/population structure matters and ii) space/population structure (may) need more consideratin in model development with special attention payed to exactly what kind interactions are happening that you want to model. 

However, I CANT GET OVER THE FACT THAT THEY USED 'HAWK DOVE' FOR EVERY PAYOFF MATRIX, BUT DIDN'T SHOW ANY ACTUAL HAWK DOVE GAMES! Like.. why??? I'm so distracted (and confused?) by this. Why not just use a standard payoff matrix with C/D for cooperate and defect? They didn't even explain the hawk dove game. FYI Hawk=fight for food & Dove=don't fight for food. Named after wartime ideologies. So if you choose dove and your opponent chooses hawk, you get nothing (payoff value c=0). They steal your food. They claimed that case three was the true hawk-dove game, and, no. Not traditionally anyway, which requires a= (v-c)/2 b=v c=0 and d=v/2. v being benefit/victory of winning food and c being cost of fighting. and while you could modify pyaoffs somewhat (because they are arbitraryish) the whole point of the hawk dove game is that the dove would rather give up everything than fight. So dove strategy should not go below 0 - ie benefit is reduced but cost = 0 since cost is fighting. -end rant-

## Emily

This paper compares the predictions of different types of models with different levels of detail. These are models using ordinary differential equations, reaction diffusion system, patch models, and interacting particle systems. Outcomes of the models are analyzed for the hawk and dove game, in which the hawks and doves interact differently in the different models (e.g. interaction with neighbors a certain number of steps away in a model with spatial patches vs a dynamical system where interaction can in essence happen anywhere). The main differences in the interpretations of these models are whether individuals are “infinitesimal” or are treated as discrete units, and whether patches of individuals have spatial structure or not. The main findings are:

When fitness of one type of individual is enhanced by the presence of the other, all approaches come to the same conclusion that there is a unique equilibrium.

When two individuals compete for the same resource, spatial models and nonspatial models reach different conclusions. In spatial models, the winner first establishes itself in an area, then expands this area. In the nonspatial models, only initial density seems to determine the winner.

When one type always reproduces faster than the other, the deterministic models die out, but a patch model allows for growth in some patches balanced by a decline in other, effectively creating a cycle where densities may decrease to near extinction but then recover. 

The comparisons of these models give some insight into which situations may be more suited to modeling by a certain approach, depending on the biological rationale, which could be informed by empirical data that gives insight to the most important aspects of a situation for modeling. This leads to one question I had, which is about just how accurate, biologically speaking, these models can be. Assumptions are always made in order to allow us to model complex situations, but how can we be assured that any of these approaches will be “good enough,” since they all make different assumptions? Additionally, in comparing these models (or in comparing any models), how were the parameters for testing/comparison determined? Models can be radically different for different initial values or parameter values, so I’m not sure I’m convinced choosing “random” or even “interesting” parameter values is appropriate for a valid comparison, past allowing for some qualitative comparisons.

