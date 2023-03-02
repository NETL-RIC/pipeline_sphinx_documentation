# CO2 Pipeline Tool Documentation using Sphinx
Repo for the source Sphinx files and build files for the CO2 Pipeline documentation. 

## Installation
Create a virtual environment via the yaml file, `exported_venv/environment.yml` from the root project directory. If you do not have it, download anaconda via your distro's package manager or navigating to [their website](https://www.anaconda.com/products/distribution) with your web browser.

Navigate to exported_venv, and execute the following in the anaconda terminal:

    conda env create --name sphinxpipe --file=environment.yml
    
Then activate the virtual environemnt via:

  conda activate sphinxpipe

## Contributing and Building Content
This project uses MyST parser to create new markdown content.

Add to or create markdown files following what is expected by [MyST](https://myst-parser.readthedocs.io/en/latest/index.html) and [Sphinx](https://www.sphinx-doc.org/en/master/).

To build your changes, execute the makefile on unix via `make html`, or `make.bat html` on Windows. 

## Looking at the Output Documentation

The built html files in the `_build/html` folder can be viewed with any web browser. The main page that leads to all others is index.html.
I have modified the `_build` folder to be at the same directory level as `source`, instead of the default which is inside of `source`.
