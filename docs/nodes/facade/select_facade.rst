==================
Select Facade Node
==================

The nodes gives possibility of choosing facades by an index.

Inputs
------

Facade
  Repeatable socket of arbitrary sequence of facades 

Properties
----------

Match mode
  It determines how handle the case when given index is grater than number of
  given facades.

  - None
      Ignore indexes which grater than facades number.
  - Repeat
      If index is greater than number of facades it always selects the last
      facade.
  - Cycle
      It returns facades as if they are infinitely repeated. For example 
      ``A B C`` facades are given. Index 4 will select ``B`` because 
      *A(0) -> B(1) -> C(2) -> A(3) -> B(4)*

Index
  Index of the facade to be used. 0 index will shoos first connected facade, 1
  the second and so on. If there is no facades for given index the index will be
  ignored.

Outputs
-------

Facade
  Selected facade.

Examples
--------

.. figure:: /images/nodes/Select_facade.*
   :width: 700 px

   Using facade according to its material index.