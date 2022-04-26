# Volume-Visualization

<img width="1611" alt="50TimePoint_Ana3_every10_white" src="https://user-images.githubusercontent.com/54334152/165230472-bd681439-3b03-4546-944c-b111dc9d4696.png">

Tools for visualizing medical volumetric data are currently lacking despite increased use cases for generating in silico medical datasets using scientific computational modeling tools. This page provides an automated workflow for the rendering of 3D volumetric medical datasets using the software Houdini. We are providing all files to freely render a 3D animation of volumetric datasets using a free version of Houdini. Also included in this repository are files for an optional (alternative?) method of rendering using Redshift renderer, which requires paid licenses for both Houdini and Redshift.

## Overview
This repository includes:
* A sample dataset of 51 image stacks, including 1 image stack of a portion of an in silico breast model generated using a procedural analytic model (from the VICTRE pipeline: https://github.com/DIDSR/VICTRE) and 50 time points of a growing tumor within that anatomy (from: "Computational model of tumor growth for in silico trials." Aunnasha Sengupta, Diksha Sharma, and Aldo Badano.  Medical Imaging 2021: Physics of Medical Imaging. Vol. 11595. International Society for Optics and Photonics, 2021.)
* A Houdini hipnc file (.hipnc) which includes the virtual environment and automated python script to render an animation using Houdini's native renderer, Mantra (free)
* An optional Houdini hiplc file (.hiplc) while includes the virtual environment and automated python script to render the same animation using third-party renderer, Redshift (requires paid license)
* A video tutorial with instructions for running the automated python script within the Houdini interface
* Example animation videos output from the automated pipeline


## Requirements
**Free version (Houdini Apprentice + Mantra Renderer)**
* To open the Houdini hipnc file (.hipnc), you must have installed the free version of Houdini which comes with the native renderer Mantra:
  * Install Houdini Apprentice version 19.0 or newer from https://www.sidefx.com/buy/#houdini-free (free license)
  * Note: Mantra is a CPU-based renderer.

**Redshift version (Houdini Indie + Redshift Renderer)**
* To open the **optional** Houdini hiplc file (.hiplc), you must have installed a paid license for Houdini, as well as a paid license for Redshift:
  * Install Houdini Indie version 19.0 or newer from https://www.sidefx.com/buy/#houdini-indie (paid license)
  * Install Redshift version 3.0.66 or newer from https://www.maxon.net/en/buy (paid license)
  * Refer to the Redshift documentation on how to configure the Redshift plugin for Houdini https://docs.redshift3d.com/display/RSDOCS/Houdini+Plugin+Configuration?product=houdini#HoudiniPluginConfiguration-Pluginreleasedversions
  * Note: Redshift is a GPU-accelerated renderer with the following minimum GPU requirements: https://www.maxon.net/en/requirements/redshift-requirements


## How to Use
1. Install Houdini Apprentice (free)
2. Download the Houdini hipnc file (.hipnc) from this repository
3. Download the sample dataset from this repository, or use your own image stack (see https://www.sidefx.com/docs/houdini/io/formats/image_formats.html for image file formats supported by Houdini)
4. Run the Houdini hipnc file (.hipnc) and follow instructions from the video tutorial

