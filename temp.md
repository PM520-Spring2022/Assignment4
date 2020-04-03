The assignment questions are given below. TYou can find any files you need in this repo. Please push your answers to the version of this repo that was created when you accepted the classroom invite on Github classroom. You can either submit one file for each, or a single file that contains all the answers (either a pdf or a .md file, complete with images). The deadline is April 27th.

Assignment4

There are two parts to assignment 4. Please upload your answers to your clone of this repo.

## Here is part 1 of the assignment:

Use the Urn model starting with 2 red balls of weight 1, and one black (mutation) ball of weight w.

Draw balls until you have 10 non-black balls. Implement the rejection method to answer the following questions:

Assuming a Uniform[0,20] prior for the weight of the black ball, if all non-black balls are the same color at the end, what is the posterior distribution of the weight of the black ball?

Assuming a Uniform[0,20] prior for the weight of the black ball, if there are exactly two non-black balls are the same color at the end, what is the posterior distribution of the weight of the black ball?

## Here is part 2 of the assignment:

Repeat part 1 of the assignment, but this time just to find the posterior distribution for the weight of the black ball if we observe just one non-black color at the end.
But this time sample the weights, <img src="/tex/a0636197f9b37d9928c1c149816cd7dc.svg?invert_in_darkmode&sanitize=true" align=middle width=11.96348834999999pt height=24.7161288pt/> using an expo(<img src="/tex/73329a120aa2f3d674600e682659c3bb.svg?invert_in_darkmode&sanitize=true" align=middle width=44.09455049999999pt height=22.831056599999986pt/>) distribution, rather than a Uniform[0,20] distribution.
We are now doing importance sampling, so if you accept the value of <img src="/tex/a0636197f9b37d9928c1c149816cd7dc.svg?invert_in_darkmode&sanitize=true" align=middle width=11.96348834999999pt height=24.7161288pt/>, because the simulated urn had just one non-black color in it, then you need to add a mass of <img src="/tex/b710bdebc5f29bc7fd7339a1532d21e3.svg?invert_in_darkmode&sanitize=true" align=middle width=289.57730999999995pt height=24.7161288pt/>\theta'<img src="/tex/9410d7acd9bb698c5421124afd3f9441.svg?invert_in_darkmode&sanitize=true" align=middle width=800.0883560999999pt height=24.65753399999998pt/>\pi<img src="/tex/dd8802c0539c9324818a8802ad3181fe.svg?invert_in_darkmode&sanitize=true" align=middle width=277.62785489999993pt height=24.65753399999998pt/>\psi(\theta')$.
compare the efficiency of this algorithm to that pf the pure rejection method you used in part 1. (How many iterations are required to get 1000 accepted values, say?)
