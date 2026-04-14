# nvmultiurisrcbin: camera info via `NvDsUserMeta` (downstream)

Unified diffs for attaching camera metadata through `NvDsUserMeta` in the `nvmultiurisrcbin` path (`gstnvdscustomhelper`), DeepStream **8.0** tree layout.

## Patch files

| File | Scope |
|------|--------|
| `camera-info-usermeta_deepstream-8.0.patch` | Full diff: root `README.md` plus `libs/gstnvdscustomhelper/` (implementation doc + `gst-nvmultiurisrcbincreator.cpp`). |
| `camera-info-usermeta_deepstream-8.0-libs-only.patch` | **`libs/` only**—no top-level `README.md` change. |

## Apply

1. Use the official DeepStream **8.0** source tree with the same relative paths (`libs/gstnvdscustomhelper/...`).
2. From the **root** of that tree:

```bash
patch -p1 < /path/to/deepstream-community-patches/patches/deepstream-8.0/nvmultiurisrcbin/camera-info-usermeta/camera-info-usermeta_deepstream-8.0.patch
```

Or with Git:

```bash
git apply --check /path/to/camera-info-usermeta_deepstream-8.0.patch
git apply /path/to/camera-info-usermeta_deepstream-8.0.patch
```

If your layout differs, adjust `-p0` / `-p1` or apply hunks manually.

3. Rebuild the affected components per DeepStream documentation.
