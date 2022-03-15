## climetlab-spml

A dataset plugin for climetlab for the dataset spml-ml.


Features
--------

In this README is a description of how to get the dataset(s) provided by the python package spml.

## Datasets description

There are two datasets: 

### 1 : `ml`
Model level fields: "u","cc","v","t","q","clwc","ciwc","w"
or access all with "all"
Download multiple dates with a list of dates.

### 2 : `sfc`
Surface fields: single file (per date) with all surface fields.

For either, see https://storage.ecmwf.europeanweather.cloud/SPML/README.html for list of dates.


## Using climetlab to access the data

See the [demo notebooks](https://github.com/mchantry/climetlab_spml/tree/main/notebooks)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mchantry/climetlab_spml/main?urlpath=lab)


- [demo_ml.ipynb](https://github.com/mchantry/climetlab_spml/tree/main/notebooks/demo_ml.ipynb)
[![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.jupyter.org/github/mchantry/climetlab_spml/blob/main/notebooks/demo_ml.ipynb) 
[![Open in colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mchantry/climetlab_spml/blob/main/notebooks/demo_ml.ipynb) 
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mchantry/climetlab_spml/main?filepath=notebooks/demo_ml.ipynb)
[<img src="https://deepnote.com/buttons/launch-in-deepnote-small.svg">](https://deepnote.com/launch?name=MyProject&url=https://github.com/mchantry/climetlab_spml/tree/main/notebooks/demo_ml.ipynb)


- TODO.


The climetlab python package allows easy access to the data with a few lines of code such as:
``` python

!pip install climetlab climetlab-spml
import climetlab as cml
ds = cml.load_dataset("spml-ml", date="20180701",parameter="all")
!or
ds = cml.load_dataset("spml-sfc", date="20180701")
ds.to_xarray()
```


Support and contributing
------------------------

Either open a issue on github if this is a github repository, or send an email to email@example.com.

LICENSE
-------

See the LICENSE file.
(C) Copyright 2022 European Centre for Medium-Range Weather Forecasts.
This software is licensed under the terms of the Apache Licence Version 2.0
which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
In applying this licence, ECMWF does not waive the privileges and immunities
granted to it by virtue of its status as an intergovernmental organisation
nor does it submit to any jurisdiction.

Authors
-------

Matthew Chantry and al.

See also the CONTRIBUTORS.md file.
