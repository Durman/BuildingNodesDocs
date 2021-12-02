==============
Facade Pattern
==============

This node can combine floors into a facade style. You can imagine floors as rows
in 2D array. So this node takes different rows and combine them together.
Read details in :doc:`/data_structure`.

Inputs
------

Last
  Last floor

Fill
  Floor which should be used to cover facade between first and last floors if
  they were given

First
  Fist floor

Properties
----------

Size
  This parameter is used by :doc:`join_facades`. It shows a size which this
  facade can obtain from total size of main facade.

Remote floor properties
-----------------------

Scalable
  If true the floor will be scale along Z axis together with other scalable
  floors to fit total height of floors into facade height. If all floors are
  not scalable the facade may have gap in the top.

Examples
--------
