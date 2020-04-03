The assignment questions are given below. There are three parts. You can find any files you need in this repo. Please push your answers to the version of this repo that was created when you accepted the classroom invite on Github classroom. You can either submit one file for each, or a single file that contains all the answers (either a pdf or a .md file, complete with images). The deadline is April 27th.

As an aside, this .md file was created using a nice github app called TeXify (https://github.com/apps/texify), a GitHub app that looks in your pushes for files with extension *.tex.md and turns them into rendered .md files.

### Here is part 1 of the assignment:

Use the Urn model starting with 2 red balls of weight 1, and one black (mutation) ball of weight w.

Draw balls until you have 10 non-black balls. Implement the rejection method to answer the following questions:

Assuming a Uniform[0,20] prior for the weight of the black ball, if all non-black balls are the same color at the end, what is the posterior distribution of the weight of the black ball?

Assuming a Uniform[0,20] prior for the weight of the black ball, if there are exactly two non-black balls are the same color at the end, what is the posterior distribution of the weight of the black ball?

## Here is part 2 of the assignment:

Repeat part 1 of the assignment, but this time just to find the posterior distribution for the weight of the black ball if we observe just one non-black color at the end.

But this time sample the weights, <img src="/tex/a0636197f9b37d9928c1c149816cd7dc.svg?invert_in_darkmode&sanitize=true" align=middle width=11.96348834999999pt height=24.7161288pt/> using an <img src="/tex/f0a22edc5ba5f8d311cca7323e8cf491.svg?invert_in_darkmode&sanitize=true" align=middle width=46.073176049999994pt height=24.65753399999998pt/> distribution, rather than a <img src="/tex/60d6ce53e307c98314b287f932fd3d7f.svg?invert_in_darkmode&sanitize=true" align=middle width=79.45941464999999pt height=24.65753399999998pt/> distribution.

We are now doing importance sampling, so if you accept the value of <img src="/tex/a0636197f9b37d9928c1c149816cd7dc.svg?invert_in_darkmode&sanitize=true" align=middle width=11.96348834999999pt height=24.7161288pt/>, because the simulated urn had just one non-black color in it, then you need to add a mass of <img src="/tex/5c79c11b1db66c3ac4e272e81d83bd00.svg?invert_in_darkmode&sanitize=true" align=middle width=80.61855614999999pt height=24.7161288pt/> to the posterior distribution of <img src="/tex/a0636197f9b37d9928c1c149816cd7dc.svg?invert_in_darkmode&sanitize=true" align=middle width=11.96348834999999pt height=24.7161288pt/> (whereas we used to add a mass of 1).

Remember to truncate the expo at 20, to match the domain of the prior dsistribution <img src="/tex/f30fdded685c83b0e7b446aa9c9aa120.svg?invert_in_darkmode&sanitize=true" align=middle width=9.96010619999999pt height=14.15524440000002pt/> (and to allow for thius when you evaluate <img src="/tex/33086d7b21850b2bcc7ceffa0a69980a.svg?invert_in_darkmode&sanitize=true" align=middle width=36.86842334999999pt height=24.7161288pt/>.

Compare the efficiency of this algorithm to that pf the pure rejection method you used in part 1. (How many iterations are required to get 1000 accepted values, say?)

Many tissues contain 2 (or more) cell-types.

## Here is part 3 of the assignment:

Many tissues contain 2 (or more) cell-types. An investigator wants a way of testing whether each of 2 cell types in a given tissue is homogeneously distributed (in space). So:

<img src="/tex/30074edb23bec8e7c47c584ff885e5b5.svg?invert_in_darkmode&sanitize=true" align=middle width=20.21695004999999pt height=22.465723500000017pt/>: cell types are homogeneously (randomly) arranged
<img src="/tex/208fbcc5ce29722c2f701868ac31fc3c.svg?invert_in_darkmode&sanitize=true" align=middle width=20.21695004999999pt height=22.465723500000017pt/>: cell types are not homogeneously arranged (i.e. they are clustered in some fashion).

Your job is to come up with such a test, using Monte Carlo methods.

1. Formulate your test.

2. Apply it to each of Grid1, Grid2, Grid3 and determine a p-value for rejecting the <img src="/tex/30074edb23bec8e7c47c584ff885e5b5.svg?invert_in_darkmode&sanitize=true" align=middle width=20.21695004999999pt height=22.465723500000017pt/> in favor of <img src="/tex/208fbcc5ce29722c2f701868ac31fc3c.svg?invert_in_darkmode&sanitize=true" align=middle width=20.21695004999999pt height=22.465723500000017pt/>.

3. Write-up your test (i.e. Methods) and your Results as an Markdown file.
