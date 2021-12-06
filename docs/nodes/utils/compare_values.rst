===================
Compare Values Node
===================

The node performs comparison operations.

Properties
----------

Operation
  Comparison operation to use

  * **Equal:** true if two values are equal
  * **Is close:** true if tow values are close to each other according to
    given maximum possible difference
  * **Not equal:** true if two values are not equal
  * **Grater than:** true if first value is grater
  * **Grater or equal:** true if first value grater or equal to the second one
  * **Less than:**  true if first value is less
  * **Less or equal:**  true if first values is less or equal to the second one

Float
  First value

Float
  Second value

Tolerance (Is close mode)
  Maximum difference between values after which they are recognized as unequal

Outputs
-------

Bool
  True of False value