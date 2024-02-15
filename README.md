# Roblox Optimization (and visual) FFlags v7.3 ![](https://pixels.crd.co/assets/images/gallery13/4bae341f.gif)

## Potato Flags

Forces Direct3D11 (better performance on newer pcs)

```json
{
  "FFlagDebugGraphicsDisableDirect3D11": false,
  "FFlagDebugGraphicsPreferD3D11": true,
  "FFlagDebugGraphicsPreferD3D11FL10": false
}
```

Forces Direct3D10 (better performance on older PCs)

```json
{
  "FFlagDebugGraphicsDisableDirect3D11": false,
  "FFlagDebugGraphicsPreferD3D11": false,
  "FFlagDebugGraphicsPreferD3D11FL10": true,
  "FFlagGraphicsEnableD3D10Compute": true
}
```

Forces Vulkan (can crash)

```json
{
  "FFlagDebugGraphicsDisableVulkan": false,
  "FFlagDebugGraphicsDisableVulkan11": false,
  "FFlagDebugGraphicsPreferVulkan": true,
  "FFlagRenderVulkanFixMinimizeWindow": true
}
```

Forces Metal (only for macOS (?) and should give perf boost?? idk)

```json
{
  "FFlagDebugGraphicsPreferMetal": true
}
```

Forces Voxel lightning

```json
{
  "DFFlagDebugRenderForceTechnologyVoxel": true
}
```

Disables terrain grass (?)

```json
{
  "FIntFRMMinGrassDistance": 0,
  "FIntFRMMaxGrassDistance": 0,
  "FIntRenderGrassDetailStrands": 0,
  "FintRenderGrassHeightScaler": 0
}
```

Breaks Voxel shadows (only works w/ voxel lightning)

```json
{
  "DFFlagDebugPauseVoxelizer": true
}
```

Makes Roblox at high res. lower quality

```json
{
  "DFFlagDisableDPIScale": false
}
```

Disables textures (doesn't give perf boost, only visual)

```json
{
  "FStringPartTexturePackTablePre2022": "{\"glass\":{\"ids\":[\"rbxassetid://7547304948\",\"rbxassetid://7546645118\"],\"color\":[254,254,254,7]}}",
  "FStringPartTexturePackTable2022": "{\"glass\":{\"ids\":[\"rbxassetid://7547304948\",\"rbxassetid://7546645118\"],\"color\":[254,254,254,7]}}",
  "FStringTerrainMaterialTablePre2022": "",
  "FStringTerrainMaterialTable2022": ""
}
```

Disables textures and breaks glass (alternative for one above)

```json
{
  "FStringPartTexturePackTablePre2022": "",
  "FStringPartTexturePackTable2022": "",
  "FStringTerrainMaterialTablePre2022": "",
  "FStringTerrainMaterialTable2022": ""
}
```

Disables player shadows

```json
{
  "FIntRenderShadowIntensity": 0
}
```

Disables some effects (like sunrays)

```json
{
  "FFlagDisablePostFx": true
}
```

Disables antialiasing

```json
{
  "FIntDebugForceMSAASamples": 0
}
```

Makes textures low quality

```json
{
  "DFFlagTextureQualityOverrideEnabled": true,
  "DFIntTextureQualityOverride": 0
}
```

Lowers model polygons from far

```json
{
  "DFIntCSGLevelOfDetailSwitchingDistance": 0,
  "DFIntCSGLevelOfDetailSwitchingDistanceL12": 0,
  "DFIntCSGLevelOfDetailSwitchingDistanceL23": 0,
  "DFIntCSGLevelOfDetailSwitchingDistanceL34": 0
}
```

Limits light updates

```json
{
  "FIntRenderLocalLightUpdatesMax": 1,
  "FIntRenderLocalLightUpdatesMin": 1
}
```

Enables gray sky w/ no clouds

```json
{
  "FFlagDebugSkyGray": true
}
```

Disables Selfview

```json
{
  "FFlagCoreGuiTypeSelfViewPresent": false
}
```

Forces graphics quality to 1 (while being able to change render distance!)

```json
{
  "DFIntDebugFRMQualityLevelOverride": 1
}
```

Enable Hyperthreading

```json
{
 "FFlagRenderCheckThreading": "True"
}
```

Removes most textures of other players
```json
{
  "DFIntTextureCompositorActiveJobs": 0
}
```

## How to add FFlags to this list

Please do not open an issue, instead make a pull request and add the FFlag to the correct section, with the correct format and below the latest FFlag
```json
{
  "Flag1": "Value",
  "Flag2" : 23
}
```
