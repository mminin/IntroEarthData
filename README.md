# CH05-210103-IntroEarthData

* [Links and resources](resources.md)
* [Sample data](sample_data.md)
* [Libraries and modules](libraries.md)
* Notebooks
  * [CH05-210103_00-general-intro.ipynb](notebooks/CH05-210103_00-general-intro.ipynb)
  * [CH05-210103_01-basics.ipynb](notebooks/CH05-210103_01-basics.ipynb)
  * [CH05-210103_02-data-Intro.ipynb](notebooks/CH05-210103_02-data-Intro.ipynb)
  * [CH05-210103_03-archives.ipynb](notebooks/CH05-210103_02-data-Intro.ipynb)
  * [CH05-210103_04-data-load.ipynb](notebooks/CH05-210103_04-data-load.ipynb)
  * [CH05-210103_05-data-handling-analysis-1D.ipynb](notebooks/CH05-210103_05-data-handling-analysis-1D.ipynb)
  * [CH05-210103_06-data-handling-analysis-2D.ipynb](notebooks/CH05-210103_06-data-handling-analysis-2D.ipynb)

To use [Anaconda](http://anaconda.com/) with the notebooks above, please create a new environment with [introearth.yml](introearth.yml). There might be the need, depending on platform of few fixes and troubleshooting. Some manual setup, e.g. with [owslib fork](https://github.com/earthserver-eu/OWSLib) could be needed, e.g. from within the environment ```introearth```, i.e.

```
source activate introearth
```
and then:
```
git clone https://github.com/earthserver-eu/OWSLib.git
cd OWSLib
git checkout olcl-wcs-200
python setup.py install
```
this should also achieve the same:

```
pip install git+https://github.com/earthserver-eu/OWSLib@olcl-wcs-200
```

--- 
with miniconda on mac computers one might need to set also:

```
export PATH="/Users/<your_home_directory>/miniconda/bin:$PATH
export LC_ALL=en_US.UTF-8 && export LANG=en_US.UTF-8"
```
one possible solution is to create an alias, i.e. add those lines to your ```.bashrc```:

```
alias anaconda="export PATH="/Users/<your_home_directory>/miniconda/bin:$PATH" && \
export LC_ALL=en_US.UTF-8 && export LANG=en_US.UTF-8"
```
