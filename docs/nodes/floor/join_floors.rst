================
Join Floors Node
================

This node can join floors along horizontal or vertical axis. If join axis is
horizontal it can join only :doc:`finite floors <floor>` otherwise the first
input floor will be outputted.

Inputs
------

Floor
  Repeatable socket which expects floors to join

Properties
-----------------------

Direction
  It determines in which direction given floors should be joined to each other.

  Vertical
    In this mode floors will be put on top of each other.
  Horizontal
    In this mode floors will be put along length of initial facade.

Match mode
  It determines how to handle the case when floors are shooter than
  base facade length.

  None
    In this case the floor will remain with a gap which the style was unable
    to cover.
  Repeat
    In this case if facade has longer size than floor
    can cover the remain space will be covered with last floor.
  Cycle
    In this mode all given floors will be repeated if their size is 
    shooter than size of base facade. For example ``A B C`` floor styles are
    given. They can be stack with each other in next way ``A B C A B C A`` and
    so on.

Outputs
-------

Floor
  Resulting floor

Examples
--------

.. figure:: /images/nodes/Join_floors.*
   :width: 700 px

   Join floors with length 4 along horizontal axis.

.. figure:: /images/nodes/Join_floors2.*
   :width: 700 px

   Add ledge on the top of each floor.