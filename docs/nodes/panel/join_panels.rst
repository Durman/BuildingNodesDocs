================
Join Panels Node
================

This node get several panels as input and bake them into a single panel.
When one panel is joined to another it sticks to one side of the previous panel.
Process of joining can go from left to right and bottom to top or vice versa.

Inputs
------

Panel
  Repeatable socket for input panels

Properties
----------

Align
  This property determines the side where to put next panel (right, left, top or
  bottom).

Outputs
-------

Panel
  Resulting panel

Examples
--------

.. figure:: /images/nodes/Join_panels.*
   :width: 700 px

   This setup join windows and pillars in a way that central pillars are always
   lesser than number of windows on one item. In yellow border there are two
   panels which are joined by first Join node and in the red border there are
   two panels which are joined by second Join node.
