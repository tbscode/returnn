.. _installation:

============
Installation
============

Installation is easy.
Checkout the Git repository of RETURNN (https://github.com/rwth-i6/returnn/).
Install all dependencies, which are just numpy, h5py (:code:`pip install -r requirements.txt`),
and the backend you want to use (TensorFlow or Theano).

For TensorFlow, use :code:`pip install tensorflow-gpu` if you have a Nvidia GPU,
and make sure that CUDA and cuDNN can be found.

For Theano, only version 0.9 works (:code:`pip install theano==0.9`).
For Theano usage, make sure that you have this in your ``~/.theanorc``::

    [global]
    device = cpu
    floatX = float32

For some specific datasets or special layers, additional dependencies might be needed,
such as ``librosa``.
For running the tests, you need ``nose``.

See :ref:`basic_usage` for the basic usage of RETURNN.
