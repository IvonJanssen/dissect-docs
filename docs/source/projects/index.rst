Projects
========

Installing individual projects
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Dissect is a collection of libraries and tools, so every Dissect project is individually installable. You'll find that
installing the ``dissect`` package from PyPI will install all available ``dissect.*`` packages for you! If, however,
you just want to work with the NTFS and registry parsers in your own scripts, you can opt to only install or depend
on those specific projects:

.. code-block:: console

    $ pip install dissect.ntfs dissect.regf

.. toctree::
    :maxdepth: 1
    :glob:

    /projects/*/index
