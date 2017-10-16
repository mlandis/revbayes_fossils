# RevBayes: Analysis of Fossil and Molecular Data

## Instructors: Rachel Warnock and Michael Landis

### General Information
This workshop is a 3-hour session, held on October 21, 2017 at the [Geological Society of America Annual Conference in Seattle, WA USA](http://community.geosociety.org/gsa2017/home). 

This half-day workshop will guide participants through the theory and practice of combined inference of dated phylogenies using fossil and molecular data. For this workshop, participants should attend the RevBayes Introduction workshop or have previous experience using RevBayes. We will cover the background necessary to understand the fossilized birth-death process, relaxed clock models, and discrete morphological evolution. The tutorial provided will demonstrate how to perform a "total-evidence analysis" on a provided dataset. Additionally, participants can bring their own data to analyze.  

### Contact Information

* Rachel Warnock: `rachel dot warnock at bsse dot ethz dot ch`
* Michael Landis: `michael dot landis at yale dot edu`

## Background Material

This workshop covers a very complicated analysis that requires the participants to specify complex statistical models. Unfortunately, the three-hour workshop will not afford enough time for us to review everything in detail. Yet, because of the challenging material, we expect all participants to have some previous experience with Bayesian phylogenetics before attending the workshop. Below is a list of papers and tutorials to help prepare those who are interested:

Papers:

>Heath, T. A., Huelsenbeck, J. P., & Stadler, T. (2014). The fossilized birth–death process for coherent calibration of divergence-time estimates. Proceedings of the National Academy of Sciences, 111(29), E2957-E2966. [pdf](http://www.pnas.org/content/111/29/E2957.full.pdf)

>Ronquist, F., Klopfstein, S., Vilhelmsen, L., Schulmeister, S., Murray, D. L., & Rasnitsyn, A. P. (2012). A total-evidence approach to dating with fossils, applied to the early radiation of the Hymenoptera. Systematic Biology, 61(6), 973-999. [pdf](https://academic.oup.com/sysbio/article-pdf/61/6/973/17830528/sys058.pdf)

>Gavryushkina, A., Heath, T. A., Ksepka, D. T., Stadler, T., Welch, D., & Drummond, A. J. (2017). Bayesian total-evidence dating reveals the recent crown radiation of penguins. Systematic biology, 66(1), 57-73. [pdf](https://academic.oup.com/sysbio/article-pdf/66/1/57/19609000/syw060.pdf)




Tutorials:
> Basic Introduction to Rev and MCMC ([tutorial PDF](https://github.com/ssb2017/revbayes_intro/blob/master/tutorials/RB_Basics_Tutorial.pdf))

> Introduction to MCMC Simulation ([tutorial PDF](https://github.com/revbayes/revbayes_tutorial/blob/master/tutorial_TeX/RB_MCMC_Intro_Tutorial/RB_MCMC_Intro_Tutorial.pdf))

> Substitution Models for Time-Constrained Trees ([tutorial pdf](https://github.com/ssb2017/revbayes_intro/blob/master/tutorials/RB_CTMC_Tutorial.pdf))

> Partitioned Data Analysis ([tutorial pdf](https://github.com/ssb2017/revbayes_intro/blob/master/tutorials/RB_Partition_Tutorial.pdf))

> *Optional*: Model Selection using Bayes Factors ([tutorial pdf](https://github.com/ssb2017/revbayes_intro/blob/master/tutorials/RB_BayesFactor_Tutorial.pdf))




## Install RevBayes

This workshop will use RevBayes v1.0.6. It can be downloaded from [the latest release](https://github.com/revbayes/revbayes/releases/tag/v1.0.6-release) for Windows 7 or higher or for Mac OSX 10.6 or higher. For Unix systems, you can clone the source code from [https://github.com/revbayes/revbayes](https://github.com/revbayes/revbayes).

## Accessory Programs

The RevBayes workshops will also use additional for analysis of output and summarization of the MCMC. Please download and install the following:

* Tracer ([http://tree.bio.ed.ac.uk/software/tracer/](http://tree.bio.ed.ac.uk/software/tracer/))
* FigTree ([http://tree.bio.ed.ac.uk/software/figtree/](http://tree.bio.ed.ac.uk/software/figtree/))
* IcyTree (a web-based tree viewer; [http://tgvaughan.github.io/icytree/](http://tgvaughan.github.io/icytree))
* Text editors
	* Mac OSX: [TextWrangler](http://www.barebones.com/products/TextWrangler/), [Sublime Text](https://www.sublimetext.com/)
	* Windows: [Notepad++](https://notepad-plus-plus.org/), [Sublime Text](https://www.sublimetext.com/)
	* Linux: [Geany](https://www.geany.org/), [Sublime Text](https://www.sublimetext.com/)

## Workshop Outline
### Background and Theory

[ Slides not yet available. ]

The course will consist of a brief overview of the models and statistical methods for conducting a total-evidence analysis under the fossilized birth-death model in RevBayes. We will focus on the following models:

* Stochastic branching processes as tree priors, with particular emphasis on the fossilized birth-death model (FBD)
* Models of lineage-specific substitution rates (or rates of morphological change)
* Models of discrete morphological character change and accounting for acquisition biases

### Tutorial
After presenting the theoretical background, we will lead a hands-on tutorial using an empirical dataset. This exercise will demonstrate:

* Importing multiple data matrices in RevBayes
* Creating clade constraints
* Specification of the FBD model
* Sampling fossil occurrence dates from known age ranges
* Setting up the uncorrelated lognormal model for relaxing the molecular clock
* Defining the parameters of the GTR+G model of sequence evolution
* Applying a strict clock to the rates of morphological evolution
* Defining the parameters of the Mk model of discrete morphological character evolution while accounting for sampling only variable characters
* Executing an MCMC sampler in RevBayes
* Summarizing and evaluating the marginal posterior samples of various model parameters
* Summarizing a fossilized birth-death tree with sampled ancestors

The next section provides specific details for locating the tutorial exercise and associated files.


## Exercise: Estimating the Phylogeny and Divergence Times of Fossil and Extant Bears

This tutorial is maintained on the RevBayes tutorial repository ([https://github.com/revbayes/revbayes_tutorial](https://github.com/revbayes/revbayes_tutorial)). On this site you can find a wide range of tutorials for different RevBayes analyses. 

### Download the Files

For this workshop, it is recommended that you create a working directory on your computer. You can call this `RB_TotalEvidence_FBD_Tutorial`.

In `RB_TotalEvidence_FBD_Tutorial` download the data files and uncompress the zipped archives:

* [`data.zip`](https://github.com/revbayes/revbayes_tutorial/raw/master/RB_TotalEvidenceDating_FBD_Tutorial/data.zip) 

Also download the detailed tutorial document:

* [`RB_TotalEvidenceDating_FBD_Tutorial.pdf`](https://github.com/revbayes/revbayes_tutorial/raw/master/tutorial_TeX/RB_TotalEvidenceDating_FBD_Tutorial/RB_TotalEvidenceDating_FBD_Tutorial.pdf) 

### Getting Started

Now that you have all the files and installed the software, execute RevBayes and follow the tutorial exercise. If you have any trouble, please ask for help. 
