# Commentary on Kendall et al. 2019






## Rachael 
Matrix population models (MPMs) have been presented as a way to turn life-history information into a quantitative form, but the authors argue that even published MPMs contain errors. They talk about how b_x (birth rate at age x) can't be a matrix element because it doesn't span a timestep. They then explain post-breeding census modeling is when F(x) = sigma_x * b_x' is F(x) = parent survival * birthrate for individuals aged x'. When you let x_m be age at first reproduction, and the individuals are age x_m at the end of the timestep - they just reproduced for the first time, meaning they were age x_(m-1) at the beginning of the timestep - you need to ensure you don't mess up the placement of the first nonzero fertility coefficient. It seems that the most common error is thinking it is one ahead of where it actually is, so they suggest F_xm = sigma_xm * b_xm, which is basically focusing on age at the end of the time step. This approach doesn't translate over to stage-structured model formulations, though. The depictions of intuitive v. correct stage-structured models were helpful in trying to understand this part. They then discussed the challenges of estimating gamma_i, the fraction of individuals who end up exiting stage i. A large portion of the paper is about assessing a set of studies that use MPMs, classifying them as pre-breeding and post-breeding census models, and searching for three types of errors.

## Isaac
For this week reading we have MPM commentary in which the authors address the main errors made by biologist when constructing MPM. The authors also make relevant issues between two types of census: Pre-breeding and post-breeding  The three main issues are: 
•	Failing to include survival coefficients in time steps and life cycle graphs
o	The authors mention that Biologist  fail to meet assumptions of MPM model by including the wrong age measures and calculations.
•	Introducing one year delay in age of at first reproduction I post breeding census. 
o	Age at reproductive maturity (xm). In a post breeding MPM the individuals with age xm at the end of one timestep means that the individuals has already reproduce, have a age of xm-1 at the start of the next timestep. A model using xm as the age to be associated with the fertility coefficient creates a one year delay which mislead the actual life history.
	The failure of including xm-1 with the fertility coefficient is means that Juveniles are not reproducing. This is a fundamental different between age structure models vs stage structure models. 
•	Failing to match the right growth rate calculation to the species life history.
o	The authors walk to what is growth rate model means and what assumption make take in consideration. This particularly helpful when estimating lamba. 
This paper was interesting and very helpful to see how small errors can affect the interpretation of models. I found myself being called out, since I definitely have an approach to models as a biologist. The authors suggests that biologists should think more as “modelers” which is great, but they also recognize that literature and textbooks may not offer a way to educate biologist on creating the type of critical thinking to address these issues. I think the conclusion is that small mistakes may have big implications if the species being model has a completely different life history. 
![image](https://user-images.githubusercontent.com/92698815/142801250-57ea1bce-82ac-48ca-98fe-4d73b7e8567e.png)

