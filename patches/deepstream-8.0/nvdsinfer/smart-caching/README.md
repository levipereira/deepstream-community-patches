# nvdsinfer: smart caching (TensorRT engine naming / auto-discovery) — DeepStream 8.0

Unified diffs for `libs/nvdsinfer` on **DeepStream 8.0** (and compatible 8.x layouts).

## Patch files

| File | Scope |
|------|--------|
| `nvdsinfer-smart-caching_deepstream-8.x.patch` | Full tree (top-level `README.md` + `libs/nvdsinfer/`). |
| `nvdsinfer-smart-caching_deepstream-8.x-libs-nvdsinfer-only.patch` | **`libs/nvdsinfer/` only** (minimal). |

## Apply

1. Use the official **DeepStream 8.0** source tree; paths must match the patch (`libs/nvdsinfer/...`).
2. From the **root** of that tree:

```bash
patch -p1 < /path/to/deepstream-community-patches/patches/deepstream-8.0/nvdsinfer/smart-caching/nvdsinfer-smart-caching_deepstream-8.x-libs-nvdsinfer-only.patch
```

Or with Git:

```bash
git apply --check /path/to/nvdsinfer-smart-caching_deepstream-8.x-libs-nvdsinfer-only.patch
git apply /path/to/nvdsinfer-smart-caching_deepstream-8.x-libs-nvdsinfer-only.patch
```

If your layout differs, adjust `-p0` / `-p1` or apply hunks manually.

3. Rebuild `nvdsinfer` per DeepStream documentation.

**DeepStream 9.0:** use [`patches/deepstream-9.0/nvdsinfer/smart-caching/`](../../../deepstream-9.0/nvdsinfer/smart-caching/).
