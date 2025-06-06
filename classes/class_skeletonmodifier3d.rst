:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/SkeletonModifier3D.xml.

.. _class_SkeletonModifier3D:

SkeletonModifier3D
==================

**Inherits:** :ref:`Node3D<class_Node3D>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

**Inherited By:** :ref:`LookAtModifier3D<class_LookAtModifier3D>`, :ref:`PhysicalBoneSimulator3D<class_PhysicalBoneSimulator3D>`, :ref:`RetargetModifier3D<class_RetargetModifier3D>`, :ref:`SkeletonIK3D<class_SkeletonIK3D>`, :ref:`SpringBoneSimulator3D<class_SpringBoneSimulator3D>`, :ref:`XRBodyModifier3D<class_XRBodyModifier3D>`, :ref:`XRHandModifier3D<class_XRHandModifier3D>`

A node that may modify a Skeleton3D's bones.

.. rst-class:: classref-introduction-group

Description
-----------

**SkeletonModifier3D** retrieves a target :ref:`Skeleton3D<class_Skeleton3D>` by having a :ref:`Skeleton3D<class_Skeleton3D>` parent.

If there is an :ref:`AnimationMixer<class_AnimationMixer>`, a modification always performs after playback process of the :ref:`AnimationMixer<class_AnimationMixer>`.

This node should be used to implement custom IK solvers, constraints, or skeleton physics.

.. rst-class:: classref-introduction-group

Tutorials
---------

- `Design of the Skeleton Modifier 3D <https://godotengine.org/article/design-of-the-skeleton-modifier-3d/>`__

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +---------------------------+---------------------------------------------------------------+----------+
   | :ref:`bool<class_bool>`   | :ref:`active<class_SkeletonModifier3D_property_active>`       | ``true`` |
   +---------------------------+---------------------------------------------------------------+----------+
   | :ref:`float<class_float>` | :ref:`influence<class_SkeletonModifier3D_property_influence>` | ``1.0``  |
   +---------------------------+---------------------------------------------------------------+----------+

.. rst-class:: classref-reftable-group

Methods
-------

.. table::
   :widths: auto

   +-------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                              | :ref:`_process_modification<class_SkeletonModifier3D_private_method__process_modification>`\ (\ ) |virtual|                                                                                                 |
   +-------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                              | :ref:`_process_modification_with_delta<class_SkeletonModifier3D_private_method__process_modification_with_delta>`\ (\ delta\: :ref:`float<class_float>`\ ) |virtual|                                        |
   +-------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                              | :ref:`_skeleton_changed<class_SkeletonModifier3D_private_method__skeleton_changed>`\ (\ old_skeleton\: :ref:`Skeleton3D<class_Skeleton3D>`, new_skeleton\: :ref:`Skeleton3D<class_Skeleton3D>`\ ) |virtual| |
   +-------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                              | :ref:`_validate_bone_names<class_SkeletonModifier3D_private_method__validate_bone_names>`\ (\ ) |virtual|                                                                                                   |
   +-------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Skeleton3D<class_Skeleton3D>` | :ref:`get_skeleton<class_SkeletonModifier3D_method_get_skeleton>`\ (\ ) |const|                                                                                                                             |
   +-------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Signals
-------

.. _class_SkeletonModifier3D_signal_modification_processed:

.. rst-class:: classref-signal

**modification_processed**\ (\ ) :ref:`🔗<class_SkeletonModifier3D_signal_modification_processed>`

Notifies when the modification have been finished.

\ **Note:** If you want to get the modified bone pose by the modifier, you must use :ref:`Skeleton3D.get_bone_pose()<class_Skeleton3D_method_get_bone_pose>` or :ref:`Skeleton3D.get_bone_global_pose()<class_Skeleton3D_method_get_bone_global_pose>` at the moment this signal is fired.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Enumerations
------------

.. _enum_SkeletonModifier3D_BoneAxis:

.. rst-class:: classref-enumeration

enum **BoneAxis**: :ref:`🔗<enum_SkeletonModifier3D_BoneAxis>`

.. _class_SkeletonModifier3D_constant_BONE_AXIS_PLUS_X:

.. rst-class:: classref-enumeration-constant

:ref:`BoneAxis<enum_SkeletonModifier3D_BoneAxis>` **BONE_AXIS_PLUS_X** = ``0``

Enumerated value for the +X axis.

.. _class_SkeletonModifier3D_constant_BONE_AXIS_MINUS_X:

.. rst-class:: classref-enumeration-constant

:ref:`BoneAxis<enum_SkeletonModifier3D_BoneAxis>` **BONE_AXIS_MINUS_X** = ``1``

Enumerated value for the -X axis.

.. _class_SkeletonModifier3D_constant_BONE_AXIS_PLUS_Y:

.. rst-class:: classref-enumeration-constant

:ref:`BoneAxis<enum_SkeletonModifier3D_BoneAxis>` **BONE_AXIS_PLUS_Y** = ``2``

Enumerated value for the +Y axis.

.. _class_SkeletonModifier3D_constant_BONE_AXIS_MINUS_Y:

.. rst-class:: classref-enumeration-constant

:ref:`BoneAxis<enum_SkeletonModifier3D_BoneAxis>` **BONE_AXIS_MINUS_Y** = ``3``

Enumerated value for the -Y axis.

.. _class_SkeletonModifier3D_constant_BONE_AXIS_PLUS_Z:

.. rst-class:: classref-enumeration-constant

:ref:`BoneAxis<enum_SkeletonModifier3D_BoneAxis>` **BONE_AXIS_PLUS_Z** = ``4``

Enumerated value for the +Z axis.

.. _class_SkeletonModifier3D_constant_BONE_AXIS_MINUS_Z:

.. rst-class:: classref-enumeration-constant

:ref:`BoneAxis<enum_SkeletonModifier3D_BoneAxis>` **BONE_AXIS_MINUS_Z** = ``5``

Enumerated value for the -Z axis.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Property Descriptions
---------------------

.. _class_SkeletonModifier3D_property_active:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **active** = ``true`` :ref:`🔗<class_SkeletonModifier3D_property_active>`

.. rst-class:: classref-property-setget

- |void| **set_active**\ (\ value\: :ref:`bool<class_bool>`\ )
- :ref:`bool<class_bool>` **is_active**\ (\ )

If ``true``, the **SkeletonModifier3D** will be processing.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModifier3D_property_influence:

.. rst-class:: classref-property

:ref:`float<class_float>` **influence** = ``1.0`` :ref:`🔗<class_SkeletonModifier3D_property_influence>`

.. rst-class:: classref-property-setget

- |void| **set_influence**\ (\ value\: :ref:`float<class_float>`\ )
- :ref:`float<class_float>` **get_influence**\ (\ )

Sets the influence of the modification.

\ **Note:** This value is used by :ref:`Skeleton3D<class_Skeleton3D>` to blend, so the **SkeletonModifier3D** should always apply only 100% of the result without interpolation.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Method Descriptions
-------------------

.. _class_SkeletonModifier3D_private_method__process_modification:

.. rst-class:: classref-method

|void| **_process_modification**\ (\ ) |virtual| :ref:`🔗<class_SkeletonModifier3D_private_method__process_modification>`

**Deprecated:** Use :ref:`_process_modification_with_delta()<class_SkeletonModifier3D_private_method__process_modification_with_delta>` instead.

Override this virtual method to implement a custom skeleton modifier. You should do things like get the :ref:`Skeleton3D<class_Skeleton3D>`'s current pose and apply the pose here.

\ :ref:`_process_modification()<class_SkeletonModifier3D_private_method__process_modification>` must not apply :ref:`influence<class_SkeletonModifier3D_property_influence>` to bone poses because the :ref:`Skeleton3D<class_Skeleton3D>` automatically applies influence to all bone poses set by the modifier.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModifier3D_private_method__process_modification_with_delta:

.. rst-class:: classref-method

|void| **_process_modification_with_delta**\ (\ delta\: :ref:`float<class_float>`\ ) |virtual| :ref:`🔗<class_SkeletonModifier3D_private_method__process_modification_with_delta>`

Override this virtual method to implement a custom skeleton modifier. You should do things like get the :ref:`Skeleton3D<class_Skeleton3D>`'s current pose and apply the pose here.

\ :ref:`_process_modification_with_delta()<class_SkeletonModifier3D_private_method__process_modification_with_delta>` must not apply :ref:`influence<class_SkeletonModifier3D_property_influence>` to bone poses because the :ref:`Skeleton3D<class_Skeleton3D>` automatically applies influence to all bone poses set by the modifier.

\ ``delta`` is passed from parent :ref:`Skeleton3D<class_Skeleton3D>`. See also :ref:`Skeleton3D.advance()<class_Skeleton3D_method_advance>`.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModifier3D_private_method__skeleton_changed:

.. rst-class:: classref-method

|void| **_skeleton_changed**\ (\ old_skeleton\: :ref:`Skeleton3D<class_Skeleton3D>`, new_skeleton\: :ref:`Skeleton3D<class_Skeleton3D>`\ ) |virtual| :ref:`🔗<class_SkeletonModifier3D_private_method__skeleton_changed>`

Called when the skeleton is changed.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModifier3D_private_method__validate_bone_names:

.. rst-class:: classref-method

|void| **_validate_bone_names**\ (\ ) |virtual| :ref:`🔗<class_SkeletonModifier3D_private_method__validate_bone_names>`

Called when bone name and index need to be validated such as the timing of the entering tree or changing skeleton.

.. rst-class:: classref-item-separator

----

.. _class_SkeletonModifier3D_method_get_skeleton:

.. rst-class:: classref-method

:ref:`Skeleton3D<class_Skeleton3D>` **get_skeleton**\ (\ ) |const| :ref:`🔗<class_SkeletonModifier3D_method_get_skeleton>`

Get parent :ref:`Skeleton3D<class_Skeleton3D>` node if found.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
.. |bitfield| replace:: :abbr:`BitField (This value is an integer composed as a bitmask of the following flags.)`
.. |void| replace:: :abbr:`void (No return value.)`
