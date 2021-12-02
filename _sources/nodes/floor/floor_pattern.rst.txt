==================
Floor Pattern Node
==================

This node can combine panels into a floor. You can imagine a floor as 1D array
of panels. Read details in :doc:`/data_structure`.

Inputs
------

Left
  Panel to be put to the left most side.

Fill
  Panel which should be used to cover all available space of the floor.

Right
  Panel to be put to the right most side.

Properties
----------

Height
  If enabled the height of the floor will be defined by this value otherwise
  the height will be determined by the highest panel in the floor.

Scalable
  It is used by :doc:`/nodes/facade/facade_pattern`. If true the floor will
  take part in adopting size of facade to actual dimensions.

Join size
  It is used by :doc:`/nodes/facade/join_facades`. It determines the width of
  the floor in total size of the facade.

Remote panel properties
-----------------------

Scalable
  This properties is used to define which panels can be scaled to adjust width
  of the floor so it would be equal to width of the facade.

Outputs
-------

Floor
  Resulting floor

Examples
--------
