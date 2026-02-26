# ShaderFx(bpy_struct)

base class — [`bpy_struct`](bpy.types.bpy_struct.html#bpy.types.bpy_struct "bpy.types.bpy_struct")

subclasses — [`ShaderFxBlur`](bpy.types.ShaderFxBlur.html#bpy.types.ShaderFxBlur "bpy.types.ShaderFxBlur"), [`ShaderFxColorize`](bpy.types.ShaderFxColorize.html#bpy.types.ShaderFxColorize "bpy.types.ShaderFxColorize"), [`ShaderFxFlip`](bpy.types.ShaderFxFlip.html#bpy.types.ShaderFxFlip "bpy.types.ShaderFxFlip"), [`ShaderFxGlow`](bpy.types.ShaderFxGlow.html#bpy.types.ShaderFxGlow "bpy.types.ShaderFxGlow"), [`ShaderFxPixel`](bpy.types.ShaderFxPixel.html#bpy.types.ShaderFxPixel "bpy.types.ShaderFxPixel"), [`ShaderFxRim`](bpy.types.ShaderFxRim.html#bpy.types.ShaderFxRim "bpy.types.ShaderFxRim"), [`ShaderFxShadow`](bpy.types.ShaderFxShadow.html#bpy.types.ShaderFxShadow "bpy.types.ShaderFxShadow"), [`ShaderFxSwirl`](bpy.types.ShaderFxSwirl.html#bpy.types.ShaderFxSwirl "bpy.types.ShaderFxSwirl"), [`ShaderFxWave`](bpy.types.ShaderFxWave.html#bpy.types.ShaderFxWave "bpy.types.ShaderFxWave")

_class _bpy.types.ShaderFx(_bpy_struct_)
    

Effect affecting the Grease Pencil object

name
    

Effect name

Type:
    

string, default “”, (never None)

show_expanded
    

Set effect expansion in the user interface

Type:
    

boolean, default False

show_in_editmode
    

Display effect in Edit mode

Type:
    

boolean, default False

show_render
    

Use effect during render

Type:
    

boolean, default False

show_viewport
    

Display effect in viewport

Type:
    

boolean, default False

type
    

Type:
    

enum in [Object Shaderfx Type Items](bpy_types_enum_items/object_shaderfx_type_items.html#rna-enum-object-shaderfx-type-items), default `'FX_BLUR'`, (readonly)

_classmethod _bl_rna_get_subclass(_id_ , _default =None_, _/_)
    

Parameters:
    

**id** (_str_) – The RNA type identifier.

Returns:
    

The RNA type or default when not found.

Return type:
    

[`bpy.types.Struct`](bpy.types.Struct.html#bpy.types.Struct "bpy.types.Struct") subclass

_classmethod _bl_rna_get_subclass_py(_id_ , _default =None_, _/_)
    

Parameters:
    

**id** (_str_) – The RNA type identifier.

Returns:
    

The class or default when not found.

Return type:
    

type

## Inherited Properties

  * [`bpy_struct.id_data`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.id_data "bpy.types.bpy_struct.id_data")

| 


  
---|---  
  
## Inherited Functions

  * [`bpy_struct.as_pointer`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.as_pointer "bpy.types.bpy_struct.as_pointer")
  * [`bpy_struct.driver_add`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.driver_add "bpy.types.bpy_struct.driver_add")
  * [`bpy_struct.driver_remove`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.driver_remove "bpy.types.bpy_struct.driver_remove")
  * [`bpy_struct.get`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.get "bpy.types.bpy_struct.get")
  * [`bpy_struct.id_properties_clear`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.id_properties_clear "bpy.types.bpy_struct.id_properties_clear")
  * [`bpy_struct.id_properties_ensure`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.id_properties_ensure "bpy.types.bpy_struct.id_properties_ensure")
  * [`bpy_struct.id_properties_ui`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.id_properties_ui "bpy.types.bpy_struct.id_properties_ui")
  * [`bpy_struct.is_property_hidden`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.is_property_hidden "bpy.types.bpy_struct.is_property_hidden")
  * [`bpy_struct.is_property_overridable_library`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.is_property_overridable_library "bpy.types.bpy_struct.is_property_overridable_library")
  * [`bpy_struct.is_property_readonly`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.is_property_readonly "bpy.types.bpy_struct.is_property_readonly")
  * [`bpy_struct.is_property_set`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.is_property_set "bpy.types.bpy_struct.is_property_set")
  * [`bpy_struct.items`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.items "bpy.types.bpy_struct.items")

| 

  * [`bpy_struct.keyframe_delete`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.keyframe_delete "bpy.types.bpy_struct.keyframe_delete")
  * [`bpy_struct.keyframe_insert`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.keyframe_insert "bpy.types.bpy_struct.keyframe_insert")
  * [`bpy_struct.keys`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.keys "bpy.types.bpy_struct.keys")
  * [`bpy_struct.path_from_id`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.path_from_id "bpy.types.bpy_struct.path_from_id")
  * [`bpy_struct.path_resolve`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.path_resolve "bpy.types.bpy_struct.path_resolve")
  * [`bpy_struct.pop`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.pop "bpy.types.bpy_struct.pop")
  * [`bpy_struct.property_overridable_library_set`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.property_overridable_library_set "bpy.types.bpy_struct.property_overridable_library_set")
  * [`bpy_struct.property_unset`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.property_unset "bpy.types.bpy_struct.property_unset")
  * [`bpy_struct.rna_ancestors`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.rna_ancestors "bpy.types.bpy_struct.rna_ancestors")
  * [`bpy_struct.type_recast`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.type_recast "bpy.types.bpy_struct.type_recast")
  * [`bpy_struct.values`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.values "bpy.types.bpy_struct.values")

  
---|---  
  
## References

  * [`Object.shader_effects`](bpy.types.Object.html#bpy.types.Object.shader_effects "bpy.types.Object.shader_effects")
  * [`ObjectShaderFx.new`](bpy.types.ObjectShaderFx.html#bpy.types.ObjectShaderFx.new "bpy.types.ObjectShaderFx.new")

| 

  * [`ObjectShaderFx.remove`](bpy.types.ObjectShaderFx.html#bpy.types.ObjectShaderFx.remove "bpy.types.ObjectShaderFx.remove")

  
---|---
