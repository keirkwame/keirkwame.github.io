---
permalink: /
excerpt: "Keir K. Rogers's academic webpage"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I'm a cosmologist who started a [Dunlap Fellowship](https://www.dunlap.utoronto.ca/people/dunlap-fellows) at the end of 2020.

I'm interested in testing new cosmological models using large and complex datasets -- and developing novel statistical & machine learning methods to improve that inference. I'm currently working on tests of dark matter models (in particular, axions) using cosmological data. I study the cosmic microwave background -- the bath of (polarised) photons from the early Universe -- and large-scale structure -- specifically the Lyman-alpha forest, the absorption lines from neutral gas in the early Universe observed in the spectra of distant quasars. The range of scales and redshifts probed by these two complementary observations allows us to test many extensions to the standard cosmological model -- for example, the properties of neutrinos, models of cosmic inflation or the phenomenology of dark matter.

Above, you can see a link to my publications list on the arXiv -- and a link to an outreach article I wrote about some of my research: A clear view of the primordial Universe.

## Dark matter
I worked with the Lyman-alpha forest to place a strong bound on the canonical mass range for ultra-light axions to be the dark matter (ULADM; "fuzzy dark matter"). The mass range of 10<sup>-22</sup> eV to 10<sup>-21</sup> eV, motivated by the string axiverse and solutions to possible tensions in the cold dark matter model, is heavily disfavoured in our study. The study looked for the characteristic cut-off in the matter power spectrum associated with ULADM as traced by the Lyman-alpha forest. Its non-detection placed a 95% credibility upper limit on the axion mass at 2 x 10<sup>-20</sup> eV.

In order to use the Lyman-alpha forest to test the nature of the dark matter, it is necessary to construct a statistically-robust way to use computationally-expensive hydrodynamical simulations. In order to do this, I constructed a general framework for dark matter model bounds. This includes a Bayesian-optimised emulator for the Lyman-alpha forest flux power spectrum as a function of the scale and shape of the power spectrum cut-off and nuisance astrophysical and cosmological parameters. This framework can now also be applied to other DM models, like warm dark matter or light (sub-GeV) DM-baryon scattering.

## Emulators & Bayesian optimisation
Emulators are an ML-based model for predicting the output of simulations. Gaussian processes provide a powerful emulator model, probabilistically interpolating between an efficiently-sampled training set of simulations. I worked in teams developing an emulator for cosmological analyses using the Lyman-alpha forest. This is targetted towards realising competitive constraints on extended cosmological models in next-generation Lyman-alpha forest surveys like the Dark Energy Spectroscopic Instrument.

In particular, I worked on applying Bayesian optimisation to constructing emulators for cosmological analyses. This entails iteratively building up the training set, maximising a combination of sampling high posterior probability parameter space and reducing uncertainty in the emulator prediction. This leads to two major advantages. Tests of convergence in parameter inference with respect to the emulator model can be carried out. Further, it makes the use of emulators feasible in high-dimensional physical models by efficient sampling of parameter space. This is very important for large-scale structure studies, where forward modelling is computationally expensive and there are many free parameters.

## Cosmic microwave background
A limiting factor in measuring the primordial inflationary tensor modes in the CMB is contamination from polarised dust emission in the Milky Way. I studied the problem of removing this contamination using a signal processing technique called spin-directional wavelets. These were able for the first time to exploit morphological information in the filamentary structure of dust emission to improve the reconstruction of the primordial signal. This can help to achieve the goal of improving the tensor-to-scalar mode ratio and neutrino mass sensitivities in next-generation, higher S/N CMB experiments like the Simons Observatory and CMB-S4. You can find more details and the cleaned *Planck* data products [here](http://www.silc-cmb.org).

## High-density absorbers in the IGM
High column density (HCD) hydrogen absorption, if incorrectly modelled, can bias our inference on cosmological parameters using the Lyman-alpha forest. I developed a model to mitigate this effect using the *Illustris* cosmological hydrodynamical simulation. The model accounts for the modification to the column density distribution function caused by the process of pre-screening the most prominent absorbers in quasar spectra. It has been used to check for HCD contamination in the latest (e)BOSS analyses of both the 1D power function and 3D correlation function of the Lyman-alpha forest flux.