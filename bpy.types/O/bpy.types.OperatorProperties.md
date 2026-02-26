# OperatorProperties(bpy_struct)

base class — [`bpy_struct`](bpy.types.bpy_struct.md#bpy.types.bpy_struct "bpy.types.bpy_struct")

_class _bpy.types.OperatorProperties(_bpy_struct_)
    

Input properties of an operator

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

| 


  
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

| 

  * [`bpy_struct.keyframe_delete`](bpy.types.bpy_struct.md#bpy.types.bpy_struct.keyframe_delete "bpy.types.bpy_struct.keyframe_delete")
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

  
---|---  
  
## References

  * [`Gizmo.target_set_operator`](bpy.types.Gizmo.md#bpy.types.Gizmo.target_set_operator "bpy.types.Gizmo.target_set_operator")
  * [`KeyConfigurations.find_item_from_operator`](bpy.types.KeyConfigurations.md#bpy.types.KeyConfigurations.find_item_from_operator "bpy.types.KeyConfigurations.find_item_from_operator")
  * [`KeyMapItem.properties`](bpy.types.KeyMapItem.md#bpy.types.KeyMapItem.properties "bpy.types.KeyMapItem.properties")
  * [`KeyMapItems.find_from_operator`](bpy.types.KeyMapItems.md#bpy.types.KeyMapItems.find_from_operator "bpy.types.KeyMapItems.find_from_operator")
  * [`Macro.properties`](bpy.types.Macro.md#bpy.types.Macro.properties "bpy.types.Macro.properties")
  * [`Operator.description`](bpy.types.Operator.md#bpy.types.Operator.description "bpy.types.Operator.description")
  * [`Operator.properties`](bpy.types.Operator.md#bpy.types.Operator.properties "bpy.types.Operator.properties")
  * [`OperatorMacro.properties`](bpy.types.OperatorMacro.md#bpy.types.OperatorMacro.properties "bpy.types.OperatorMacro.properties")
  * [`UILayout.operator`](bpy.types.UILayout.md#bpy.types.UILayout.operator "bpy.types.UILayout.operator")

| 

  * [`UILayout.operator_menu_enum`](bpy.types.UILayout.md#bpy.types.UILayout.operator_menu_enum "bpy.types.UILayout.operator_menu_enum")
  * [`UILayout.operator_menu_hold`](bpy.types.UILayout.md#bpy.types.UILayout.operator_menu_hold "bpy.types.UILayout.operator_menu_hold")
  * [`UILayout.template_asset_view`](bpy.types.UILayout.md#bpy.types.UILayout.template_asset_view "bpy.types.UILayout.template_asset_view")
  * [`UILayout.template_asset_view`](bpy.types.UILayout.md#bpy.types.UILayout.template_asset_view "bpy.types.UILayout.template_asset_view")
  * [`UILayout.template_popup_confirm`](bpy.types.UILayout.md#bpy.types.UILayout.template_popup_confirm "bpy.types.UILayout.template_popup_confirm")
  * [`WindowManager.operator_properties_last`](bpy.types.WindowManager.md#bpy.types.WindowManager.operator_properties_last "bpy.types.WindowManager.operator_properties_last")
  * [`WorkSpaceTool.operator_properties`](bpy.types.WorkSpaceTool.md#bpy.types.WorkSpaceTool.operator_properties "bpy.types.WorkSpaceTool.operator_properties")
  * [`XrActionMapItem.op_properties`](bpy.types.XrActionMapItem.md#bpy.types.XrActionMapItem.op_properties "bpy.types.XrActionMapItem.op_properties")

  
---|---
