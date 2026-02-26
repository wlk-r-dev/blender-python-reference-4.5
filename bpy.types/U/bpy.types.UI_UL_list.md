# UI_UL_list(UIList)

base classes — [`bpy_struct`](bpy.types.bpy_struct.html#bpy.types.bpy_struct "bpy.types.bpy_struct"), [`UIList`](bpy.types.UIList.html#bpy.types.UIList "bpy.types.UIList")

_class _bpy.types.UI_UL_list(_UIList_)
    

_static _filter_items_by_name(_pattern_ , _bitflag_ , _items_ , _propname ='name'_, _flags =None_, _reverse =False_)
    

Set FILTER_ITEM for items which name matches filter_name one (case-insensitive). pattern is the filtering pattern. propname is the name of the string property to use for filtering. flags must be a list of integers the same length as items, or None! return a list of flags (based on given flags if not None), or an empty list if no flags were given and no filtering has been done.

_classmethod _sort_items_by_name(_items_ , _propname ='name'_)
    

Re-order items using their names (case-insensitive). propname is the name of the string property to use for sorting. return a list mapping org_idx -> new_idx, or an empty list if no sorting has been done.

_static _sort_items_helper(_sort_data_ , _key_ , _reverse =False_)
    

Common sorting utility. Returns a neworder list mapping org_idx -> new_idx. sort_data must be an (unordered) list of tuples [(org_idx, …), (org_idx, …), …]. key must be the same kind of callable you would use for sorted() builtin function. reverse will reverse the sorting!

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
  * [`UIList.bl_idname`](bpy.types.UIList.html#bpy.types.UIList.bl_idname "bpy.types.UIList.bl_idname")
  * [`UIList.list_id`](bpy.types.UIList.html#bpy.types.UIList.list_id "bpy.types.UIList.list_id")
  * [`UIList.layout_type`](bpy.types.UIList.html#bpy.types.UIList.layout_type "bpy.types.UIList.layout_type")
  * [`UIList.use_filter_show`](bpy.types.UIList.html#bpy.types.UIList.use_filter_show "bpy.types.UIList.use_filter_show")
  * [`UIList.filter_name`](bpy.types.UIList.html#bpy.types.UIList.filter_name "bpy.types.UIList.filter_name")

| 

  * [`UIList.use_filter_invert`](bpy.types.UIList.html#bpy.types.UIList.use_filter_invert "bpy.types.UIList.use_filter_invert")
  * [`UIList.use_filter_sort_alpha`](bpy.types.UIList.html#bpy.types.UIList.use_filter_sort_alpha "bpy.types.UIList.use_filter_sort_alpha")
  * [`UIList.use_filter_sort_reverse`](bpy.types.UIList.html#bpy.types.UIList.use_filter_sort_reverse "bpy.types.UIList.use_filter_sort_reverse")
  * [`UIList.use_filter_sort_lock`](bpy.types.UIList.html#bpy.types.UIList.use_filter_sort_lock "bpy.types.UIList.use_filter_sort_lock")
  * [`UIList.bitflag_filter_item`](bpy.types.UIList.html#bpy.types.UIList.bitflag_filter_item "bpy.types.UIList.bitflag_filter_item")
  * [`UIList.bitflag_item_never_show`](bpy.types.UIList.html#bpy.types.UIList.bitflag_item_never_show "bpy.types.UIList.bitflag_item_never_show")

  
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
  * [`bpy_struct.keyframe_delete`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.keyframe_delete "bpy.types.bpy_struct.keyframe_delete")
  * [`bpy_struct.keyframe_insert`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.keyframe_insert "bpy.types.bpy_struct.keyframe_insert")
  * [`bpy_struct.keys`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.keys "bpy.types.bpy_struct.keys")
  * [`bpy_struct.path_from_id`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.path_from_id "bpy.types.bpy_struct.path_from_id")

| 

  * [`bpy_struct.path_resolve`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.path_resolve "bpy.types.bpy_struct.path_resolve")
  * [`bpy_struct.pop`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.pop "bpy.types.bpy_struct.pop")
  * [`bpy_struct.property_overridable_library_set`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.property_overridable_library_set "bpy.types.bpy_struct.property_overridable_library_set")
  * [`bpy_struct.property_unset`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.property_unset "bpy.types.bpy_struct.property_unset")
  * [`bpy_struct.rna_ancestors`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.rna_ancestors "bpy.types.bpy_struct.rna_ancestors")
  * [`bpy_struct.type_recast`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.type_recast "bpy.types.bpy_struct.type_recast")
  * [`bpy_struct.values`](bpy.types.bpy_struct.html#bpy.types.bpy_struct.values "bpy.types.bpy_struct.values")
  * [`UIList.draw_item`](bpy.types.UIList.html#bpy.types.UIList.draw_item "bpy.types.UIList.draw_item")
  * [`UIList.draw_filter`](bpy.types.UIList.html#bpy.types.UIList.draw_filter "bpy.types.UIList.draw_filter")
  * [`UIList.filter_items`](bpy.types.UIList.html#bpy.types.UIList.filter_items "bpy.types.UIList.filter_items")
  * [`UIList.append`](bpy.types.UIList.html#bpy.types.UIList.append "bpy.types.UIList.append")
  * [`UIList.is_extended`](bpy.types.UIList.html#bpy.types.UIList.is_extended "bpy.types.UIList.is_extended")
  * [`UIList.prepend`](bpy.types.UIList.html#bpy.types.UIList.prepend "bpy.types.UIList.prepend")
  * [`UIList.remove`](bpy.types.UIList.html#bpy.types.UIList.remove "bpy.types.UIList.remove")
  * [`UIList.bl_rna_get_subclass`](bpy.types.UIList.html#bpy.types.UIList.bl_rna_get_subclass "bpy.types.UIList.bl_rna_get_subclass")
  * [`UIList.bl_rna_get_subclass_py`](bpy.types.UIList.html#bpy.types.UIList.bl_rna_get_subclass_py "bpy.types.UIList.bl_rna_get_subclass_py")

  
---|---
