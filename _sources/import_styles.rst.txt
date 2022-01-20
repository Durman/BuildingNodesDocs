======================
Import Building Styles
======================

If you created a complex building style you may want to use it in different
projects. In order to do this you have to import the style in different files
somehow. This is possible to do with Blender append functionality.

.. image:: /images/Import_style1.*

- Use ``Topbar -> File -> Append``
- In the appeared window browse to the file from which you want to import a
  building style.
- Open the file
- Inside the file you will find *Node tree* folder. If there is no such folder
  then the file does not have any Building styles.
- Open *Node tree* folder

.. image:: /images/Import_style2.*

- Inside the folder find the name of the style (or names) you want to import
  and press append button.

Importing of a style is going with all dependent panels. After the import
you can use it inside the file. Read more how to use styles in 
:doc:`quick_start`, only instead of creating new style select the imported
style.

.. note::
   In future Blender may support adding custom node groups to the asset manager
   in this case sharing of building styles will be even simpler.
