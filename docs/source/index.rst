Welcome to Dissect!
===================

Effortlessly investigate **forensic artefacts** from any source with **Dissect**.
With Dissect, you can go from intake call to patient zero in a matter of hours,
even in infrastructures with thousands of systems.


Quick Demo
----------

In just a couple of seconds you can query a forensic image or even **shell-in**!
This short animation shows how to list deleted files from an suspicious machine
and explore the contents of the machine through a shell...

.. image:: /images/demo.gif


Usage Example
-------------

One of the most prominent tools that Dissect offers is called **target-query**.
With this simple one-liner you can extract all user accounts from an image: 

.. code-block:: console

    $ target-query pc.img -f users
    
    <windows/user ... name='systemprofile' ...>
    <windows/user ... name='LocalService' ...>
    <windows/user ... name='NetworkService' ...>
    <windows/user ... name='Mr. Evil' ...>


Key features
------------

Dissect is a powerful artefact extractor and parser that saves you a lot of time.
With Dissect you can:

* Quickly **extract** artefacts from any source (like EWF, Kape, DD, VDI, PVM)
* Access artefacts from almost any **OS** (like Windows, macOS, Linux/Unix, ESXi)
* Access almost any **filesystem** (like NTFS, EXT, XFS, QNX6)
* **Parse** (binary) logs, registry entries, cookies, history and more
* **Export** findings to Text, JSON, CSV or stream to datastores like Splunk, Elastic, MySQL
* **Feed, filter and script** to process found records in any way you like
* Investigate images with powerful tools like **target-shell**, **target-mount** or the **Python API**

Easy to setup
-------------

No matter your skill level, we have an easy setup solution for you!

* Just install with `pip install dissect` from `PyPI <https://pypi.python.org/pypi/dissect>`_
* Try in the browser `try.dissect.tools <https://try.dissect.tools>`_
* Use the Docker image `here <https://github.com/orgs/fox-it/packages/container/package/dissect>`_ (`mirror <https://hub.docker.com/r/dissect/dissect>`_).


About this manual
-----------------

This manual uses a head first approach. As you have seen we immediately showed some examples of
how you can leverage the power of Dissect. From here on, the documentation will become more
fine-grained at every level. To this end, the manual consists of 

* :doc:`Basics <target-query>`: here we review the basic features of Dissect tools to get started quickly
* :doc:`Reference Guide <tools/target-query>`: these are complete descriptions of every tool in the box
* :doc:`Sub-projects <projects/dissect.target/index>`: descriptions per repository that makes up  
* :doc:`API <api/dissect/target/index>`: this is the most detailed level of explanation

Furthermore, under the advanced section we also discuss:

* Architecture: overall architectural decisions
* Scenarios: more complex (and realistic) real-world usage scenarios

.. toctree::
    :hidden:
    :caption: Introduction
    
    Welcome <self>
    Install </install>
    Tutorial </tutorial>

.. toctree::
    :hidden:
    :caption: Basics
    
    target-query </target-query>
    target-shell </target-shell>
    acquire </acquire>
    rdump </rdump>
    other tools </misc>

.. toctree::
    :hidden:
    :caption: Advanced

    Architecture </overview/index>
    Subprojects </projects/index>
    Scenarios </usage/index>
    Reference Guide </tools/index>
    API /advanced/index

.. toctree::
    :hidden:
    :caption: Project

    /contributing/developing
    /contributing/style-guide
    /contributing/tooling
    License </license>
    /resources/dissect-in-action
    /resources/talks-and-conferences
    GitHub <https://github.com/fox-it/dissect/>
    Try in your browser <https://try.dissect.tools/>
    PyPI <https://pypi.org/project/dissect/>

