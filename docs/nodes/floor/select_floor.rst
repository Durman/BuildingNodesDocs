=================
Select Floor Node
=================

The nodes gives possibility of choosing floor by an index.

Inputs
------

Floor
  Repeatable socket of arbitrary sequence of floors 

Properties
----------

Match mode
  It determines how handle the case when given index is grater than number of
  given floors.

  - None
      Ignore indexes which grater than floors number.
  - Repeat
      If index is greater than number of floors it always selects the last
      floor.
  - Cycle
      It returns floors as if they are infinitely repeated. For example 
      ``A B C`` floors are given. Index 4 will select ``B`` because 
      *A(0) -> B(1) -> C(2) -> A(3) -> B(4)*

Index
  Index of the floor to be used. 0 index will shoos first connected floor, 1
  the second and so on. If there is no floors for given index the index will be
  ignored.

Outputs
-------

Floor
  Selected floor.

Examples
--------

.. figure:: /images/nodes/Floor_attr.*
   :width: 700 px

   Choose floor according its index.
