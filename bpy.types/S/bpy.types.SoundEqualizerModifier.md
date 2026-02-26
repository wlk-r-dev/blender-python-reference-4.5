# SoundEqualizerModifier(StripModifier)

base classes — [`bpy_struct`](bpy.types.bpy_struct.md#bpy.types.bpy_struct "bpy.types.bpy_struct"), [`StripModifier`](bpy.types.StripModifier.md#bpy.types.StripModifier "bpy.types.StripModifier")

_class _bpy.types.SoundEqualizerModifier(_StripModifier_)
    

Equalize audio

graphics
    

Graphical definition equalization

Type:
    

[`bpy_prop_collection`](bpy.types.bpy_prop_collection.md#bpy.types.bpy_prop_collection "bpy.types.bpy_prop_collection") of [`EQCurveMappingData`](bpy.types.EQCurveMappingData.md#bpy.types.EQCurveMappingData "bpy.types.EQCurveMappingData"), (readonly)

new_graphic(_min_freq_ , _max_freq_)
    

Add a new EQ band

Parameters:
    

  * **min_freq** (_float in_ _[__0_ _,__20000_ _]_) – Minimum Frequency, Minimum Frequency

  * **max_freq** (_float in_ _[__0_ _,__20000_ _]_) – Maximum Frequency, Maximum Frequency


Returns:
    

Newly created graphical Equalizer definition

Return type:
    

[`EQCurveMappingData`](bpy.types.EQCurveMappingData.md#bpy.types.EQCurveMappingData "bpy.types.EQCurveMappingData")

clear_soundeqs()
    

Remove all graphical equalizers from the Equalizer modifier

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
  * [`StripModifier.name`](bpy.types.StripModifier.md#bpy.types.StripModifier.name "bpy.types.StripModifier.name")
  * [`StripModifier.type`](bpy.types.StripModifier.md#bpy.types.StripModifier.type "bpy.types.StripModifier.type")
  * [`StripModifier.mute`](bpy.types.StripModifier.md#bpy.types.StripModifier.mute "bpy.types.StripModifier.mute")
  * [`StripModifier.show_expanded`](bpy.types.StripModifier.md#bpy.types.StripModifier.show_expanded "bpy.types.StripModifier.show_expanded")

| 

  * [`StripModifier.input_mask_type`](bpy.types.StripModifier.md#bpy.types.StripModifier.input_mask_type "bpy.types.StripModifier.input_mask_type")
  * [`StripModifier.mask_time`](bpy.types.StripModifier.md#bpy.types.StripModifier.mask_time "bpy.types.StripModifier.mask_time")
  * [`StripModifier.input_mask_strip`](bpy.types.StripModifier.md#bpy.types.StripModifier.input_mask_strip "bpy.types.StripModifier.input_mask_strip")
  * [`StripModifier.input_mask_id`](bpy.types.StripModifier.md#bpy.types.StripModifier.input_mask_id "bpy.types.StripModifier.input_mask_id")

  
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
  * [`StripModifier.bl_rna_get_subclass`](bpy.types.StripModifier.md#bpy.types.StripModifier.bl_rna_get_subclass "bpy.types.StripModifier.bl_rna_get_subclass")
  * [`StripModifier.bl_rna_get_subclass_py`](bpy.types.StripModifier.md#bpy.types.StripModifier.bl_rna_get_subclass_py "bpy.types.StripModifier.bl_rna_get_subclass_py")

  
---|---
