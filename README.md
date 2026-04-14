# deepstream-community-patches

Unified-diff patches for DeepStream **source** components. This repository ships **patches only**—not the DeepStream SDK, not NVIDIA binary or full source trees—so others can reproduce changes on top of an SDK they already obtained under NVIDIA’s terms.

Patches are grouped **by DeepStream version** first, then by component and feature.

## Legal notice

- Patches are **incremental diffs**. You must **lawfully possess** the matching DeepStream / NVIDIA sources before applying them.


## Index by DeepStream version

### DeepStream 8.0

| Component | Feature | Directory |
|-----------|---------|-----------|
| `nvdsinfer` | Smart caching / TensorRT engine naming & auto-discovery | [`patches/deepstream-8.0/nvdsinfer/smart-caching/`](patches/deepstream-8.0/nvdsinfer/smart-caching/) |
| `nvmultiurisrcbin` | Camera info via `NvDsUserMeta` (downstream) | [`patches/deepstream-8.0/nvmultiurisrcbin/camera-info-usermeta/`](patches/deepstream-8.0/nvmultiurisrcbin/camera-info-usermeta/) |
| `nvmultiurisrcbin` | Camera metadata storage (global ctypes) | [`patches/deepstream-8.0/nvmultiurisrcbin/camera-metadata-global-ctypes/`](patches/deepstream-8.0/nvmultiurisrcbin/camera-metadata-global-ctypes/) |

### DeepStream 9.0

| Component | Feature | Directory |
|-----------|---------|-----------|
| `nvdsinfer` | Smart caching / TensorRT engine naming & auto-discovery | [`patches/deepstream-9.0/nvdsinfer/smart-caching/`](patches/deepstream-9.0/nvdsinfer/smart-caching/) |

Add new work under `patches/deepstream-<major>.<minor>/<component>/<short-name>/` with a local `README.md` describing what it does and how to apply the patches.

## Layout convention

```text
patches/
  deepstream-8.0/       # or deepstream-9.0, etc.
    <component>/        # e.g. nvdsinfer, nvmultiurisrcbin
      <feature>/
        README.md
        *.patch
```

 