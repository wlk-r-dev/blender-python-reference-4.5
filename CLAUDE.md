# Blender 4.5 Python API Reference

Local copy of the Blender Python API docs for offline reference and tool development.

## What This Is

HTML documentation for `bpy` — Blender's Python API (version 4.5). Use this to look up classes, operators, properties, and types when building Blender scripts, addons, or automation tools.

## File Structure

Files are organized into subfolders by module. Root contains core entry points and indexes.

### Root Files
| File | What It Covers |
|---|---|
| `bpy.context.html` | **Context** — active object, selected objects, mode, scene |
| `bpy.data.html` | **Data access** — `bpy.data.objects`, `.meshes`, `.materials`, etc. |
| `bpy.props.html` | **Properties** — IntProperty, FloatProperty, etc. for addons |
| `bpy.path.html` | **Path utilities** — Blender-specific path helpers |
| `bpy.msgbus.html` | **Message bus** — subscribe to property changes |
| `mathutils.html` | **Math** — Vector, Matrix, Quaternion, Euler |
| `aud.html` | **Audio** — sound playback |
| `blf.html` | **Font** — text drawing in the viewport |
| `bgl.html` | **OpenGL** — direct GL calls (deprecated, prefer `gpu`) |
| `bl_math.html` | **Math helpers** — clamp, lerp, smoothstep |
| `idprop.types.html` | **ID Properties** — custom data on any datablock |
| `index.html` | Main landing page |
| `py-modindex.html` | Module index |
| `search.html` | Built-in search (browser) |

### Subfolders
| Folder | Contents | Files |
|---|---|---|
| `bpy.types/A-Z/` | **Types** — RNA types, nodes, modifiers, constraints. Split by first letter. | ~1663 |
| `bpy.types/_other/` | Base types (`bpy_struct`, `bpy_prop_collection`, `wm*`) | 6 |
| `bpy.ops/` | **Operators** — all `bpy.ops.*` modules | 78 |
| `bpy.app/` | **App info** — handlers, timers, translations, version info | 5 |
| `bpy.utils/` | **Utilities** — register/unregister, previews, script paths | 3 |
| `bpy_extras/` | **Extras** — anim, asset, io, mesh, object, view3d utils | 11 |
| `bmesh/` | **BMesh** — low-level mesh editing (verts, edges, faces, ops) | 5 |
| `mathutils/` | **Math submodules** — bvhtree, geometry, interpolate, kdtree, noise | 5 |
| `gpu/` | **GPU module** — modern shader/draw API | 9 |
| `gpu_extras/` | **GPU extras** — batch, presets | 3 |
| `freestyle/` | **Freestyle** — non-photorealistic line rendering | 8 |
| `imbuf/` | **Image buffer** — image types | 2 |
| `info/` | **Guides** — quickstart, gotchas, best practices, tips | 15 |
| `bpy_types_enum_items/` | Enum item reference pages | ~199 |
| `_static/` | CSS, JS, images for the docs | ~32 |

### Finding a Type
To find `bpy.types.Mesh`, look in `bpy.types/M/bpy.types.Mesh.html` (first letter of the type name).

### Finding an Operator
To find `bpy.ops.mesh.*`, look in `bpy.ops/bpy.ops.mesh.html`.

## How to Troubleshoot

### "AttributeError: 'X' has no attribute 'Y'"
1. Open `bpy.types.X.html` and check the actual property/method names
2. Properties may have been renamed or moved between versions

### "RuntimeError: Operator bpy.ops.X.Y.poll() failed"
1. Open `bpy.ops.X.html`, find operator `Y`
2. Check the **poll** conditions — usually requires correct mode/context
3. Common fix: ensure correct `bpy.context.area.type` or object mode

### "Context is incorrect"
1. Check `bpy.context.html` for what's available in your context
2. Operators often need specific area types — use `bpy.ops.X.Y('INVOKE_DEFAULT')` vs `('EXEC_DEFAULT')`
3. Override context with `with bpy.context.temp_override(...):`

### Finding the right operator
1. In Blender: hover over any button → status bar shows `bpy.ops.*` call
2. Or search `bpy.ops.html` for the index of all operator modules
3. Then open the specific `bpy.ops.<module>.html` for full signatures

### Finding the right type/property
1. Start at `bpy.types.Object.html` for object-level properties
2. Follow links to specific types: `Mesh.html`, `Material.html`, etc.
3. `bpy.types.bpy_struct.html` is the base class for all RNA types

## Common Workflows

### Mesh manipulation
- High-level: `bpy.ops.mesh.*` (requires edit mode)
- Low-level: `bmesh` module (create BMesh from mesh data, edit, write back)
- Read `bmesh.html` → `bmesh.types.html` → `bmesh.ops.html`

### Materials & Shaders
- `bpy.types.Material.html` → material settings
- `bpy.types.ShaderNode*.html` → all shader node types
- `bpy.types.ShaderNodeTree.html` → node tree management

### Modifiers
- `bpy.types.*Modifier.html` — one file per modifier type
- Add via `obj.modifiers.new(name, type)` — types listed in `bpy.types.Modifier.html`

### Geometry Nodes
- `bpy.types.GeometryNode*.html` — all geometry node types
- `bpy.types.GeometryNodeTree.html` — the node tree itself
- `bpy.types.NodesModifier.html` — the modifier that applies a node group

### Import/Export
- `bpy.ops.import_scene.html` / `bpy.ops.export_scene.html`
- `bpy.ops.import_anim.html` / `bpy.ops.export_anim.html`

### Handlers & Automation
- `bpy.app.handlers.html` — run code on file load, frame change, render, etc.
- `bpy.app.timers.html` — periodic callbacks
- `bpy.msgbus.html` — subscribe to property changes

## Tips

- **Always check the version** — this is 4.5. APIs change between versions.
- **RNA vs Python** — most properties are RNA (defined in C). Custom ones use `bpy.props`.
- **`bpy.types.html`** has the full alphabetical index of all types.
- **`py-modindex.html`** has the module index.
- **`searchindex.js`** + **`search.html`** — built-in search if viewed in a browser.
