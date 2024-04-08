.. image:: https://img.shields.io/badge/sitcomtn--125-lsst.io-brightgreen.svg
   :target: https://sitcomtn-125.lsst.io
.. image:: https://github.com/lsst-sitcom/sitcomtn-125/workflows/CI/badge.svg
   :target: https://github.com/lsst-sitcom/sitcomtn-125/actions/

################################################################
Neural network classification of AuxTel mount tracking failures.
################################################################

SITCOMTN-125
============

For each image taken by the AuxTel, the tracking performance of the mount is monitored and analyzed.  Typically the RMS tracking errors are small, less that 0.2 arcseconds.  However, there are several problems that can cause the tracking errors to exceed this.  In this work, I built a neural network classifier that classifies the types of tracking failures based on the FFT of the tracking errors.  This was applied to all of the AuxTel data for 2023.  I believe these techniques will be useful for the Simonyi telescope as well.

**Links:**

- Publication URL: https://sitcomtn-125.lsst.io
- Alternative editions: https://sitcomtn-125.lsst.io/v
- GitHub repository: https://github.com/lsst-sitcom/sitcomtn-125
- Build system: https://github.com/lsst-sitcom/sitcomtn-125/actions/


Build this technical note
=========================

You can clone this repository and build the technote locally if your system has Python 3.11 or later:

.. code-block:: bash

   git clone https://github.com/lsst-sitcom/sitcomtn-125
   cd sitcomtn-125
   make init
   make html

Repeat the ``make html`` command to rebuild the technote after making changes.
If you need to delete any intermediate files for a clean build, run ``make clean``.

The built technote is located at ``_build/html/index.html``.

Publishing changes to the web
=============================

This technote is published to https://sitcomtn-125.lsst.io whenever you push changes to the ``main`` branch on GitHub.
When you push changes to a another branch, a preview of the technote is published to https://sitcomtn-125.lsst.io/v.

Editing this technical note
===========================

The main content of this technote is in ``index.rst`` (a reStructuredText file).
Metadata and configuration is in the ``technote.toml`` file.
For guidance on creating content and information about specifying metadata and configuration, see the Documenteer documentation: https://documenteer.lsst.io/technotes.
