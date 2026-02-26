# Blender 4.5 Python API Reference

Local copy of the Blender Python API docs for offline reference and tool development.

## What This Is

HTML documentation for `bpy` — Blender's Python API (version 4.5). Use this to look up classes, operators, properties, and types when building Blender scripts, addons, or automation tools.

## File Structure

All files are flat HTML in this directory. No nested folders. Key naming conventions:

| Pattern | What It Covers |
|---|---|
| `bpy.ops.*.html` | **Operators** — actions you can call (mesh ops, object ops, etc.) |
| `bpy.types.*.html` | **Types** — data structures, RNA types, nodes, modifiers, constraints |
| `bpy.data.html` | **Data access** — `bpy.data.objects`, `.meshes`, `.materials`, etc. |
| `bpy.context.html` | **Context** — active object, selected objects, mode, scene |
| `bpy.props.html` | **Properties** — IntProperty, FloatProperty, etc. for addons |
| `bpy.path.html` | **Path utilities** — Blender-specific path helpers |
| `bpy.utils.html` | **Utilities** — register/unregister, previews, script paths |
| `bpy.app.*.html` | **App info** — handlers, timers, translations, version info |
| `bpy.msgbus.html` | **Message bus** — subscribe to property changes |
| `bmesh.*.html` | **BMesh** — low-level mesh editing (verts, edges, faces, operators) |
| `mathutils.*.html` | **Math** — Vector, Matrix, Quaternion, Euler, noise, geometry |
| `bgl.html` | **OpenGL** — direct GL calls (deprecated, prefer `gpu`) |
| `gpu*.html` | **GPU module** — modern shader/draw API |
| `aud.html` | **Audio** — sound playback |
| `blf.html` | **Font** — text drawing in the viewport |
| `bl_math.html` | **Math helpers** — clamp, lerp, smoothstep |
| `freestyle*.html` | **Freestyle** — non-photorealistic line rendering |
| `idprop.types.html` | **ID Properties** — custom data on any datablock |

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
