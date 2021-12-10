# MKT J174641.0-321404 Paper Figures

 Data and Figures on the discovery of radio flares MKT J174641.0-321404, originating from M dwarf SCR1746-3214.
 
![plotGIF](https://imgur.com/q7JE37b.gif)

 
 **For Andersson et al. (2022), MNRAS submitted**
 
 The full paper is accessible online for free at: <arxiv link>

 This repo contains 3 Jupyter notebooks and the data required to reproduce all figures from the paper "Serendipitous discovery of radio flaring behaviour from a nearby M dwarf with MeerKAT". Comments in the code are intended to guide the reader but I make no promise at perfectly readable documentation. If you do have any questions please get in touch. 
 
 
 **Notebooks**
 - _Paper Figures.ipynb_ is the primary notebook for the paper, used for Figures 1-4, 7 and 9. This covers the radio data, MeerLICHT data, public ASAS-SN optical data and SALT spectra.
- _TIC 111898820-Mstar.ipynb_ reproduces the TESS figures for Tess Input Candidate 111898820 (the flare star), i.e. Figures 5 and 6.
 - _GuedelPlot.ipynb_ reproduces Figure 8. **NB: this is a copy of** https://github.com/AstroLaura/GuedelPlot with permission and discussion with LND, plus the data to put the X-ray and radio data of MKT J174641.0-321404 on the plot. Please cite the above, separate GitHub repo when using this plot.
 
 **Software**
 This notebook is written in Python3.8. Compatibility with 2.7 has not been attempted and is left as an exercise for the reader. Below are the relevant third party packages, in rough order of importance:
 - astropy v4.3.1
 - numpy v1.21.3
 - matplotlib v3.3.4
- lightkurve v2.0.11
- pandas v1.2.4
- spectutils v1.4.1
