# nvmultiurisrcbin: camera metadata storage (global ctypes)

Unified diffs for camera metadata handling and related `nvmultiurisrcbin` / multi-uri source changes, DeepStream **8.0** tree layout.

## Patch files

| File | Scope |
|------|--------|
| `camera-metadata-global-ctypes_deepstream-8.0.patch` | Full diff: `docs/`, `gst-plugins/gst-nvmultiurisrcbin/`, and `libs/gstnvdscustomhelper/`. |
| `camera-metadata-global-ctypes_deepstream-8.0-code-only.patch` | **`libs/`** and **`gst-plugins/`** only—no `docs/` or extra examples. |

## Apply

1. Use the official DeepStream **8.0** source tree with matching paths (`docs/`, `gst-plugins/`, `libs/gstnvdscustomhelper/`, etc.).
2. From the **root** of that tree:

```bash
patch -p1 < /path/to/deepstream-community-patches/patches/deepstream-8.0/nvmultiurisrcbin/camera-metadata-global-ctypes/camera-metadata-global-ctypes_deepstream-8.0.patch
```

Or with Git:

```bash
git apply --check /path/to/camera-metadata-global-ctypes_deepstream-8.0.patch
git apply /path/to/camera-metadata-global-ctypes_deepstream-8.0.patch
```

If your layout differs, adjust `-p0` / `-p1` or apply hunks manually.

3. Rebuild the affected components per DeepStream documentation.
