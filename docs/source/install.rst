Install
-------

Installing Dissect is easy. The preferred way of installing Dissect is with `pip`.
The install procedure is described below.

System requirements
~~~~~~~~~~~~~~~~~~~

These are recommended system requirements.
Dissect may still work on older systems but we do not actively
test on those.

* Operating system versions: Linux 4+, macOS 11+, Windows 8+
* **Python 3.9 - 3.11**
* Processor: 64-bit 1 gigahertz (GHz) or faster with two or more cores
* At least 16 GB of RAM


Install Procedure
~~~~~~~~~~~~~~~~~

Before you install Dissect it is recommended to create a `virtual environment <https://docs.python.org/3/tutorial/venv.html>`_.

.. code-block:: console

    $ pip install dissect

That's all, you're now ready to use Dissect. To get you started, grab a test forensic image `here <https://cfreds.nist.gov/>`_.
!


Using the Docker image
~~~~~~~~~~~~~~~~~~~~~~

If you simply want to get started with some of the examples without having to install anything, a basic Docker image
is available `here <https://github.com/orgs/fox-it/packages/container/package/dissect>`_ (`mirror <https://hub.docker.com/r/dissect/dissect>`_).
You can start using this image by executing the following command in your terminal:

.. code-block:: console

    $ docker run -it --rm -v /path/to/targets/:/mnt:ro ghcr.io/fox-it/dissect:3.2
    (<dissect version>) <container hash>:/workspace$

This will drop you in a shell environment with all the Dissect ``target-*`` :doc:`tools </tools/index>` at your disposal.
The purpose of the ``-v`` option is to mount a local directory inside the Docker container. You can use this to interact
with local data from within the Docker container.

Browser demo
~~~~~~~~~~~~

If you don't feel like doing the above, then there is an interactive browser demo available at
`try.dissect.tools <https://try.dissect.tools>`_ to play around with!

You can select evidence files from your local system, such as VMDK or EWF files, and explore some of the capabilities
of Dissect. Nothing gets uploaded to a server, it all happens locally thanks to `Pyodide <https://pyodide.org/en/stable/>`_!

.. caution::

    The browser demo was developed as a quick demo and is bound to be unstable. Not everything may work as expected.

