# Commentary on Kendall et al. 2019






## Rachael 
Matrix population models (MPMs) have been presented as a way to turn life-history information into a quantitative form, but the authors argue that even published MPMs contain errors. They talk about how b_x (birth rate at age x) can't be a matrix element because it doesn't span a timestep. They then explain post-breeding census modeling is when F(x) = sigma_x * b_x' is F(x) = parent survival * birthrate for individuals aged x'. When you let x_m be age at first reproduction, and the individuals are age x_m at the end of the timestep - they just reproduced for the first time, meaning they were age x_(m-1) at the beginning of the timestep - you need to ensure you don't mess up the placement of the first nonzero fertility coefficient. It seems that the most common error is thinking it is one ahead of where it actually is, so they suggest F_xm = sigma_xm * b_xm, which is basically focusing on age at the end of the time step. This approach doesn't translate over to stage-structured model formulations, though. The depictions of intuitive v. correct stage-structured models were helpful in trying to understand this part. They then discussed the challenges of estimating gamma_i, the fraction of individuals who end up exiting stage i. A large portion of the paper is about assessing a set of studies that use MPMs, classifying them as pre-breeding and post-breeding census models, and searching for three types of errors.
