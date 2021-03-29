# pinout

![GitHub](https://img.shields.io/github/license/j0ono0/pinout) ![GitHub last commit](https://img.shields.io/github/last-commit/j0ono0/pinout) ![Read the Docs](https://img.shields.io/readthedocs/pinout)

SVG diagram creation from Python code - **pinout** provides an easy method of creating pin-out diagrams for electronic hardware.

<p align="center">
    <img alt="Example diagram created from pinout: micropython pin-out on Adafruit Huzzah32 ESP32 Feather Board." src="docs/_static/huzzah32_pinout.png" />
</p>

Please visit [pinout.readthedocs.io](https://pinout.readthedocs.io) for the latest 'getting started' guide and detailed documentation on all options provided by the *pinout* package.

## Quick start

*pinout* provides some sample files for a quick start and demonstration of key features. 

### Install

Using a virtual environment is recommended; Start by installing the *pinout* package. Either clone this repo and pip install it or install from PyPi:
```
pip install pinout

# Or upgrade to the latest version
pip install --upgrade pinout
```

### Duplicate sample files

A normal pinout diagram will ultimately include an SVG file, an image of hardware to be documented, and a stylesheet that provides unique styles to the diagram. Duplicate the sample files from the *pinout* package by launch Python at the location you intend to work and enter the following:
```python
from pinout import resources
resources.duplicate('get started')

# expected output:
# >>> get_started_pinout.py duplicated.
# >>> get_started_board.png duplicated.
# >>> get_started_styles.css duplicated.
```

Once you have these file a finished diagram can be generated by running the python script from a command line `py get_started_pinout.py`. An SVG file is created and can be conveniently view in a browser.

![SVG diagram ](docs/_static/finished_sample_diagram.png)

For a detailed walk through *sample_diagram.py* and more information on *pinout* please visit [pinout.readthedocs.io](https://pinout.readthedocs.io).
