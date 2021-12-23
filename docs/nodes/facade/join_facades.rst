=================
Join Facades Node
=================

This node can combine several facades into one by joining them together. It
can stack facades along X or along Z axis. It stacks facades only if they are
:doc:`finite <facade>`.

Inputs
------

Facade
  Repeatable socket which expects sequence of facades to be join.

Properties
----------

Direction
  It determines in which direction given facades should be joined to each other.

  Vertical
    In this mode facades will be put on top of each other.
  Horizontal
    In this mode facade styles will be put along length of initial facade.

Match mode
  It determines how to handle the case when facade styles are shooter than
  initial facade.

  None
    In this case the facade will remain with a gap which the style was unable
    to cover.
  Repeat
    In this case if base facade has longer length or height than facade styles
    can cover the remain space will be covered with last facade style.
  Cycle
    In this mode all given facade styles will be repeated if their size is 
    shooter than size of base facade. For example ``A B C`` facade styles are
    given. They can be stack with each other in next way ``A B C A B C A`` and
    so on.

Examples
--------

.. figure:: /images/nodes/Join_facades.*
   :width: 700 px

   Repeat some facade style with length 10 along horizontal axis.