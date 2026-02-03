# spectra-filtering


[![image](https://img.shields.io/pypi/v/TARDIS_Spectrum_Filtering.svg)](https://pypi.python.org/pypi/TARDIS_Spectrum_Filtering)


**Package used to apply telescope filters to spectra from Stars or Supernovae**

-   Free software: MIT License

# How to import and use

-   Import using "import TARDIS_Spectrum_Filtering.Spectrum_Filtering


-   Comes with the following functions:

    -   get_url_from_config(config_file_path): Obtain the URL of the spectrum filter file from the yml config file. returns url, safename. safename can be used in the download_filter function as filename

    -   download_filter(url, filename): Download the filter into the Filters/ Directory

    -   interp_filter(spectrum_to_filter, filter_name): Interpolates the wavelengths in the filter's xml file with the wavelengths given by the spectrum so they become compatible

    -   apply_filter(spectrum, chosen_filter): Applies the filter to the spectrum, outputting a filtered spectrum

    -   plot_original_spectrum(spectrum): Plots the spectrum you input

    -   plot_filter(spectrum, chosen_filter): Plots the filter's transmission curve

    -   plot_filtered_spectrum(spectrum, chosen_filter): Plots the filtered spectrum