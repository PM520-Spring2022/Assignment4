The assignment questions are given below. TYou can find any files you need in this repo. Please push your answers to the version of this repo that was created when you accepted the classroom invite on Github classroom. You can either submit one file for each, or a single file that contains all the answers (either a pdf or a .md file, complete with images). The deadline is April 27th.

Assignment4
There are two parts to assignment 4. Please upload your answers to your clone of this repo.

Here is part 1 of the assignment:
Use the Urn model starting with 2 red balls of weight 1, and one black (mutation) ball of weight w.

Draw balls until you have 10 non-black balls. Implement the rejection method to answer the following questions:

Assuming a Uniform[0,20] prior for the weight of the black ball, if all non-black balls are the same color at the end, what is the posterior distribution of the weight of the black ball?

Assuming a Uniform[0,20] prior for the weight of the black ball, if there are exactly two non-black balls are the same color at the end, what is the posterior distribution of the weight of the black ball?

Here is part 2 of the assignment:
Repeat part 1 of the assignment, but this time just to find the posterior distribution for the weight of the black ball if we observe just one non-black color at the end.
But this time sample the weights, $\theta'$ using an expo($lamba$) distribution, rather than a Uniform[0,20] distribution.
We are now doing importance sampling, so if you accept the value of $\theta'$, because the simulated urn had just one non-black color in it, then you need to add a mass of $\pi(\theta')/\psi(\theta') to the posterior distribution of $\theta'$ (whereas we used to add a mass of 1.
Remember to truncate the expo at 20, to match the domain of the prior dsistribution $\pi$ (and to allow for thius when you evaluate $\psi(\theta')$.
compare the efficiency of this algorithm to that pf the pure rejection method you used in part 1. (How many iterations are required to get 1000 accepted values, say?)
