The assignment questions are given below. There are three parts. You can find any files you need in this repo. Please push your answers to the version of this repo that was created when you accepted the classroom invite on Github classroom. You can either submit one file for each, or a single file that contains all the answers (either a pdf or a .md file, complete with images). The deadline is April 27th.

As an aside, this .md file was created using a nice github app called TeXify (https://github.com/apps/texify), a GitHub app that looks in your pushes for files with extension *.tex.md and turns them into rendered .md files.

### Here is part 1 of the assignment:

Use the Urn model starting with 2 red balls of weight 1, and one black (mutation) ball of weight w.

Draw balls until you have 10 non-black balls. Implement the rejection method to answer the following questions:

Assuming a Uniform[0,20] prior for the weight of the black ball, if all non-black balls are the same color at the end, what is the posterior distribution of the weight of the black ball?

Assuming a Uniform[0,20] prior for the weight of the black ball, if there are exactly two non-black balls are the same color at the end, what is the posterior distribution of the weight of the black ball?

## Here is part 2 of the assignment:

Repeat part 1 of the assignment, but this time just to find the posterior distribution for the weight of the black ball if we observe just one non-black color at the end.

But this time sample the weights, $\theta'$ using an $expo(\lamba)$ distribution, rather than a $Unif[0,20]$ distribution.

We are now doing importance sampling, so if you accept the value of $\theta'$, because the simulated urn had just one non-black color in it, then you need to add a mass of $\pi(\theta')/\psi(\theta')$ to the posterior distribution of $\theta'$ (whereas we used to add a mass of 1).

Remember to truncate the expo at 20, to match the domain of the prior dsistribution $\pi$ (and to allow for thius when you evaluate $\psi(\theta')$.

Compare the efficiency of this algorithm to that pf the pure rejection method you used in part 1. (How many iterations are required to get 1000 accepted values, say?)

Many tissues contain 2 (or more) cell-types.

## Here is part 3 of the assignment:

Many tissues contain 2 (or more) cell-types. An investigator wants a way of testing whether each of 2 cell types in a given tissue is homogeneously distributed (in space). So:

$H_0$: cell types are homogeneously (randomly) arranged
$H_1$: cell types are not homogeneously arranged (i.e. they are clustered in some fashion).

Your job is to come up with such a test, using Monte Carlo methods.

1. Formulate your test.

2. Apply it to each of Grid1, Grid2, Grid3 and determine a p-value for rejecting the $H_0$ in favor of $H_1$.

3. Write-up your test (i.e. Methods) and your Results as an Markdown file.
