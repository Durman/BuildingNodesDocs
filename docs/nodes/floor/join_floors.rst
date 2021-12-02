================
Join Floors Node
================

This node can join floors along horizontal axis. It's possible to classify
to different kinds of floors - infinite and finite. The node tries to get
finite floors first and if after that there is free space it uses infinite
floors to full all the rest space. If it joins more then one infinite floor
the spaces is divided between them according to their `join size` value.

Inputs
------

Floor
  Repeatable socket which expects floors to join

Remote floor properties
-----------------------

Join size
  It is used only if there is two or more infinite floors, with Fill panel,
  to join. In this case size of the infinite floors is determined proportionally
  to their join size.

Outputs
-------

Floor
  Resulting floor

Examples
--------
