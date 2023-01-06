# ERS_NIRCam
Demonstration to duplicate the data reduction of a transit of WASP-39b observed with NIRCam/F322W2 as part of the JWST Transiting Exoplanet Early Release Science Program (ERS 1366). This demonstration follows the data reduction with Eureka! presented in Ahrer et al. (2022). Reduction demo DOI: https://doi.org/10.5281/zenodo.7510106

Run the following commands to get started! These commands set up an environment with Eureka! v0.6 - see the Eureka! documentation at https://eurekadocs.readthedocs.io/en/latest/index.html for more information.

```
conda create -n ers-nircam python==3.9.7
conda activate ers-nircam
git clone -b v0.8 https://github.com/kevin218/Eureka.git
cd Eureka
pip install -e '.[jwst]'
cd ..
conda install jupyter
pip install stcal[opencv]
ipython kernel install --user --name=ers-nircam
```

Ensure you are in the correct environment with ```conda env list```!

When opening the demo Jupyter Notebook, check to make sure that you are in the correct kernel by making sure the right-hand corner of the notebook says ```ers-nircam'''. If it doesn't, select the menu options Kernel --> Change kernel --> ers-nircam.
