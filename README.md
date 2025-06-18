# Spectra Reduction school project
This project demonstrates a comprehensive data analysis pipeline for reducing astronomical spectra, starting from raw spectrometer output and culminating in a clean, calibrated visual representation of the spectrum. The process was carried out as part of an academic lab assignment, highlighting core competencies in data wrangling, signal processing, and scientific visualization.


The goal is to transform raw CCD data from a spectrometer into a scientifically meaningful 1D spectrum, corrected for instrumental and environmental effects. The final output allows for the identification of spectral lines and comparison to theoretical models.
Spectral data is messy by nature, and turning it into something usable requires a strong grasp of both the physics and data processing. This project highlights:

    Real-world data cleaning and calibration

    Working with FITS files and astronomical data formats

    Handling multi-step preprocessing workflows

    Visual storytelling through scientific plots

Key Steps Involve: 

    Raw Data Loading

        Imported FITS files from a spectrometer

        Extracted metadata and pixel data using astropy.io.fits

    Preprocessing & Cleaning

        Bias subtraction

        Dark current removal

        Flat-field correction
        
        Removing cosmic rays

    Extraction of the Spectrum

        Collapsing a 2D CCD image into a 1D spectrum

        Background subtraction

    Wavelength Calibration

        Used known emission lines

        Fitted a polynomial solution to map pixel index to wavelength

     Calibration

        Adjusted for instrument sensitivity

    Data Visualization

        Plotted the final reduced spectrum with wavelength on the x-axis and flux on the y-axis


Tools & Libraries Used

    Python

    NumPy, SciPy

    Astropy 

    Matplotlib for data visualization

    Ccdproc
Included are file outputs and a notebook
Use https://nbviewer.org/ to view the notebook
