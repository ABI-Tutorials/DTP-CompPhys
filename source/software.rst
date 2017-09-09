.. _dtp_cp_software:

Software Tools
==============

Here we introduce the tools used in this module and provide instructions for getting them set up to perform the tasks in this module.

.. contents::

MAP Client
----------

The Musculoskeletal Atlas Project Client (MAP Client) is an open-source cross-platform framework for managing workflows.  A workflow, as far as MAP Client is concerned, consists of a number of connected workflow steps.  The MAP Client framework is a plugin-based application where the plugins are workflow steps.  MAP Client is a Python based application which makes use of the Qt widget library.

Documentation for the project can be found at `MAP Client documentation <https://map-client.readthedocs.io/en/latest/>`_.

MAP Client is available to download from `MAP Client download <https://github.com/MusculoskeletalAtlasProject/mapclient/releases>`_

To get the best out of the MAP Client you will need to get some plugins, by default the MAP Client comes with five basic plugins.  A collection of available plugins can be found at `MAP Client plugins <https://github.com/mapclient-plugins>`_.

OpenCOR
-------

Instructions for obtaining and using `OpenCOR <http://opencor.ws/>`_ are covered in the :ref:`cellml_opencor_pmr_tutorial__installation`. If you are using one of the DTP laptops, then the correct version of OpenCOR will already be installed, but for the purposes of this module you need to install the *12 August 2017 snapshot*, or newer, verison of OpenCOR.

Getting to know OpenCOR
+++++++++++++++++++++++

OpenCOR is a very flexible model management, editing, and simulation tool with many features. The full :ref:`cellml_opencor_pmr_tutorial_index` tutorial covers a lot of material that is relevant to this tutorial, but before continuing here it is useful to quickly run through the section :ref:`cellml_opencor_pmr_tutorial__first_model` to get a bit of familiarity with the tool.

.. _preparation-pmrAccount:

Connecting OpenCOR to your PMR account
++++++++++++++++++++++++++++++++++++++

Once you have OpenCOR installed, we want to connect it to PMR to enable you to archive and share your work. If you follow the instructions over at :ref:`cellml_opencor_pmr_tutorial__pmr_with_opencor` to create an account on the teaching instance of the Physiome Model Repository (PMR) and then set up OpenCOR to use that account. You can use this `CellML model <https://models.physiomeproject.org/workspace/25d/rawfile/c702d05c6a698b7b97dbb5b106600a16abfbff97/lorenz.cellml>`_ as the test model for that part of the tutorial.

.. include:: PMR2/teaching-instance-warning.rst




.. toctree::
   :hidden:
   
   opencor-tutorial/source/install
