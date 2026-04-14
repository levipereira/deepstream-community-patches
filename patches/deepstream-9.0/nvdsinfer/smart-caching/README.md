# nvdsinfer: smart caching (TensorRT engine naming / auto-discovery) — DeepStream 9.0

Unified diff for `libs/nvdsinfer` on **DeepStream 9.0**.

## Patch file

| File | Scope |
|------|--------|
| `nvdsinfer-smart-caching_deepstream-9.0.patch` | `libs/nvdsinfer/` only. |

## Apply

1. Use the official **DeepStream 9.0** source tree; paths must match the patch (`libs/nvdsinfer/...`).
2. From the **root** of that tree:

```bash
patch -p1 < /path/to/deepstream-community-patches/patches/deepstream-9.0/nvdsinfer/smart-caching/nvdsinfer-smart-caching_deepstream-9.0.patch
```

Or with Git:

```bash
git apply --check /path/to/nvdsinfer-smart-caching_deepstream-9.0.patch
git apply /path/to/nvdsinfer-smart-caching_deepstream-9.0.patch
```

If your layout differs, adjust `-p0` / `-p1` or apply hunks manually.

3. Rebuild `nvdsinfer` per DeepStream documentation.

**DeepStream 8.0:** use [`patches/deepstream-8.0/nvdsinfer/smart-caching/`](../../../deepstream-8.0/nvdsinfer/smart-caching/).
