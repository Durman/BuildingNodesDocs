================
Join Floors Node
================

This node can join floors along horizontal axis. It can join only 
:doc:`infinite floors <floor>`.

Inputs
------

Floor
  Repeatable socket which expects floors to join

Properties
-----------------------

Match mode
  It determines how to handle the case when floors are shooter than
  base facade length.

  None
    In this case the floor will remain with a gap which the style was unable
    to cover.
  Repeat
    In this case if facade has longer length than floor
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
