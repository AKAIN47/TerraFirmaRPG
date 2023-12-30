# TFCEvents.rockSettings

## Basic info

- Valid script types: [STARTUP]

- Has result? ✘

- Event class: RockSettingsEventJS (third-party)

```
Define new rock layers which can be referenced in a world preset json```

### Available fields:

| Name | Type | Static? |
| ---- | ---- | ------- |

Note: Even if no fields are listed above, some methods are still available as fields through *beans*.

### Available methods:

| Name | Parameters | Return type | Static? |
| ---- | ---------- | ----------- | ------- |
| defineLayer | ResourceLocation, Consumer<RockSettingsJS> |  | void | ✘ |
| defineLayer | ResourceLocation, ResourceLocation, ResourceLocation, ResourceLocation, ResourceLocation, ResourceLocation, ResourceLocation, ResourceLocation, ResourceLocation, ResourceLocation |  | RockSettings | ✘ |
| exit | Object |  | Object | ✘ |
| exit |  |  | Object | ✘ |
| success | Object |  | Object | ✘ |
| success |  |  | Object | ✘ |
| cancel | Object |  | Object | ✘ |
| cancel |  |  | Object | ✘ |


### Documented members:

- `void defineLayer(ResourceLocation id, Consumer<RockSettingsJS> settings)`

  Parameters:
  - id: ResourceLocation- The name of the rock layer
  - settings: Consumer<RockSettingsJS>- Properties defining the layer's blocks

```
Registers a new rock layer with the given properties to TFC. Does not add the layer to the world
```

- `RockSettings defineLayer(ResourceLocation id, ResourceLocation raw, ResourceLocation hardened, ResourceLocation gravel, ResourceLocation cobble, ResourceLocation sand, ResourceLocation sandstone, ResourceLocation spike, ResourceLocation loose, ResourceLocation mossyLoose)`

  Parameters:
  - id: ResourceLocation- The name of the the rock layer
  - raw: ResourceLocation- The registry name of the raw block of the rock layer
  - hardened: ResourceLocation- The registry name of the hardened block of the rock layer
  - gravel: ResourceLocation- The registry name of the gravel block of the rock layer
  - cobble: ResourceLocation- The registry name of the cobble block of the rock layer
  - sand: ResourceLocation- The registry name of the sand block of the rock layer
  - sandstone: ResourceLocation- The registry name of the sandstone block of the rock layer
  - spike: ResourceLocation- The registry name of the spike block of the rock layer, may be null to indicate no spike block
  - loose: ResourceLocation- The registry name of the loose block of the rock layer, may be null to indicate no loose block
  - mossyLoose: ResourceLocation- The registry name of the mossy loose block of the rock layer, may be null to indicate no mossy loose block

```
Registers a new rock layer with the given blocks to TFC. Does not add it to the world. This can be used to override existing layers
```

- `Object exit(Object var0)`

  Parameters:
  - var0: Object

```
Stops the event with the given exit value. Execution will be stopped **immediately**.

`exit` denotes a `default` outcome.
```

- `Object exit()`
```
Stops the event with default exit value. Execution will be stopped **immediately**.

`exit` denotes a `default` outcome.
```

- `Object success(Object var0)`

  Parameters:
  - var0: Object

```
Stops the event with the given exit value. Execution will be stopped **immediately**.

`success` denotes a `true` outcome.
```

- `Object success()`
```
Stops the event with default exit value. Execution will be stopped **immediately**.

`success` denotes a `true` outcome.
```

- `Object cancel(Object var0)`

  Parameters:
  - var0: Object

```
Cancels the event with the given exit value. Execution will be stopped **immediately**.

`cancel` denotes a `false` outcome.
```

- `Object cancel()`
```
Cancels the event with default exit value. Execution will be stopped **immediately**.

`cancel` denotes a `false` outcome.
```



### Example script:

```js
TFCEvents.rockSettings((event) => {
	// This space (un)intentionally left blank
});
```

