
Examples
========

* :ref:`example_plan_catalog`
* :ref:`example_specfile`
* :ref:`example_nscan`
* :ref:`example_tuneaxis`
* :ref:`example_source`
* :ref:`examples_downloads`


.. _example_plan_catalog:

Example: ``plan_catalog()``
+++++++++++++++++++++++++++

The *apstools* package provides an executable that can be 
used to display a summary of all the scans in the database.  
The executable wraps the demo function: :func:`plan_catalog()`.
It is for demonstration purposes only (since it does not filter
the output to any specific subset of scans).

The output is a table, formatted as restructured text, with these columns:

:date/time:

   The date and time the scan was started.

:short_uid:

   The first characters of the scan's UUID (unique identifier).

:id:

   The scan number.  
   (User has control of this and could reset the counter for the next scan.)

:plan:

   Name of the plan that initiated this scan.

:args:

   Arguments to the plan that initiated this scan.


This is run as a linux console command::

   apstools_plan_catalog | tee out.txt

The :download:`full output <resources/plan_catalog.txt>`
is almost a thousand lines.  Here are the first few lines:

.. literalinclude:: resources/plan_catalog.txt
   :language: console
   :linenos:
   :lines: 1-10

.. _example_specfile:

Example: ``specfile_example()``
+++++++++++++++++++++++++++++++

We'll use a Jupyter notebook to demonstrate the ``specfile_example()`` that writes one or more scans to a SPEC data file.
Follow here: https://github.com/BCDA-APS/apstools/blob/master/docs/source/resources/demo_specfile_example.ipynb


.. _example_specfile_databroker:

Example: Create a SPEC file from databroker
+++++++++++++++++++++++++++++++++++++++++++

We'll use a Jupyter notebook to demonstrate the how to get a scan from the databroker and write it to a spec data file.
Follow here: https://github.com/BCDA-APS/apstools/blob/master/docs/source/resources/demo_specfile_databroker.ipynb


.. _example_nscan:

Example: ``nscan()``
++++++++++++++++++++

We'll use a Jupyter notebook to demonstrate the ``nscan()`` plan.  An *nscan* is used to scan two or more axes together,
such as a :math:`\theta`-:math:`2\theta` diffractometer scan.
Follow here: https://github.com/BCDA-APS/apstools/blob/master/docs/source/resources/demo_nscan.ipynb

.. _example_tuneaxis:

Example: ``TuneAxis()``
+++++++++++++++++++++++

We'll use a Jupyter notebook to demonstrate the ``TuneAxis()`` support that provides custom alignment
of a signal against an axis.
Follow here: https://github.com/BCDA-APS/apstools/blob/master/docs/source/resources/demo_tuneaxis.ipynb


.. _example_source:

Source Code Documentation
+++++++++++++++++++++++++

.. automodule:: apstools.examples
    :members:

.. _examples_downloads:

Downloads
+++++++++

The jupyter notebook and files related to this section may be downloaded from the following table.

* :download:`plan_catalog.txt <resources/plan_catalog.txt>`
* jupyter notebook: :download:`demo_nscan <resources/demo_nscan.ipynb>`
* jupyter notebook: :download:`demo_tuneaxis <resources/demo_tuneaxis.ipynb>`
* jupyter notebook: :download:`demo_specfile_example <resources/demo_specfile_example.ipynb>`

  * :download:`spec1.dat <resources/spec1.dat>`
  * :download:`spec2.dat <resources/spec2.dat>`
  * :download:`spec3.dat <resources/spec3.dat>`
  * :download:`spec_tunes.dat <resources/spec_tunes.dat>`
  * :download:`test_specdata.txt <resources/test_specdata.txt>`
