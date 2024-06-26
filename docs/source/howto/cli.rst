.. _topics:cli:

**********************
Command line interface
**********************
As a supplement command for `verdi`, the command line interface utility for AiiDA-WorkGraph is called ``workgraph``.
This section explains the basic concepts that apply to all ``workgraph`` commands.

.. _topics:cli:parameters:

Parameters
==========
Parameters to ``workgraph`` commands come in two flavors:

* Arguments: positional parameters, e.g. ``123`` in ``workgraph graph show 123``
* Options: announced by a flag (e.g. ``-f`` or ``--flag``), potentially followed by a value. E.g. ``workgraph graph list --limit 10`` or ``workgraph graph -h``.


.. _topics:cli:help_strings:

Help strings
============
Append the ``--help`` option to any verdi (sub-)command to get help on how to use it.
For example, ``workgraph graph kill --help`` shows::

    Usage: workgraph graph kill [OPTIONS] [PROCESSES]...

        Kill running processes.

    Options:
        -t, --timeout FLOAT  Time in seconds to wait for a response before timing
                             out.  [default: 5.0]
        --wait / --no-wait   Wait for the action to be completed otherwise return as
                             soon as it's scheduled.
        -h, --help           Show this message and exit.
