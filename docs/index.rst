.. Building Nodes documentation master file, created by
   sphinx-quickstart on Thu Nov 25 16:46:53 2021.

Welcome to Building Nodes's documentation!
==========================================

This is a tool for procedural generation of buildings. The work of the add-on is
similar to panel housing construction. The process is composed from three steps:

1. Creating :ref:`panels`. This should be done with standard Blender tools.
2. Creating building style. There is dedicated for this node tree editor.
3. Creating :ref:`base mesh <base_geometry>` which will be turned into a
   building. It also should be created with standard Blender modeling tools.

After the steps a building style can be applied to a base mesh. Instead of 
base mesh the add-on will create a building. Base mesh and building style can
be edited any moment and changes will be applied at once.

Main features
-------------

.. figure:: /images/Apply_style.*
   :align: center

   Once building style was created it can be applied to as many objects as you
   wish.

.. figure:: /images/Using_nodes.*
   :align: center

   Using nodes for creating building styles.

.. figure:: /images/Edit_facade.*
   :align: center

   Editing buildings in real time.


.. _limitations:

Limitations / roadmap
---------------------

- There are no any tools for roofs modeling. 
- Using Geometry nodes for generating base meshes is currently unsupported.
  Read :doc:`more <execution_system>`
- Using Loop cut tool with live update makes Blender to crush_. Using edge
  crease tool also works weird.
- Custom properties per building and node groups
  :ref:`are not supported <tree_editor>`.
- :ref:`Base mesh <base_geometry>` should consist only of quad polygons.
- Animation :doc:`is not supported <execution_system>`.

.. _crush: https://developer.blender.org/T67093

Some of this limitation should gone in future versions.


About me
--------

Since 2017 I'm developing open source Sverchok_ add-on and investigating
procedural approaches in 3D modeling. Some of my works can be found on Twitter_.
Because of active development of Geometry node project in the end of 2021 I 
decided take a break in Sverchok development and switch to this add-on.

.. _Sverchok: https://github.com/nortikin/sverchok
.. _Twitter: https://twitter.com/SoluSerg

Actually the add-on does not bring unique functionality. If not the same but
close result can be achieved in Sverchok. Something already is possible in
Geometry nodes and in future it also will be capable of such sort of things.

**What is advantage of this add-on over the mentioned projects?:**

- Ease of usage
- Achieve the same results with lesser nodes. In Sverchok you have to use
  hundreds ore even probably thousands of nodes.
- The work of the add-on nodes is intuitively clearer. The abstraction of the
  nodes is close to real world objects.
- No need in learning vector math, different algorithm of mesh processing and
  data structure of a geometry.


.. toctree::
   :maxdepth: 1

   quick_start
   installation
   user_interface
   data_structure
   execution_system
   nodes/categories
