.. _osx:

Other Linux & MacOS
===================

Compatibility
-------------

* MacOS: 10.6+, all browsers supported
* Linux: Any system with Python 2.7, all browsers supported

.. _pex:

Install
-------

To install Kolibri on Linux distributions other than Debian, as well as on MacOS, you can use :ref:`generic installation <pip-installation>` with ``pip install`` command, or follow these steps to run Kolibri with the ``PEX`` package. 

#. Download the `Kolibri PEX installer <https://learningequality.org/r/kolibri-pex-latest>`_.
#. Make sure to **open the Terminal where you downloaded** the ``PEX`` file. For example, if you saved it in the *Downloads* folder, type this when you open the Terminal, and press Enter:

	.. code-block:: bash

	  cd Downloads

#. Type the following commands next (press Enter after each one). 


	.. code-block:: bash

	  chmod +x kolibri-installer-filename.pex
	  ./kolibri-installer-filename.pex start

	.. warning:: Make sure to **substitute the** ``kolibri-installer-filename.pex`` **with the exact name of the file you downloaded** in both commands. For example, if the name of the downloaded file is ``kolibri-v0.10.0.pex``, type that instead of ``kolibri-installer-filename.pex``. 

#. When the command finishes, open the default browser at http://127.0.0.1:8080 and proceed with the :ref:`setup_initial` of your facility. 


Uninstall
---------

#. Delete the ``PEX`` file.
#. Delete the ``./kolibri`` folder in your user's Home directory if you want to completely remove all the Kolibri files and content channels you imported.

Upgrade
-------

To upgrade Kolibri, follow these steps.

#. Download the new version of `Kolibri PEX installer <https://learningequality.org/r/kolibri-pex-latest>`_.
#. Start Kolibri as during the first install.
#. Go explore the new and improved Kolibri features!