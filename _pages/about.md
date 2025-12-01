---
permalink: /
excerpt: "Keir K. Rogers's academic webpage"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I'm a cosmologist who is a Proleptic Senior Lecturer in Physics and a UKRI STFC Ernest Rutherford Fellow at [King's College London](https://www.kcl.ac.uk/research/theoretical-particle-physics-cosmology). I previously held the fellowship at [Imperial College London](https://www.imperial.ac.uk/astrophysics). Before that, I was a [Dunlap Fellow](https://www.dunlap.utoronto.ca) at the University of Toronto and a postdoctoral fellow at the [Oskar Klein Centre for Cosmoparticle Physics](http://www.okc.albanova.se) at Stockholm University. I defended my PhD thesis ([*A clear view of the primordial Universe*](https://discovery.ucl.ac.uk/id/eprint/10044716)) at [University College London](https://www.ucl.ac.uk/astrophysics), after obtaining my Master's degree at the [University of Oxford](https://www2.physics.ox.ac.uk).

My research focuses on understanding fundamental physics in the cosmological model -- and developing robust statistical and artificial intelligence/machine learning models and methods to improve parameter inference. In particular, I have worked on tests of dark matter models (ultra-light axions, light dark matter) using cosmological data. I study the cosmic microwave background (CMB -- the oldest light in the Universe), the large-scale structure and the sub-structure of the Milky Way. I work at the intersection of data, theory, simulations and analysis methods, for example, with cosmological emulators, wavelet decomposition and simulation-based inference.

Above, you can find links to my publications list on INSPIRE-HEP, to my *curriculum vitae*, to a website collating astrophysical limits on dark matter, and to clean maps of the CMB that I created using a novel component separation method.

Below, you can find out more about some of my research.

## Ultra-light axions and cosmological tensions
<img src='/images/linear_power_log_m28_24_zoom27.png'>

Ultra-light axions are well-motivated dark matter and dark energy particle candidates that have *extremely* low masses -- somewhere between 10<sup>-32</sup> eV and 10<sup>-18</sup> eV. I set out to see what fraction of the Universe's energy budget can consist of axions using all the CMB and spectroscopic galaxy data that we currently have. I found that axions cannot be more than 1% of the dark matter if their mass is between 10<sup>-30</sup> eV and 10<sup>-28</sup> eV or more than 10% if their mass is less than 10<sup>-26</sup> eV. But, it turns out that there is just enough axions allowed to help resolve a growing cosmological parameter discrepancy: the *S*<sub>8</sub> tension. The plot above illustrates how axions suppress the clustering of matter in just the right way to maintain consistency with the large-scale modes probed by current CMB data and to give lower values of *S*<sub>8</sub> that large-scale structure probes prefer.

## Dark matter
<img src='/images/comparisonUS.png'>

I used the Lyman-alpha forest to place a strong bound on the canonical mass range for ultra-light axions to be the dark matter (ULADM; "fuzzy dark matter"). The plot above compares my new Lyman-alpha forest bound to previous efforts. The mass range of 10<sup>-22</sup> eV to 10<sup>-21</sup> eV, motivated by the string axiverse and solutions to possible tensions in the cold dark matter model, is heavily disfavoured in our study. The study looked for the characteristic cut-off in the matter power spectrum associated with ULADM as traced by the Lyman-alpha forest. Its non-detection placed a 95% credibility upper limit on the axion mass at 2 x 10<sup>-20</sup> eV. I am also in collaborations using CMB and galaxy data to look for mixed axion dark matter as suggested by the string axiverse.

<img src='/images/scale_new4.png'>

Direct detection of dark matter using nuclear recoil is limited to dark matter particles heavier than about a GeV. But, cosmological data can set strong bounds on lighter, sub-GeV dark matter by looking for the imprint of dark matter - baryon collisions in the early Universe. The plot above shows how the scale of this imprint depends on dark matter particle mass and cross section. I lead a study that set the strongest bounds to-date on this well-motivated model space.

In order to use the Lyman-alpha forest to test the nature of the dark matter, it is necessary to construct a statistically-robust way to use computationally-expensive hydrodynamical simulations. In order to do this, I constructed a general framework for dark matter model bounds. This includes a Bayesian-optimised emulator for the Lyman-alpha forest flux power spectrum as a function of the scale and shape of the power spectrum cut-off and nuisance astrophysical and cosmological parameters. This framework can now also be applied to other DM models, like warm dark matter.

## Emulators & Bayesian optimisation
<img src='/images/Bayesian_optimisation_annotated.png'>

Emulators are an ML-based model for predicting the output of simulations. Gaussian processes provide a powerful emulator model, probabilistically interpolating between an efficiently-sampled training set of simulations. I worked in teams developing an emulator for cosmological analyses using the Lyman-alpha forest. This is targeted towards realising competitive constraints on extended cosmological models in next-generation Lyman-alpha forest surveys like the Dark Energy Spectroscopic Instrument.

In particular, I worked on applying active learning to constructing emulators for cosmological analyses. The plot above illustrates how active learning works using a simple toy problem. This entails iteratively building up the training set, maximising a combination of sampling high posterior probability parameter space and reducing uncertainty in the emulator prediction. This leads to two major advantages. Tests of convergence in parameter inference with respect to the emulator model can be carried out. Further, it makes the use of emulators feasible in high-dimensional physical models by efficient sampling of parameter space. This is very important for large-scale structure studies, where forward modelling is computationally expensive and there are many free parameters.

## Cosmic microwave background
<img src='/images/block_diagram_illustrator.png'>

A limiting factor in measuring the primordial inflationary tensor modes in the CMB is contamination from polarised dust emission in the Milky Way. I studied the problem of removing this contamination using a signal processing technique called spin-directional wavelets. The plot above shows how these wavelets are used to reconstruct the CMB *E* and *B* polarisation modes. I was able for the first time to exploit morphological information in the filamentary structure of dust emission to improve the reconstruction of the primordial signal. This can help to achieve the goal of improving the tensor-to-scalar mode ratio and neutrino mass sensitivities in next-generation, higher S/N CMB experiments like the Simons Observatory and CMB-S4. You can find more details and the cleaned *Planck* data products [here](http://www.silc-cmb.org).

## High-density absorbers in the IGM
<img src='/images/contaminant_power_absolute_1D_limit_z_2_00_only2.png'>

High column density (HCD) hydrogen absorption, if incorrectly modelled, can bias our inference on cosmological parameters using the Lyman-alpha forest. I developed a model to mitigate this effect using the *Illustris* cosmological hydrodynamical simulation. The plot above shows the relative contribution of each type of high-density absorber to the Lyman-alpha forest power spectrum in *Illustris*. The model that is used to mitigate contamination accounts for the modification to the column density distribution function caused by the process of pre-screening the most prominent absorbers in quasar spectra. It has been used to check for HCD contamination in the latest (e)BOSS analyses of both the 1D power spectrum and 3D correlation function of the Lyman-alpha forest flux.
