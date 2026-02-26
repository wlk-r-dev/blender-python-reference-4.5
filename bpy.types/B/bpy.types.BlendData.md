# BlendData(bpy_struct)

base class — [[bpy_struct]]

_class _bpy.types.BlendData(_bpy_struct_)
    

Main data structure representing a .blend file and all its data-blocks

actions
    

Action data-blocks

Type:
    

[[BlendDataActions]] [[bpy_prop_collection]] of [[Action]], (readonly)

armatures
    

Armature data-blocks

Type:
    

[[BlendDataArmatures]] [[bpy_prop_collection]] of [[Armature]], (readonly)

brushes
    

Brush data-blocks

Type:
    

[[BlendDataBrushes]] [[bpy_prop_collection]] of [[Brush]], (readonly)

cache_files
    

Cache Files data-blocks

Type:
    

[[BlendDataCacheFiles]] [[bpy_prop_collection]] of [[CacheFile]], (readonly)

cameras
    

Camera data-blocks

Type:
    

[[BlendDataCameras]] [[bpy_prop_collection]] of [[Camera]], (readonly)

collections
    

Collection data-blocks

Type:
    

[[BlendDataCollections]] [[bpy_prop_collection]] of [[Collection]], (readonly)

curves
    

Curve data-blocks

Type:
    

[[BlendDataCurves]] [[bpy_prop_collection]] of [[Curve]], (readonly)

filepath
    

Path to the .blend file

Type:
    

string, default “”, (readonly, never None)

fonts
    

Vector font data-blocks

Type:
    

[[BlendDataFonts]] [[bpy_prop_collection]] of [[VectorFont]], (readonly)

grease_pencils
    

Annotation data-blocks (legacy Grease Pencil)

Type:
    

[[BlendDataGreasePencils]] [[bpy_prop_collection]] of [[GreasePencil]], (readonly)

grease_pencils_v3
    

Grease Pencil data-blocks

Type:
    

[[BlendDataGreasePencilsV3]] [[bpy_prop_collection]] of [[GreasePencilv3]], (readonly)

hair_curves
    

Hair curve data-blocks

Type:
    

[[BlendDataHairCurves]] [[bpy_prop_collection]] of [[Curves]], (readonly)

images
    

Image data-blocks

Type:
    

[[BlendDataImages]] [[bpy_prop_collection]] of [[Image]], (readonly)

is_dirty
    

Have recent edits been saved to disk

Type:
    

boolean, default False, (readonly)

is_saved
    

Has the current session been saved to disk as a .blend file

Type:
    

boolean, default False, (readonly)

lattices
    

Lattice data-blocks

Type:
    

[[BlendDataLattices]] [[bpy_prop_collection]] of [[Lattice]], (readonly)

libraries
    

Library data-blocks

Type:
    

[[BlendDataLibraries]] [[bpy_prop_collection]] of [[Library]], (readonly)

lightprobes
    

Light Probe data-blocks

Type:
    

[[BlendDataProbes]] [[bpy_prop_collection]] of [[LightProbe]], (readonly)

lights
    

Light data-blocks

Type:
    

[[BlendDataLights]] [[bpy_prop_collection]] of [[Light]], (readonly)

linestyles
    

Line Style data-blocks

Type:
    

[[BlendDataLineStyles]] [[bpy_prop_collection]] of [[FreestyleLineStyle]], (readonly)

masks
    

Masks data-blocks

Type:
    

[[BlendDataMasks]] [[bpy_prop_collection]] of [[Mask]], (readonly)

materials
    

Material data-blocks

Type:
    

[[BlendDataMaterials]] [[bpy_prop_collection]] of [[Material]], (readonly)

meshes
    

Mesh data-blocks

Type:
    

[[BlendDataMeshes]] [[bpy_prop_collection]] of [[Mesh]], (readonly)

metaballs
    

Metaball data-blocks

Type:
    

[[BlendDataMetaBalls]] [[bpy_prop_collection]] of [[MetaBall]], (readonly)

movieclips
    

Movie Clip data-blocks

Type:
    

[[BlendDataMovieClips]] [[bpy_prop_collection]] of [[MovieClip]], (readonly)

node_groups
    

Node group data-blocks

Type:
    

[[BlendDataNodeTrees]] [[bpy_prop_collection]] of [[NodeTree]], (readonly)

objects
    

Object data-blocks

Type:
    

[[BlendDataObjects]] [[bpy_prop_collection]] of [[Object]], (readonly)

paint_curves
    

Paint Curves data-blocks

Type:
    

[[BlendDataPaintCurves]] [[bpy_prop_collection]] of [[PaintCurve]], (readonly)

palettes
    

Palette data-blocks

Type:
    

[[BlendDataPalettes]] [[bpy_prop_collection]] of [[Palette]], (readonly)

particles
    

Particle data-blocks

Type:
    

[[BlendDataParticles]] [[bpy_prop_collection]] of [[ParticleSettings]], (readonly)

pointclouds
    

Point cloud data-blocks

Type:
    

[[BlendDataPointClouds]] [[bpy_prop_collection]] of [[PointCloud]], (readonly)

scenes
    

Scene data-blocks

Type:
    

[[BlendDataScenes]] [[bpy_prop_collection]] of [[Scene]], (readonly)

screens
    

Screen data-blocks

Type:
    

[[BlendDataScreens]] [[bpy_prop_collection]] of [[Screen]], (readonly)

shape_keys
    

Shape Key data-blocks

Type:
    

[[bpy_prop_collection]] of [[Key]], (readonly)

sounds
    

Sound data-blocks

Type:
    

[[BlendDataSounds]] [[bpy_prop_collection]] of [[Sound]], (readonly)

speakers
    

Speaker data-blocks

Type:
    

[[BlendDataSpeakers]] [[bpy_prop_collection]] of [[Speaker]], (readonly)

texts
    

Text data-blocks

Type:
    

[[BlendDataTexts]] [[bpy_prop_collection]] of [[Text]], (readonly)

textures
    

Texture data-blocks

Type:
    

[[BlendDataTextures]] [[bpy_prop_collection]] of [[Texture]], (readonly)

use_autopack
    

Automatically pack all external data into .blend file

Type:
    

boolean, default False

version
    

File format version the .blend file was saved with

Type:
    

int array of 3 items in [0, inf], default (0, 0, 0), (readonly)

volumes
    

Volume data-blocks

Type:
    

[[BlendDataVolumes]] [[bpy_prop_collection]] of [[Volume]], (readonly)

window_managers
    

Window manager data-blocks

Type:
    

[[BlendDataWindowManagers]] [[bpy_prop_collection]] of [[WindowManager]], (readonly)

workspaces
    

Workspace data-blocks

Type:
    

[[BlendDataWorkSpaces]] [[bpy_prop_collection]] of [[WorkSpace]], (readonly)

worlds
    

World data-blocks

Type:
    

[[BlendDataWorlds]] [[bpy_prop_collection]] of [[World]], (readonly)

batch_remove(_ids_)
    

Remove (delete) several IDs at once.

Note that this function is quicker than individual calls to `remove()` (from `bpy.types.BlendData` ID collections), but less safe/versatile (it can break Blender, e.g. by removing all scenes…).

Parameters:
    

**ids** (Sequence[[[bpy.types.ID]]]) – Sequence of IDs (types can be mixed).

_classmethod _bl_rna_get_subclass(_id_ , _default =None_, _/_)
    

Parameters:
    

**id** (_str_) – The RNA type identifier.

Returns:
    

The RNA type or default when not found.

Return type:
    

[[bpy.types.Struct]] subclass

_classmethod _bl_rna_get_subclass_py(_id_ , _default =None_, _/_)
    

Parameters:
    

**id** (_str_) – The RNA type identifier.

Returns:
    

The class or default when not found.

Return type:
    

type

file_path_map(_subset =None_, _key_types =None_, _include_libraries =False_)
    

Returns a mapping of all ID data-blocks in current `bpy.data` to a set of all file paths used by them.

For list of valid set members for key_types, see: [[bpy.types.KeyingSetPath.id_type]].

Parameters:
    

  * **subset** (_sequence_) – When given, only these data-blocks and their used file paths will be included as keys/values in the map.

  * **key_types** (_set_ _of_ _strings_) – When given, filter the keys mapped by ID types. Ignored if `subset` is also given.

  * **include_libraries** (_bool_) – Include library file paths of linked data. False by default.


Returns:
    

dictionary of [[bpy.types.ID]] instances, with sets of file path strings as their values.

Return type:
    

dict

orphans_purge()
    

Remove (delete) all IDs with no user.

Parameters:
    

  * **do_local_ids** (_bool_ _,__optional_) – Include unused local IDs in the deletion, defaults to True

  * **do_linked_ids** (_bool_ _,__optional_) – Include unused linked IDs in the deletion, defaults to True

  * **do_recursive** (_bool_ _,__optional_) – Recursively check for unused IDs, ensuring no orphaned one remain after a single run of that function, defaults to False


Returns:
    

The number of deleted IDs.

temp_data(_filepath =None_)
    

A context manager that temporarily creates blender file data.

Parameters:
    

**filepath** (_str_ _|__bytes_ _|__None_) – The file path for the newly temporary data. When None, the path of the currently open file is used.

Returns:
    

Blend file data which is freed once the context exists.

Return type:
    

`bpy.types.BlendData`

user_map(_*_ , _subset =None_, _key_types =None_, _value_types =None_)
    

Returns a mapping of all ID data-blocks in current `bpy.data` to a set of all data-blocks using them.

For list of valid set members for key_types & value_types, see: [[bpy.types.KeyingSetPath.id_type]].

Parameters:
    

  * **subset** (Sequence[[[bpy.types.ID]]]) – When passed, only these data-blocks and their users will be included as keys/values in the map.

  * **key_types** (_set_ _[__str_ _]_) – Filter the keys mapped by ID types.

  * **value_types** (_set_ _[__str_ _]_) – Filter the values in the set by ID types.


Returns:
    

dictionary that maps data-blocks ID’s to their users.

Return type:
    

dict[[[bpy.types.ID]], set[[[bpy.types.ID]]]]

## Inherited Properties

  * [[bpy_struct.id_data]]

| 


  
---|---  
  
## Inherited Functions

  * [[bpy_struct.as_pointer]]
  * [[bpy_struct.driver_add]]
  * [[bpy_struct.driver_remove]]
  * [[bpy_struct.get]]
  * [[bpy_struct.id_properties_clear]]
  * [[bpy_struct.id_properties_ensure]]
  * [[bpy_struct.id_properties_ui]]
  * [[bpy_struct.is_property_hidden]]
  * [[bpy_struct.is_property_overridable_library]]
  * [[bpy_struct.is_property_readonly]]
  * [[bpy_struct.is_property_set]]
  * [[bpy_struct.items]]

| 

  * [[bpy_struct.keyframe_delete]]
  * [[bpy_struct.keyframe_insert]]
  * [[bpy_struct.keys]]
  * [[bpy_struct.path_from_id]]
  * [[bpy_struct.path_resolve]]
  * [[bpy_struct.pop]]
  * [[bpy_struct.property_overridable_library_set]]
  * [[bpy_struct.property_unset]]
  * [[bpy_struct.rna_ancestors]]
  * [[bpy_struct.type_recast]]
  * [[bpy_struct.values]]

  
---|---  
  
## References

  * [[Context.blend_data]]

| 

  * [[RenderEngine.update]]

  
---|---
