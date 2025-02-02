Repository Enhancement
======================

The original repository for the OPi.GPIO library, available at https://github.com/rm-hull/OPi.GPIO, has been enhanced to support additional boards: Orange Pi 3B and Orange Pi Zero 3.

Key Modifications:
------------------

- **Added Support for Orange Pi 3B**
- **Added Support for Orange Pi Zero 3**

Installation
------------

To install the enhanced version of OPi.GPIO, use the following pip command:

.. code-block:: bash

    pip3 install terindo.gpio==1.0.1

Usage
-----

After installation, OPi.GPIO can be utilized in your Python code as shown below:

.. code-block:: python

    import OPi.GPIO as GPIO
    # import orangepi.zero3
    import orangepi.pi3b

    # GPIO.setmode(orangepi.zero3.BOARD)
    GPIO.setmode(orangepi.pi3b.BOARD)





OPi.GPIO
========

.. image:: https://travis-ci.org/rm-hull/OPi.GPIO.svg?branch=master
   :target: https://travis-ci.org/rm-hull/OPi.GPIO

.. image:: https://coveralls.io/repos/github/rm-hull/OPi.GPIO/badge.svg?branch=master
   :target: https://coveralls.io/github/rm-hull/OPi.GPIO?branch=master

.. image:: https://readthedocs.org/projects/opi-gpio/badge/?version=latest
   :target: http://opi-gpio.readthedocs.io/en/latest/?badge=latest

.. image:: https://img.shields.io/pypi/pyversions/OPi.GPIO.svg
   :target: https://pypi.python.org/pypi/OPi.GPIO

.. image:: https://img.shields.io/pypi/v/OPi.GPIO.svg
   :target: https://pypi.python.org/pypi/OPi.GPIO
   
.. image:: https://img.shields.io/maintenance/yes/2021.svg?maxAge=2592000

A drop-in replacement library for `RPi.GPIO <https://sourceforge.net/projects/raspberry-gpio-python/>`_
for the Orange Pi Zero and other SBCs. Only the basic GPIO functions are replicated,
using sysfs: this allows the GPIO pins to be accessed from user space.

See the `documentation <https://opi-gpio.readthedocs.io>`_ for install
instructions and detailed API usage.

References
----------
* https://www.kernel.org/doc/Documentation/gpio/sysfs.txt
* http://linux-sunxi.org/GPIO
* https://forum.armbian.com/index.php?/topic/1471-solved-difficulty-accessing-gpio-via-the-sunxi-gpio-export-interface/
* https://forum.armbian.com/index.php?/topic/3655-guide-orange-pi-zero-gpios/
* https://jsfiddle.net/tuav7f6q/2/
* https://www.mysensors.org/build/orange
* https://kaspars.net/blog/linux/orange-pi-zero-gpio
* https://developer.toradex.com/knowledge-base/pwm-linux

License
-------
The MIT License

Copyright (c) 2018 Richard Hull

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
