# ESAC Astropy Course - October 23-25 2019

## If you are short on time

Before we go over the installation instructions, if you don't have time or are
not able to install the software on your laptop in time for the workshop, you
can use the notebooks online instead by clicking on the following button:

LINK

If this works, just ignore the rest of this README!

## Notebooks

To download the notebooks to your laptop, run:

    git clone https://github.com/aperiosoftware/esac-astropy.git

If this does not work for any reason, download [this zip file](LINK) instead.
In both cases, once you have downloaded this, go inside the ``esac-astropy``
folder before proceeding to the next section:

    cd esac-astropy

## Requirements and installation

To run all the notebooks on your laptop, you will need the following software
installed:

* Python 3.5 or later
* Jupyter Notebook
* Numpy
* Matplotlib
* SciPy
* Astropy 3.2 or later
* reproject
* photutils
* regions
* astropy-healpix
* astroquery
* APLpy
* PyVO

If you have never used Python before, we recommend downloading the [Miniconda
distribution](https://docs.conda.io/en/latest/miniconda.html) and installing it
then following the steps for **Option 1: If you use conda** below.

### Option 1: If you use conda

If you use conda, the easiest way to get set up quickly is to create a new
environment with all the required dependencies by running:

    conda create -n astropy-workshop -f environment.yml

Anytime you want to switch to this environment, you can then do:

    conda activate astropy-course

(if this doesn't work, try ``source activate py37``).

If you want to start using any of the packages in your regular environment after
the workshop, see the **Option 3: Manual conda installation** section.

### Option 2: If you use pip

If you normally use pip to manage your dependencies, provided that you are using
Python 3.5 or later you can install all the required dependencies by running:

    pip install -r requirements.txt

If you prefer to install dependencies individually, see the **Option 4: Manual
pip insallation** section.

### Option 3: Manual conda installation

If you want to install the packages into an existing conda environment, make
sure that environment has Python 3.5 or later installed, then run:

    conda install notebook numpy matplotlib scipy "astropy>=3.2"
    conda install -c astropy reproject photutils astropy-healpix regions astroquery aplpy
    pip install PyVO

You can remove any packages from this list that you do not want to install.

### Option 4: Manual pip installation

If you want to install the packages into an existing Python environment with
pip, make sure that environment has Python 3.5 or later installed, then run:

    pip install notebook numpy matplotlib scipy "astropy>=3.2"
    pip install reproject photutils astropy-healpix regions astroquery aplpy PyVO

You can remove any packages from this list that you do not want to install.

## Launching the notebooks

Once you have followed one of the installation options above, you can start
up the notebook server by running:

    jupyter notebook
