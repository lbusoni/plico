# PLICO: Python Laboratory Instrumentation COntrol

| [![Build Status][travis]][travislink] | [![Coverage Status][coveralls]][coverallslink] | 


plico is a framework to develop applications controlling instrumentation typically available in a scientific laboratory.
It is entirely written in Python and support server-client applications, using [zeromq][zmq] as message dispatcher.


[zmq]: http://zeromq.org
[travis]: https://travis-ci.com/lbusoni/plico.svg?branch=master "go to travis"
[travislink]: https://travis-ci.com/lbusoni/plico
[coveralls]: https://coveralls.io/repos/github/lbusoni/plico/badge.svg?branch=master "go to coveralls"
[coverallslink]: https://coveralls.io/github/lbusoni/plico


## Installation

plico runs on Python 2.7+ and Python 3.3+. 

It depends on zmq, numpy and pyfits (to store calibrations). You need a backend (PyQt4/PySide, PyQt5/PySide2) for GUIs.

It is not very useful to install this package by itself. See [tipico][tipico] to install an example applications simulating some HW controller and a corresponding client. 

Anyhow, if you really want to install plico as standalone package go on with pip:

```
pip install plico
```

## Wish list

   + Documentation (readthedocs or alike)
   + Implement reconnect-to-devices in case of lost connection
   + Implement service discovery 


[tipico]: https://github.com/lbusoni/tipico
