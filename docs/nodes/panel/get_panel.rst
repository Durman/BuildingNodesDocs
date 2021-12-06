==============
Get Panel Node
==============

This node can choose one Panel from their collection according to the given
index.

Inputs
------

Panels
  Repeatable socket which expect collection of input panels

Properties
----------

Index
  Index of the panel. If the index is greater than number of given panels
  the node handle this according to its mode property.

Mode
  It determines how to handle the case when given index is grater than number
  of given panels.

  * **None:** Nothing will be return
  * **Repeat:** Last panel will be return
  * **Cycle:** In this mode when an index goes out of bounds it returns back
    to the start of the collection with index decreased to number of
    elements in the collection. This operation repeats till the proper panel
    won't be found. For example in collection of 3 numbers ``0, 1, 2``
    an index ``4`` points to number ``1``.

Outputs
-------

Panel
  Panel chosen by the index

Examples
--------
