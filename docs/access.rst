.. _access:

Access Kolibri
##############


Starting Kolibri on Windows
===========================

To start the **Kolibri** server on Windows, just double-click the desktop shortcut. You will see the notification message *Kolibri is starting, please wait...*.

When you see the notification *Kolibri is running...*, **Kolibri** will open in the browser with the URL http://127.0.0.1:8080.


Kolibri Taskbar Options
***********************

While it is running, **Kolibri** will display an icon in the Windows taskbar (usually at bottom right, near the clock), that allows you to stop it and configure other settings.  

    .. figure:: img/taskbar-options.png
     :alt: When you right click the Kolibri taskbar icon, you can see the taskbar options.

     Kolibri taskbar options.


* Use the **Load in browser** option to open Kolibri in the browser.
* By default **Kolibri** will start running every time you start the computer where it is installed. Uncheck the **Run Kolibri at system startup** option if you prefer to start it manually from the desktop shortcut.
* When installed, **Kolibri** will open in the browser every time it is started. Uncheck the option **Open browser when Kolibri starts** if you prefer to have it running in the background, and to open it manually in the browser by typing the URL http://127.0.0.1:8080 in the address bar.
* Select **Exit** to stop **Kolibri**. You will be prompted to confirm the selection, after which **Kolibri** will stop. You will have to close the browser (or the tab) manually.

.. note::
  Remember to :ref:`configure other computers <access_LAN>` in the network to access **Kolibri** content.


Starting Kolibri on Linux or MacOS
==================================

Starting Kolibri on Linux and MacOS will differ depending on the method you used to install it.

* If you used the **PEX** package, Kolibri will be accessible as long as the process is running in the `Terminal <https://help.ubuntu.com/community/UsingTheTerminal>`_. If you stop the process, close the Terminal window, or restart your system, you will need to :ref:`run the PEX again <pex>` to restart Kolibri. 

* If you installed Kolibri as a system service with the :ref:`DEB installer <lin_deb>`, it will run automatically on each system restart, and you do not need to start it manually. Proceed to step 2 below.

* If you installed Kolibri through the :ref:`PPA <ppa>`, or :ref:`generic installation <pip-installation>` with ``pip install`` command, follow these steps.

  1. Run this command in Terminal to start Kolibri:

    .. code-block:: bash

      kolibri start

    .. warning:: On macOS you may need to prefix the command with ``python``, and type ``python -m kolibri start`` instead.

  2. Open a web browser at ``http://127.0.0.1:8080``, the location of the **Kolibri** start page *from your local device*.

    .. note::
      The special address ``127.0.0.1`` is not accessible from other devices on the network. See: :ref:`accessing Kolibri from other devices in the network <access_LAN>`.

  3. Run this command in Terminal to stop Kolibri:

    .. code-block:: bash

      kolibri stop


.. _access_LAN:

Accessing Kolibri from A Local Network
======================================

If you have installed and started Kolibri on a computer that is connected to a local network (hotspot, cabled ethernet etc.), you can access Kolibri from other devices on the same network. In cases where Kolibri is made accessible on a local network, we call the computer with kolibri a **server** and the other devices on the network, we call **clients**.

The Server's External IP
************************

You need to know the server's external :ref:`IP address <ips>` to access it from other devices in the the same network.

For example, if Kolibri is installed and started on a computer with the IP address **192.168.0.104**, you can access it from an Android tablet connected to the same network by opening the browser on the tablet and typing the address ``http://192.168.0.104:8080``. When running ``kolibri start`` in your Terminal, you will see information about the server's IP address.


.. tip::
  * You can check the IP (**Server URL**) of the device where Kolibri is running by going to **Info** tab in the **Device** dashboard.

    .. figure:: img/device-info.png
      :alt: Open the Device page and navigate to the Info tab to find the IP (Server URL) for your device.

      Find the IP/Server URL in the Device > Info tab.
  
  * You can also use the ``ipconfig`` command on Windows or ``ifconfig`` command on Linux/OSX to find the externally visible IP address of the device running the Kolibri.


.. note::
  * In case of network problems, see :ref:`troubleshooting tips <network>`.
  * Examples and comparison of `Hardware Configurations for Kolibri <https://learningequality.org/r/hardware>`__ (PDF document).
  * Be sure to read about :ref:`system requirements <sys_reqs>` for both the server and the clients.

.. Access Kolibri on Android
.. *************************

.. Go to **Apps** on your device and tap the **Kolibri** icon.

.. figure: img/android-apps.png
..  :alt: Tap the Kolibri icon among your device apps to start.

..  Tap the Kolibri icon among your device apps to start.


.. _change_language:

Change Language
===============

To change language in which the **Kolibri** user interface is displayed, follow these steps:

#. Open your user menu in the upper right corner.
#. Select the **Change language** option.
#. Choose the desired language.
#. Click :guilabel:`CONFIRM` and Kolibri will be displayed in the selected language!

.. warning::
  The default language configured in your browser preferences might override the language configured in Kolibri. To ensure that Kolibri displays in the desired language, make sure to configure it as default in the browsers of all the devices that will be used to view Kolibri content.
