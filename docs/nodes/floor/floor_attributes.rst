=====================
Floor Attributes Node
=====================

This node outputs :ref:`floor <floors>` attributes as :ref:`fields`.

Outputs
-------

Index
  Index of the current floor. It is incremented only by Fill socket of
  :doc:`floor`. Indexing is starting from 0 value. Don't mix
  this with floor number. 0 index does not necessarily coincide with ground
  floor. This is true only if facade is starting from the ground.

Examples
--------

.. figure:: /images/nodes/Floor_attr.*
   :width: 700 px

   Choose floor according its index.
