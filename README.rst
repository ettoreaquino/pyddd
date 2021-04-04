Python DDD
==============

`pyddd` is a template, which aims to prive basic scaffolding for creating domain
driven back-ends with Poetry, Falcon and Docker.

It is very important to mention that DDD is not always necessary. But when it comes
to creating a well structured back-end, Domain Driven Design is the way to go and
glueing the basic components of a Python project can be very tedious, specially
considering tests and databases.

Basic Components
-----------------
A set of frameworks and tools are used to make easier the tedious tasks involved
in testing, packaging, and exposing endpoints.

Poetry_
^^^^^^^^^^^^^^^^^
Poetry is a very powerfull library for packaging and dependency management.

Falcon_
^^^^^^^^^^^^^^^^^
Falcon is a very light and minimalist web API framework for building backends.
The idea of it being very concise and simple, brings our structure closer to the
concept of being as objective as possible.

Docker_
^^^^^^^^^^^^^^^^^
Docker allow us to containerize our app from the beginning, helping decouple
infrastructure and make integration tests easier.

Running
-----------------
Clone this repository and install its basic dependencies:

.. code-block::

    poetry install

Run the project using docker to make sure everything is in place and configured:

.. code-block::

    make all

This command calls the Makefile command, which in turn encapsulates a sequence of
commands that will end up running the tests and stopping the container.


.. _Poetry: https://python-poetry.org/
.. _Falcon: https://falconframework.org/
.. _Docker: https://docs.docker.com/