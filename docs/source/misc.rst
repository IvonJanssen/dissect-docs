Other tools
-----------

Besides the most prominent tools like **target-query**, **acquire**, **target-shell** and **rdump**,
Dissect ships with a lot of additional utilities that might be of help:


target-dd
~~~~~~~~~

With ``target-dd`` you can export (a part of) a target to a file or to ``stdout``. At the moment, ``target-dd``
can be used for targets that have only one disk.

.. note::

    For a complete overview of all options see :doc:`here <tools/target-dd>`.


target-dump
~~~~~~~~~~~

With ``target-dump`` you can export records of a specific ``function`` used in target-query to a file.

.. note::

    For a complete overview of all options see :doc:`here <tools/target-dump>`.


target-fs
~~~~~~~~~

With ``target-fs`` you can interact with the filesystem of a target, using a set of familiar Unix commands.

.. note::

    For a complete overview of all options see :doc:`here <tools/target-fs>`.

target-info
~~~~~~~~~~~

The ``target-info`` tool gives a brief summary of a target.

.. note::

    For a complete overview of all options see :doc:`here <tools/target-info>`.



target-reg
~~~~~~~~~~

``target-reg`` is a tool to easily query the registry of Windows targets and prints it in a tree.

.. note::

    For a complete overview of all options see :doc:`here <tools/target-reg>`.


target-mount
~~~~~~~~~~~~

With ``target-mount`` you can mount the filesystem of a target to an arbitrary directory on your analysis machine,
similar to the ``mount`` command on Unix systems.

.. note::

    For a complete overview of all options see :doc:`here <tools/target-mount>`.
