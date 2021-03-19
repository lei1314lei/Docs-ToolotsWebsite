Redis Things
==========================================

Troubleshooting
================
#. Issue caused by compression lib 'lzf'

Problem looks like

.. image:: images/lzf-go-to-die.png

Tracking and positioning

.. image:: images/lzf-go-to-die-backtrace.png

Solved by chang compress lib to be 'gzip'

.. image:: images/lzf-go-to-die-solution.png

