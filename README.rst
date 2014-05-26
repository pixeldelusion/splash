=======================================
Splash - A javascript rendering service
=======================================

Splash is a javascript rendering service with an HTTP API. It's a lightweight
browser with an HTTP API, implemented in Python using Twisted and QT.

It's fast, lightweight and state-less which makes it easy to distribute.

Documentation
-------------

Documentation is available here:
http://splash.readthedocs.org/

Ubuntu 12.04+ LTS is the best server install system for this software.

Additional notes for install
=============================
To build the server for the install pip package::
``sudo apt-get install xvfb x11-xkb-utils xfonts-100dpi xfonts-75dpi xfonts-scalable xfonts-cyrillic xserver-xorg-core build-essential python-dev python-pip python-qt4``
add the essential tools required for the software to run.

The original developer of the software does not run it as headless system - I personally like it to run as this method.
To run it as Xvfb or X virtual framebuffer has it advantages for running background process.

Commands to run as background process::
	``nohup xvfb-run python -m splash.server 1>&2 &>/tmp/splash.log&``
	
Support
-------

Open source support is provided here in Github. Please `create a question
issue`_ (ie. issue with "question" label).

Commercial support is also available by `Scrapinghub`_.

.. _create a question issue: https://github.com/scrapinghub/splash/issues/new?labels=question
.. _Scrapinghub: http://scrapinghub.com
