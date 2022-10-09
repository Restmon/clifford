Example for demoing a bokeh server with Binder

[![app](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Restmon/clifford/master?urlpath=panel%2Fclifford) [![badge](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Restmon/clifford/master?filepath=clifford.ipynb)

Serves the `clifford.ipynb` app on mybinder, exploring the parameter space of clifford attractors as images rendered using datashader.

Developed by @jsignell

This repo contains:

- `environment.yml` installing bokeh and nbserverproxy
- a custom serverextension (`bokehserverextension.py`) that launches bokeh server
- a `postBuild` script to enable the server extensions and install the local one
  (this last step would go away if the local extension became a proper package)
- A [panel](https://github.com/pyviz/panel) based notebook used to serve both notebook and app based deployments

![dashboard screenshot](./assets/dashboard.png)
