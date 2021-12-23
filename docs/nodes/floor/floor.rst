==========
Floor Node
==========

This node can combine panels into a floor. You can imagine a floor as 1D array
of panels. Read details in :doc:`/data_structure`.

Floor can be infinite of finite. A floor is infinite if it has Fill panels and
its length parameter is equal to 0. In all other cases it's finite.

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
  If it's more than 0 the height of the floor will be defined by this value
  otherwise the height will be determined by the highest panel in the floor.

Length
  If it's more than 0 the length of the floor will be defined by this value.
  This property is useful together with using :doc:`join_floors`.

Scalable
  It is used by :doc:`/nodes/facade/facade`. If true the floor will
  take part in adopting size of facade to actual dimensions.

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

.. figure:: /images/nodes/Floor.*
   :width: 700 px

   Creating floor with flanking pilasters.