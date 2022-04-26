# Volume-Visualization

Tools for visualizing medical volumetric data are currently lacking despite increased use cases for generating in silico medical datasets using scientific computational modeling tools. This page provides an automated workflow for the rendering of 3D volumetric medical datasets using the software Houdini. We are providing all files to freely render a 3D animation of volumetric datasets using a free version of Houdini. Also included in this repository are files for an optional (alternative?) method of rendering using Redshift renderer, which requires paid licenses for both Houdini and Redshift.

This repository includes:
* a sample dataset of 51 image stacks, including 1 image stack of a portion of an in silico breast model generated using a procedural analytic model (from the VICTRE pipeline: https://github.com/DIDSR/VICTRE) and 50 time points of a growing tumor within that anatomy (from: "Computational model of tumor growth for in silico trials." Aunnasha Sengupta, Diksha Sharma, and Aldo Badano.  Medical Imaging 2021: Physics of Medical Imaging. Vol. 11595. International Society for Optics and Photonics, 2021.)
* a Houdini hipnc file (.hipnc) which includes the virtual environment and automated python script to render an animation using Houdini's native renderer, Mantra (free)
* an optional Houdini hiplc file (.hiplc) while includes the virtual environment and automated python script to render the same animation using third-party renderer, Redshift (requires paid license)
* a video tutorial with instructions for running the automated python script within the Houdini interface
* example files of animation videos output from the automated pipeline


### Requirements:
* Free version (Houdini Apprentice + Mantra Renderer)
  * To open the Houdini hipnc file (.hipnc), you must have installed the free version of Houdini which comes with the native renderer Mantra:
    * https://www.sidefx.com/buy/#houdini-free (free license for Apprentice version)
    * Note: Mantra is a CPU-based renderer.

* Redshift version (Houdini Indie + Redshift Renderer)
  * To open the optional Houdini hiplc file (.hiplc), you must have installed a paid license for Houdini, as well as a paid license for Redshift:
    * https://www.sidefx.com/buy/#houdini-indie (paid license for Indie version)
    * https://www.maxon.net/en/buy (paid license for Redshift)
    * Note: Redshift is a GPU-accelerated renderer with the following minimum GPU requirements: https://www.maxon.net/en/requirements/redshift-requirements
