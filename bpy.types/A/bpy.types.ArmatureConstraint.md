# ArmatureConstraint(Constraint)

base classes — [`bpy_struct`](bpy.types.bpy_struct.md#bpy.types.bpy_struct "bpy.types.bpy_struct"), [`Constraint`](bpy.types.Constraint.md#bpy.types.Constraint "bpy.types.Constraint")

_class _bpy.types.ArmatureConstraint(_Constraint_)
    

Applies transformations done by the Armature modifier

targets
    

Target Bones

Type:
    

[`ArmatureConstraintTargets`](bpy.types.ArmatureConstraintTargets.md#bpy.types.ArmatureConstraintTargets "bpy.types.ArmatureConstraintTargets") [`bpy_prop_collection`](bpy.types.bpy_prop_collection.md#bpy.types.bpy_prop_collection "bpy.types.bpy_prop_collection") of [`ConstraintTargetBone`](bpy.types.ConstraintTargetBone.md#bpy.types.ConstraintTargetBone "bpy.types.ConstraintTargetBone"), (readonly)

use_bone_envelopes
    

Multiply weights by envelope for all bones, instead of acting like Vertex Group based blending. The specified weights are still used, and only the listed bones are considered.

Type:
    

boolean, default False

use_current_location
    

Use the current bone location for envelopes and choosing B-Bone segments instead of rest position

Type:
    

boolean, default False

use_deform_preserve_volume
    

Deform rotation interpolation with quaternions

Type:
    

boolean, default False

_classmethod _bl_rna_get_subclass(_id_ , _default =None_, _/_)
    

Parameters:
    

**id** (_str_) – The RNA type identifier.

Returns:
    

The RNA type or default when not found.

Return type:
    

[`bpy.types.Struct`](bpy.types.Struct.md#bpy.types.Struct "bpy.types.Struct") subclass

_classmethod _bl_rna_get_subclass_py(_id_ , _default =None_, _/_)
    

Parameters:
    

**id** (_str_) – The RNA type identifier.

Returns:
    

The class or default when not found.

Return type:
    

type

## Inherited Properties

  * [`bpy_struct.id_data`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.id_data "bpy.types.bpy_struct.id_data")
  * [`Constraint.name`](bpy.types.Constraint.md#bpy.types.Constraint.name "bpy.types.Constraint.name")
  * [`Constraint.type`](bpy.types.Constraint.md#bpy.types.Constraint.type "bpy.types.Constraint.type")
  * [`Constraint.is_override_data`](bpy.types.Constraint.md#bpy.types.Constraint.is_override_data "bpy.types.Constraint.is_override_data")
  * [`Constraint.owner_space`](bpy.types.Constraint.md#bpy.types.Constraint.owner_space "bpy.types.Constraint.owner_space")
  * [`Constraint.target_space`](bpy.types.Constraint.md#bpy.types.Constraint.target_space "bpy.types.Constraint.target_space")
  * [`Constraint.space_object`](bpy.types.Constraint.md#bpy.types.Constraint.space_object "bpy.types.Constraint.space_object")
  * [`Constraint.space_subtarget`](bpy.types.Constraint.md#bpy.types.Constraint.space_subtarget "bpy.types.Constraint.space_subtarget")

| 

  * [`Constraint.mute`](bpy.types.Constraint.md#bpy.types.Constraint.mute "bpy.types.Constraint.mute")
  * [`Constraint.enabled`](bpy.types.Constraint.md#bpy.types.Constraint.enabled "bpy.types.Constraint.enabled")
  * [`Constraint.show_expanded`](bpy.types.Constraint.md#bpy.types.Constraint.show_expanded "bpy.types.Constraint.show_expanded")
  * [`Constraint.is_valid`](bpy.types.Constraint.md#bpy.types.Constraint.is_valid "bpy.types.Constraint.is_valid")
  * [`Constraint.active`](bpy.types.Constraint.md#bpy.types.Constraint.active "bpy.types.Constraint.active")
  * [`Constraint.influence`](bpy.types.Constraint.md#bpy.types.Constraint.influence "bpy.types.Constraint.influence")
  * [`Constraint.error_location`](bpy.types.Constraint.md#bpy.types.Constraint.error_location "bpy.types.Constraint.error_location")
  * [`Constraint.error_rotation`](bpy.types.Constraint.md#bpy.types.Constraint.error_rotation "bpy.types.Constraint.error_rotation")

  
---|---  
  
## Inherited Functions

  * [`bpy_struct.as_pointer`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.as_pointer "bpy.types.bpy_struct.as_pointer")
  * [`bpy_struct.driver_add`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.driver_add "bpy.types.bpy_struct.driver_add")
  * [`bpy_struct.driver_remove`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.driver_remove "bpy.types.bpy_struct.driver_remove")
  * [`bpy_struct.get`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.get "bpy.types.bpy_struct.get")
  * [`bpy_struct.id_properties_clear`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.id_properties_clear "bpy.types.bpy_struct.id_properties_clear")
  * [`bpy_struct.id_properties_ensure`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.id_properties_ensure "bpy.types.bpy_struct.id_properties_ensure")
  * [`bpy_struct.id_properties_ui`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.id_properties_ui "bpy.types.bpy_struct.id_properties_ui")
  * [`bpy_struct.is_property_hidden`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.is_property_hidden "bpy.types.bpy_struct.is_property_hidden")
  * [`bpy_struct.is_property_overridable_library`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.is_property_overridable_library "bpy.types.bpy_struct.is_property_overridable_library")
  * [`bpy_struct.is_property_readonly`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.is_property_readonly "bpy.types.bpy_struct.is_property_readonly")
  * [`bpy_struct.is_property_set`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.is_property_set "bpy.types.bpy_struct.is_property_set")
  * [`bpy_struct.items`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.items "bpy.types.bpy_struct.items")
  * [`bpy_struct.keyframe_delete`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.keyframe_delete "bpy.types.bpy_struct.keyframe_delete")

| 

  * [`bpy_struct.keyframe_insert`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.keyframe_insert "bpy.types.bpy_struct.keyframe_insert")
  * [`bpy_struct.keys`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.keys "bpy.types.bpy_struct.keys")
  * [`bpy_struct.path_from_id`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.path_from_id "bpy.types.bpy_struct.path_from_id")
  * [`bpy_struct.path_resolve`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.path_resolve "bpy.types.bpy_struct.path_resolve")
  * [`bpy_struct.pop`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.pop "bpy.types.bpy_struct.pop")
  * [`bpy_struct.property_overridable_library_set`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.property_overridable_library_set "bpy.types.bpy_struct.property_overridable_library_set")
  * [`bpy_struct.property_unset`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.property_unset "bpy.types.bpy_struct.property_unset")
  * [`bpy_struct.rna_ancestors`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.rna_ancestors "bpy.types.bpy_struct.rna_ancestors")
  * [`bpy_struct.type_recast`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.type_recast "bpy.types.bpy_struct.type_recast")
  * [`bpy_struct.values`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.values "bpy.types.bpy_struct.values")
  * [`Constraint.bl_rna_get_subclass`](bpy.types.Constraint.md#bpy.types.Constraint.bl_rna_get_subclass "bpy.types.Constraint.bl_rna_get_subclass")
  * [`Constraint.bl_rna_get_subclass_py`](bpy.types.Constraint.md#bpy.types.Constraint.bl_rna_get_subclass_py "bpy.types.Constraint.bl_rna_get_subclass_py")

  
---|---
