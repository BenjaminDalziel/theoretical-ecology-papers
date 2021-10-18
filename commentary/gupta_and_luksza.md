# Comments on Gupta et al. 1996 and Luksza et al. 2014

## Isaac
The first paper by Gupta et al. (1996) creates a simple mathematical model based on the genetic and amphibology concepts such as the immune system of the host, strains transmission, abundance of such strains in homogenous populations. It was interesting to see how it is possible to relate these biological concepts in a theoretical framework. The paper proposed by Luksza et al. (2014) explores the previous idea further into application. AN example is vaccine selection for the predominant strains. It would super cool if we started to model specific factors within the host that could alterate the genetic information of the virus. So, it is easier to predict possible variants and the virulance of it. An example of a factor increasing virulance on influenza virus is obesity (Honce et al. 2020). By taking this into consideration, it would be possible to create more accurate models in preventing possible more virulent strains.

Honce, R., Karlsson, E. A., Wohlgemuth, N., Estrada, L. D., Meliopoulos, V. A., Yao, J., & Schultz-Cherry, S. (2020). Obesity-related microenvironment promotes emergence of virulent influenza virus strains. MBio, 11(2), e03341-19.

## Liz
After reading Gupta et al., I felt like I get the concept they were trying to show with cross-immunity and I thought Figure 2a was really useful and good at showing that and I also liked Figure 3 a lot. One main idea being that at high levels of cross-protection it leads to linkage disequilibrium with one strain taking over instead of multiple strains coexisting in the population. I do struggle with understanding the application of this with Neisseria meningitidis, and Figure 6 I thought wasn’t very useful for displaying the different populations structures. One question I had for this paper was what real-life differences in strains might lead to one persisting in the population vs being eliminated (for example in Figure 2a what made ax and by the dominant strains vs bx and ay)? Would it be something like having a higher R0?
What I mostly understood from the Luksza and Lassig paper was that it applied the model to be able to predict future strains of influenza which is obviously very important and useful as scientists try to do that every year when making the next seasons flu vaccines. My main question is whether this model predicted flu strains better than whatever method we currently use? Is it the same method? If not, why don’t we use this if it works so well?

## Noah

The main question being asked in Gupta et al. is why do infectious pathogens maintain specific genes, as opposed to having a random distribution of genes from all the different strains that it could theoretically mate with.
They make a simple mathematical model to show that immune system pressures are a driving force behind this conservation of specific gene combinations, and propose different scenarios (Fig 6) for how different pressures might manifest.
They are seeking to highlight how evolutionary forces (and structural parts of how DNA and bacterial mating) will drive epidemiological structure when there are multiple strains.
Luksza and colleagues take a specific case of this concept and expand to include another important pressure when thinking of how a disease will manifest in a population: vaccination.
In this paper, they aim to both predict which strains of influenza might become dominant, and refine this model to predict year to year variation in a specific flu protein.
They use this model to show the evolutionary history of flu strains through a few winters, and Fig 1 really highlights how this evolution happens.

My main takeaways from these papers really concerns the evo/eco relationships that are inherent in disease systems.
I believe it highlights the evolutionary arms race that we discuss often in evolutionary relationships, but in an interesting way since one of the pressures on pathogens is an evolving entity unto itself.
Gupta highlights this relationship as we see rules emerge for how strains will occur under different types of pressure.
I also can see that pieces of this concept come from the structure of DNA itself, since only genes that are far apart structurally are likely to be able to recombine at high rates.
In the Luksza paper, I found it really interesting that, while the year to year strain phylogeny was fairly consistent, there still is a fair amount of uncertainty.
This uncertainty is very important in my work as one of the things I am thinking about is how to incorporate epidemiological and genetic information to better inform transmission trees

## Rachael 
Gupta et al. discuss how cross-protection contributes to a set of discordant strains becoming dominant. (Discordant strains don't have shared alleles for immmunologically important loci). When cross-protection is zero, all strains equilibrate at the same level, given that they have the same R_0 (the authors call this symmetric equilibrium). To test this theoretical result, they use data for a pathogen with two important epitopes (with eight and 14 families, respectively). The null hypothesis that there is random association between these epitopes is rejected using a chi-square test for significance - only a handful of discordant combinations survive at high frequency.

Luksza et al. argue that two factors dictate strain fitness: adaptive epitope mutations and detrimental non-epitope changes. Using genomic data, the authors predict evolution of influenza clades from a year to the next. They predict clade frequency in the next season: $$ \hat{X_v}(t+1) = \sum_{i:v,t}x_ie^{f_i} $$.
They also want the f_i for each strain to change based on deleterious mutations in i and cross-immunity to strains that have appeared previously: $$f_i = f_0 - L(a_i) - \sum_{j:t_j<t_i}x_jc(a_i,a_j)$$.
The value of the cross-immunity function depends on changes in strain i and in strain j (a_i and a_j).
$$ W_v = X_v(t+1)/X_v(t) $$. The predicted W_v for some clades is greater than one (mostly because antigenic mutations appear in the context of a lineage that has had more fitness-enhancing mutations recently).

## Ben (in progress)
Gupta et al. address the question of how distinct lineages of an infectious pathogen can maintain and cocirculate despite rapant opportunities for the exhange of genetic information which, absent some countervailing processes should homogenize distinc strains. They use a simple mathematical model which assumes the dominant actor in the process is the host immune system, and which assumes no spatial structure in the host population (and thus no spatial constraints on genetic exchange). In analysis of the model, several classic elements of theoretical ecology / epidemiology emerge in a new context. Equilibrium prevalence of the strains depends on the degree of cross-protection. When cross protection is low, the dynamics decouple and each strain comes to rest at a prevalence of 1 - 1/R0. When cross protection is high, there is an 'asymetrical equilibrium' where one strain comes to dominate. There is a critical level of cross protection above which the symatrical equilbrium collapases. The model predicts cocircualting strains should show linkage disequilibrium among dominant antigens modulated by the degree of cross protection, and that 'strain-structuring' immune responses can be leveraged to identify dominant antigens. THe paper introduces an elegant model that resonates with some key ideas in theoretical ecology, but it  is alo notable in the way it engages with data to advance the argument of th emodel.




