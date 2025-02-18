:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/modules/gltf/doc_classes/GLTFCamera.xml.

.. _class_GLTFCamera:

GLTFCamera
==========

**Inherits:** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

Represents a GLTF camera.

.. rst-class:: classref-introduction-group

Description
-----------

Represents a camera as defined by the base GLTF spec.

.. rst-class:: classref-introduction-group

Tutorials
---------

- `GLTF camera detailed specification <https://registry.khronos.org/glTF/specs/2.0/glTF-2.0.html#reference-camera>`__

- `GLTF camera spec and example file <https://github.com/KhronosGroup/glTF-Tutorials/blob/master/gltfTutorial/gltfTutorial_015_SimpleCameras.md>`__

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +---------------------------+-----------------------------------------------------------+------------+
   | :ref:`float<class_float>` | :ref:`depth_far<class_GLTFCamera_property_depth_far>`     | ``4000.0`` |
   +---------------------------+-----------------------------------------------------------+------------+
   | :ref:`float<class_float>` | :ref:`depth_near<class_GLTFCamera_property_depth_near>`   | ``0.05``   |
   +---------------------------+-----------------------------------------------------------+------------+
   | :ref:`float<class_float>` | :ref:`fov<class_GLTFCamera_property_fov>`                 | ``1.309``  |
   +---------------------------+-----------------------------------------------------------+------------+
   | :ref:`bool<class_bool>`   | :ref:`perspective<class_GLTFCamera_property_perspective>` | ``true``   |
   +---------------------------+-----------------------------------------------------------+------------+
   | :ref:`float<class_float>` | :ref:`size_mag<class_GLTFCamera_property_size_mag>`       | ``0.5``    |
   +---------------------------+-----------------------------------------------------------+------------+

.. rst-class:: classref-reftable-group

Methods
-------

.. table::
   :widths: auto

   +-------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`GLTFCamera<class_GLTFCamera>` | :ref:`from_dictionary<class_GLTFCamera_method_from_dictionary>` **(** :ref:`Dictionary<class_Dictionary>` dictionary **)** |static| |
   +-------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`GLTFCamera<class_GLTFCamera>` | :ref:`from_node<class_GLTFCamera_method_from_node>` **(** :ref:`Camera3D<class_Camera3D>` camera_node **)** |static|                |
   +-------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Dictionary<class_Dictionary>` | :ref:`to_dictionary<class_GLTFCamera_method_to_dictionary>` **(** **)** |const|                                                     |
   +-------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Camera3D<class_Camera3D>`     | :ref:`to_node<class_GLTFCamera_method_to_node>` **(** **)** |const|                                                                 |
   +-------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Property Descriptions
---------------------

.. _class_GLTFCamera_property_depth_far:

.. rst-class:: classref-property

:ref:`float<class_float>` **depth_far** = ``4000.0``

.. rst-class:: classref-property-setget

- void **set_depth_far** **(** :ref:`float<class_float>` value **)**
- :ref:`float<class_float>` **get_depth_far** **(** **)**

The distance to the far culling boundary for this camera relative to its local Z axis, in meters. This maps to GLTF's ``zfar`` property.

.. rst-class:: classref-item-separator

----

.. _class_GLTFCamera_property_depth_near:

.. rst-class:: classref-property

:ref:`float<class_float>` **depth_near** = ``0.05``

.. rst-class:: classref-property-setget

- void **set_depth_near** **(** :ref:`float<class_float>` value **)**
- :ref:`float<class_float>` **get_depth_near** **(** **)**

The distance to the near culling boundary for this camera relative to its local Z axis, in meters. This maps to GLTF's ``znear`` property.

.. rst-class:: classref-item-separator

----

.. _class_GLTFCamera_property_fov:

.. rst-class:: classref-property

:ref:`float<class_float>` **fov** = ``1.309``

.. rst-class:: classref-property-setget

- void **set_fov** **(** :ref:`float<class_float>` value **)**
- :ref:`float<class_float>` **get_fov** **(** **)**

The FOV of the camera. This class and GLTF define the camera FOV in radians, while Godot uses degrees. This maps to GLTF's ``yfov`` property. This value is only used for perspective cameras, when :ref:`perspective<class_GLTFCamera_property_perspective>` is true.

.. rst-class:: classref-item-separator

----

.. _class_GLTFCamera_property_perspective:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **perspective** = ``true``

.. rst-class:: classref-property-setget

- void **set_perspective** **(** :ref:`bool<class_bool>` value **)**
- :ref:`bool<class_bool>` **get_perspective** **(** **)**

Whether or not the camera is in perspective mode. If false, the camera is in orthographic/orthogonal mode. This maps to GLTF's camera ``type`` property. See :ref:`Camera3D.projection<class_Camera3D_property_projection>` and the GLTF spec for more information.

.. rst-class:: classref-item-separator

----

.. _class_GLTFCamera_property_size_mag:

.. rst-class:: classref-property

:ref:`float<class_float>` **size_mag** = ``0.5``

.. rst-class:: classref-property-setget

- void **set_size_mag** **(** :ref:`float<class_float>` value **)**
- :ref:`float<class_float>` **get_size_mag** **(** **)**

The size of the camera. This class and GLTF define the camera size magnitude as a radius in meters, while Godot defines it as a diameter in meters. This maps to GLTF's ``ymag`` property. This value is only used for orthographic/orthogonal cameras, when :ref:`perspective<class_GLTFCamera_property_perspective>` is false.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Method Descriptions
-------------------

.. _class_GLTFCamera_method_from_dictionary:

.. rst-class:: classref-method

:ref:`GLTFCamera<class_GLTFCamera>` **from_dictionary** **(** :ref:`Dictionary<class_Dictionary>` dictionary **)** |static|

Creates a new GLTFCamera instance by parsing the given :ref:`Dictionary<class_Dictionary>`.

.. rst-class:: classref-item-separator

----

.. _class_GLTFCamera_method_from_node:

.. rst-class:: classref-method

:ref:`GLTFCamera<class_GLTFCamera>` **from_node** **(** :ref:`Camera3D<class_Camera3D>` camera_node **)** |static|

Create a new GLTFCamera instance from the given Godot :ref:`Camera3D<class_Camera3D>` node.

.. rst-class:: classref-item-separator

----

.. _class_GLTFCamera_method_to_dictionary:

.. rst-class:: classref-method

:ref:`Dictionary<class_Dictionary>` **to_dictionary** **(** **)** |const|

Serializes this GLTFCamera instance into a :ref:`Dictionary<class_Dictionary>`.

.. rst-class:: classref-item-separator

----

.. _class_GLTFCamera_method_to_node:

.. rst-class:: classref-method

:ref:`Camera3D<class_Camera3D>` **to_node** **(** **)** |const|

Converts this GLTFCamera instance into a Godot :ref:`Camera3D<class_Camera3D>` node.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
