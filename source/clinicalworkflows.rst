.. _dtp_cp_clinicalworkflows:

Clinical Workflows
==================

In :numref:`fig_dtp_cp_exampleworkflow` you can see an example of a clinical workflow that adopts a computational physiology approach. In summary: 

#. Clinical observations are made (in this example, images from a mamographic scan).
#. A model is customised to those observations (a geometric model specific to the given patient).
#. Simulations are performed as part of the investigation (simulating mamographic compression on the geometrical model to determine the affect on internal structures).
#. Some kind of visualisation is performed to help interpret the simulation results in regard to the clinical observations (registering mamographic and MRI images to highlight potential calcifications in the breast tissue).
#. The preceeding steps are wrapped into a customised user interface which can be provided to the clinicians for them to execute these steps in the clinic.

.. _fig_dtp_cp_exampleworkflow:

.. figure:: /_static/example-workflow.png
   :align: center
   :figwidth: 90%
   :width: 90%
   :alt: An example clinical workflow.
   
   An example of a clinical workflow, showing the steps in the process which form the basis for the Computational Physiology module.
   
The goal of these tutorials is to make you aware of the key skills required at each step in the process described above and in :numref:`fig_dtp_cp_exampleworkflow`. We achieve this here by leading you through some examples of the various skills and demonstrate their applicability across a range of organ systems and spatial scales.

.. toctree::
   :maxdepth: 2
   :caption: Contents:
   
   segmentation/source/index
   modelconstruction/source/index
   simulation/source/index
   visualisation/source/index
   completeworkflow/source/index