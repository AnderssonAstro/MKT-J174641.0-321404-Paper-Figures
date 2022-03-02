# MKT J174641.0-321404 Paper Figures

 Data and Figures on the discovery of radio flares MKT J174641.0-321404, originating from M dwarf SCR1746-3214.
 
![plotGIF](https://imgur.com/q7JE37b.gif)

 
 **For Andersson et al. (2022), MNRAS submitted**
 
 The full paper is accessible online for free at: <arxiv link>

 This repo contains 3 Jupyter notebooks and the data required to reproduce all figures from the paper "Serendipitous discovery of radio flaring behaviour from a nearby M dwarf with MeerKAT". This paper marks the second M dwarf seen by MeerKAT and the second untargetted discovery of a radio flaring star by the ThunderKAT team. 
 
 If you use any data or methods from this repo, please consider citing Andersson et al. 2022 and/or this repo's DOI: <add link on release>
 
 Comments in the code are intended to guide the reader but I make no promise at perfectly readable documentation. If you have any questions please get in touch on here or at my email address (found in the paper).
 
 
 **Notebooks**
 
 - _Paper Figures.ipynb_ is the primary notebook for the paper, used for Figures 1-4, 7 and 9. This covers the radio data, MeerLICHT data, public ASAS-SN optical data and SALT spectra.
- _TIC 111898820-Mstar.ipynb_ reproduces the TESS figures for Tess Input Candidate 111898820 (the flare star), i.e. Figures 5 and 6.
 - _GuedelPlot(LD).ipynb_ reproduces Figure 8. **NB: this is a copy of** https://github.com/AstroLaura/GuedelPlot with permission and discussion with LD, plus the data to put the X-ray and radio data of MKT J174641.0-321404 on the plot. Please cite the above, separate GitHub repo when using this plot.
 
 
 **Data**
 
 - 11 arcminute cutouts of MeerKAT (ThunderKAT) data for Figure 2 in Data/Epochs/
 - Radio (2138_ra266...) and optical (ASAS-SN lightcurve.csv, tess2021...) light curves, from MeerKAT (processed by [TraP](https://tkp.readthedocs.io/en/latest/)), [ASAS-SN](https://asas-sn.osu.edu/) and [TESS](https://mast.stsci.edu/portal/Mashup/Clients/Mast/Portal.html) respectively.
 - Two SALT spectra, in .fits format (beginning mbgphR...) and .csv format.
 - An 8x8 arcsecond cutout from MeerLICHT, along with the appropriate catalog from the original image (ML1_q_red_cat.fits). From this catalog you can get the closest-match optical coordinates.
 - Two TraP 'runningcatalog' outputs, one for the first untargetted run, one for the monitored run. These are how we found the source.
 - Additional 3-minute imaging of the brightest 15-min epoch: a TraP light curve and 5 images around the star.
 - Additional data in the form of the PyBDSF output logs (see the readme therein for more) and PyHammer logs and results (likewise). Provided for completeness, not loaded into the notebooks at any time.
 
 **Software**
 
 This notebook is written in Python3.7. Compatibility with 2.7 has not been attempted and is left as an exercise for the reader. Below are the relevant third party packages, in rough order of importance. Everything should run with the below versions, no further tests have been attempted. I have run into issues when using astropy v4.**3**.1 when handling the EW calculations in the spectral data so look out for that.
 - astropy v4.2.1
 - matplotlib v3.3.4
 - lightkurve v2.0.11
 - pybdsf v1.9.2
 - pandas v1.2.1
 - numpy v1.20.2
 - specutils v1.3
