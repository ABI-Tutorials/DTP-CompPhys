.. _dtp_cp_modellingbestpractices:

==============================================
Introduction to (ODE) Modelling Best Practices
==============================================

.. contents::

In this part of the computational physiology module we demonstrate some modelling practices that we recommend you follow when developing any mathematical model. The key principles are modularity, reuse, and reproducibility - we demonstrate those here using the tool `OpenCOR <http://opencor.ws>`_ and the `CellML <http://cellml.org>`_ and `SED-ML <http://sed-ml.org>`_  formats, but the principles are valid across the spectrum of computational physiology. It is also important to be able to share and collaborate with other scientists and we demonstrate this using the Physiome Model Repository (PMR).

Here are a couple of links in case you need a refer back to some of the material covered earlier in the module.

* :ref:`cellml_opencor_pmr_tutorial__first_model`
* :ref:`cellml_opencor_pmr_tutorial__open_existing`
* :ref:`cellml_opencor_pmr_tutorial__sedml_web_lab`

Reproducible and reusable model descriptions
============================================

In this section we introduce some of the key concepts and best practices for ensuring your mathematical models are reproducible and reusable.

Units
-----

.. toctree::
   :hidden:
   
   opencor-tutorial/source/cellml_units

The first concept is that everything in your model should have clearly defined physical dimensions (or at least a clear statement that the quantity has no physical dimension). This ensures that when a scientist reuses a model they are able to use software tools to check for dimensional consistency and even potentially automatically convert quantities as required.

1. Take a look through the section :ref:`cellml_opencor_pmr_tutorial__cellml_units` for a discussion and some examples demonstrating the use of units in CellML and OpenCOR.

Modularity
----------

.. toctree::
   :hidden:
   
   opencor-tutorial/source/cellml_comp_and_conn
   opencor-tutorial/source/cellml_encaps_and_inter
   
The second concept is that of modularity. By defining your mathematical model in a modular fashion with clearly defined interfaces you ensure that other scientists (**and even yourself!**) are able to make sure of the modules in future novel work.

2. The section :ref:`ocr_tut_intro_cellml_comp_conn` provides an introduction to the syntax for defining modules in CellML and the mechanism for defining the communication between the modules.

3. :ref:`ocr_tut_intro_cellml_encaps_inter` then introduces the concept of hierarchically grouping modules as an aide to reuse and abstraction, as well as definition of module interfaces.

Reuse
-----

.. toctree::
   :hidden:
   
   opencor-tutorial/source/cellml_imports
   opencor-tutorial/source/cellml_import_unit_params

The final key concept is that of reusing existing modules, defined using the previous concepts.

4. :ref:`ocr_tut_intro_cellml_imports` introduces the mechanism by which existing modules can be reused in CellML models.

When describing your model it is useful to separate the mathematical model from its instaniation with a specific set of parameter values. This allows the model to be reused with different parameter sets for different purposes, including different simulation protocols, etc. Furthermore, rather than continually redefining the same set if units, it is better practice to simply define your units once and reuse their definition as required. Potentially even defining a standard set of units for a research group or collaboration to use and storing that in the repository for everyone to make use of.

5. In :ref:`ocr_tut_intro_cellml_import_unit_params` we demonstrate the separation of model parameters and reuse of a common units definition.

Collaboration, versioning, discovery
====================================

.. toctree::
   :hidden:
   
   opencor-tutorial/source/pmr
   opencor-tutorial/source/pmr_workspaces_in_opencor

One of the main reasons to encode your mathematical models following the principles described in the previous sections is to make the model available for future scientists (again, including yourself!) to utilise the model in novel investigations. The Physiome Model Repository (`PMR <https://models.physiomeproject.org/>`_) has been developed to provide scientists with a suitable repository for sharing their work with the community. Full details are provided in the `PMR documentation <https://models.physiomeproject.org/docs>`_, but here we highlight some PMR capabilities.

6. We have :ref:`previously introduced <cellml_opencor_pmr_tutorial__open_existing>` the various ways to load models from PMR into OpenCOR. In :ref:`cellml_opencor_pmr_tutorial__pmr_intro` we illustrate some of the extra information that is avaialble via the PMR web interface.

7. Choosing your favourite area of physiology, see if you can discover an interesting model in PMR and load it into OpenCOR to explore. Do you find this a more comprehensive way to understand the model than only reading the source literature?

The primary unit of information in PMR is the workspace. Each workspace is a version controlled repository which is permanently and persistently available, with each resource in the workspace assigned a unique identifier for each version of the resource submitted to the repository.

8. In :ref:`cellml_opencor_pmr_tutorial__pmr_with_opencor` we present OpenCOR's capabilties for directly working with workspaces in PMR.

9. Compare the method described in step 8 with the `previous method scientists had to follow <http://aucklandphysiomerepository.readthedocs.io/en/latest/cellmlrepositorytutorial.html>`_ in order to get models into PMR. Do you see why most scientists would prefer to email their models to Andre and let him add them to the repository?

**Extra for experts:**  if you look through the `PMR documentation <https://models.physiomeproject.org/docs>`_ you will be able to find information on how to submit your workspaces to make them public, share them directly with collaborators, and make *exposures* for specific revisions of the workspace.


OpenCOR tutorial
================

For reference, the complete tutorial on CellML, OpenCOR, and PMR (from which the material presented above is reused) is given here. It is not directly part of the DTP computational physiology module, but does provide some useful information and we still need to better extract the bits we need.


.. toctree::
   :maxdepth: 2
   
   opencor-tutorial/source/index
   
   