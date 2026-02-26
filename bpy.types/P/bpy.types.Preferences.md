# Preferences(bpy_struct)

base class — [`bpy_struct`](bpy.types.bpy_struct.html#bpy.types.bpy_struct "bpy.types.bpy_struct")

_class _bpy.types.Preferences(_bpy_struct_)
    

Global preferences

active_section
    

Preferences

Type:
    

enum in [Preference Section Items](bpy_types_enum_items/preference_section_items.html#rna-enum-preference-section-items), default `'INTERFACE'`

addons
    

Type:
    

[`Addons`](bpy.types.Addons.html#bpy.types.Addons "bpy.types.Addons") [`bpy_prop_collection`](bpy.types.bpy_prop_collection.html#bpy.types.bpy_prop_collection "bpy.types.bpy_prop_collection") of [`Addon`](bpy.types.Addon.html#bpy.types.Addon "bpy.types.Addon"), (readonly)

app_template
    

Type:
    

string, default “”, (never None)

apps
    

Preferences that work only for apps

Type:
    

[`PreferencesApps`](bpy.types.PreferencesApps.html#bpy.types.PreferencesApps "bpy.types.PreferencesApps"), (readonly, never None)

autoexec_paths
    

Type:
    

[`PathCompareCollection`](bpy.types.PathCompareCollection.html#bpy.types.PathCompareCollection "bpy.types.PathCompareCollection") [`bpy_prop_collection`](bpy.types.bpy_prop_collection.html#bpy.types.bpy_prop_collection "bpy.types.bpy_prop_collection") of [`PathCompare`](bpy.types.PathCompare.html#bpy.types.PathCompare "bpy.types.PathCompare"), (readonly)

edit
    

Settings for interacting with Blender data

Type:
    

[`PreferencesEdit`](bpy.types.PreferencesEdit.html#bpy.types.PreferencesEdit "bpy.types.PreferencesEdit"), (readonly, never None)

experimental
    

Settings for features that are still early in their development stage

Type:
    

[`PreferencesExperimental`](bpy.types.PreferencesExperimental.html#bpy.types.PreferencesExperimental "bpy.types.PreferencesExperimental"), (readonly, never None)

extensions
    

Settings for extensions

Type:
    

[`PreferencesExtensions`](bpy.types.PreferencesExtensions.html#bpy.types.PreferencesExtensions "bpy.types.PreferencesExtensions"), (readonly, never None)

filepaths
    

Default paths for external files

Type:
    

[`PreferencesFilePaths`](bpy.types.PreferencesFilePaths.html#bpy.types.PreferencesFilePaths "bpy.types.PreferencesFilePaths"), (readonly, never None)

inputs
    

Settings for input devices

Type:
    

[`PreferencesInput`](bpy.types.PreferencesInput.html#bpy.types.PreferencesInput "bpy.types.PreferencesInput"), (readonly, never None)

is_dirty
    

Preferences have changed

Type:
    

boolean, default False

keymap
    

Shortcut setup for keyboards and other input devices

Type:
    

[`PreferencesKeymap`](bpy.types.PreferencesKeymap.html#bpy.types.PreferencesKeymap "bpy.types.PreferencesKeymap"), (readonly, never None)

studio_lights
    

Type:
    

[`StudioLights`](bpy.types.StudioLights.html#bpy.types.StudioLights "bpy.types.StudioLights") [`bpy_prop_collection`](bpy.types.bpy_prop_collection.html#bpy.types.bpy_prop_collection "bpy.types.bpy_prop_collection") of [`StudioLight`](bpy.types.StudioLight.html#bpy.types.StudioLight "bpy.types.StudioLight"), (readonly)

system
    

Graphics driver and operating system settings

Type:
    

[`PreferencesSystem`](bpy.types.PreferencesSystem.html#bpy.types.PreferencesSystem "bpy.types.PreferencesSystem"), (readonly, never None)

themes
    

Type:
    

[`bpy_prop_collection`](bpy.types.bpy_prop_collection.html#bpy.types.bpy_prop_collection "bpy.types.bpy_prop_collection") of [`Theme`](bpy.types.Theme.html#bpy.types.Theme "bpy.types.Theme"), (readonly)

ui_styles
    

Type:
    

[`bpy_prop_collection`](bpy.types.bpy_prop_collection.html#bpy.types.bpy_prop_collection "bpy.types.bpy_prop_collection") of [`ThemeStyle`](bpy.types.ThemeStyle.html#bpy.types.ThemeStyle "bpy.types.ThemeStyle"), (readonly)

use_preferences_save
    

Save preferences on exit when modified (unless factory settings have been loaded)

Type:
    

boolean, default True

use_recent_searches
    

Sort the recently searched items at the top

Type:
    

boolean, default True

version
    

Version of Blender the userpref.blend was saved with

Type:
    

int array of 3 items in [0, inf], default (0, 0, 0), (readonly)

view
    

Preferences related to viewing data

Type:
    

[`PreferencesView`](bpy.types.PreferencesView.html#bpy.types.PreferencesView "bpy.types.PreferencesView"), (readonly, never None)

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

  * [`Context.preferences`](bpy.types.Context.html#bpy.types.Context.preferences "bpy.types.Context.preferences")

| 


  
---|---
