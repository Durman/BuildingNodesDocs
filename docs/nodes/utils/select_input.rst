=================
Select Input Node
=================

This node can choose which upstream node should use downstream one.

Inputs
------

Input
  Repeatable socket which expects any node to be connected.

Properties
----------

Index
  Index of the input to be used. 0 index will shoos first connected input, 1
  the second and so on. If there is no input for given index the index will be
  ignored or will be converted according to the match property.

Match mode
  It determines how handle the case when given index is grater than number of
  given inputs.

  - **None**: ignore indexes which grater than inputs number.
  - **Repeat**: if index is greater than number of inputs it always selects the
    last one.
  - **Cycle**: it returns inputs as if they are infinitely repeated. For 
    example ``A B C`` inputs are given. Index 4 will select ``B`` because
    *A(0) -> B(1) -> C(2) -> A(3) -> B(4)*

Outputs
-------

Input
  Selected input

Examples
--------

.. figure:: /images/nodes/Panel_attr.*
   :width: 700 px

   Pick a panel according to it index.