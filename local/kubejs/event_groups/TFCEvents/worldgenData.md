# TFCEvents.worldgenData

## Basic info

- Valid script types: [SERVER]

- Has result? ✘

- Event class: TFCWorldgenDataEventJS (third-party)

### Available fields:

| Name | Type | Static? |
| ---- | ---- | ------- |

Note: Even if no fields are listed above, some methods are still available as fields through *beans*.

### Available methods:

| Name | Parameters | Return type | Static? |
| ---- | ---------- | ----------- | ------- |
| thinSpike | String, String, int, int, int, int, Consumer<PlacedFeatureProperties> |  | void | ✘ |
| babyBoulder | String, List<BoulderState>, Consumer<PlacedFeatureProperties> |  | void | ✘ |
| pipeVein | String, List<VeinReplacementMapEntry>, int, float, int, int, int, int, int, int, int, int, float, Consumer<Pipe>, Consumer<PlacedFeatureProperties> |  | void | ✘ |
| veinReplacement | List<String>, List<String> |  | VeinReplacementMapEntry | ✘ |
| boulderState | String, List<String> |  | BoulderState | ✘ |
| discVein | String, List<VeinReplacementMapEntry>, int, float, int, int, int, int, Consumer<Disc>, Consumer<PlacedFeatureProperties> |  | void | ✘ |
| clusterVein | String, List<VeinReplacementMapEntry>, int, float, int, int, int, Consumer<Cluster>, Consumer<PlacedFeatureProperties> |  | void | ✘ |
| boulder | String, List<BoulderState>, Consumer<PlacedFeatureProperties> |  | void | ✘ |
| geode | String, String, String, List<String>, Consumer<PlacedFeatureProperties> |  | void | ✘ |
| ifThen | String, String, String, Consumer<PlacedFeatureProperties> |  | void | ✘ |
| exit | Object |  | Object | ✘ |
| exit |  |  | Object | ✘ |
| success | Object |  | Object | ✘ |
| success |  |  | Object | ✘ |
| cancel | Object |  | Object | ✘ |
| cancel |  |  | Object | ✘ |


### Documented members:

- `void thinSpike(String name, String state, int radius, int tries, int minHeight, int maxHeight, Consumer<PlacedFeatureProperties> placement)`

  Parameters:
  - name: String- The name of the feature, the namespace will default to 'kubejs_tfc' if none is provided
  - state: String- Sets the 'state' property of the modifier
  - radius: int- Sets the 'radius' property of the modifier
  - tries: int- Sets the 'tries' property of the modifier
  - minHeight: int- Sets the 'min_height' property of the modifier
  - maxHeight: int- Sets the 'max_height' property of the modifier
  - placement: Consumer<PlacedFeatureProperties>- The placement properties

```
Creates a thin spike configured feature and the matching placed feature
```

- `void babyBoulder(String name, List<BoulderState> states, Consumer<PlacedFeatureProperties> placement)`

  Parameters:
  - name: String- The name of the feature, the namespace will default to 'kubejs_tfc' if none is provided
  - states: List<BoulderState>- A list of {Block -> BlockState[]} objects in string form that define the baby boulder's state property
  - placement: Consumer<PlacedFeatureProperties>- The placement properties

```
Creates a baby boulder configured feature and the matching placed feature
```

- `void pipeVein(String name, List<VeinReplacementMapEntry> replacementMap, int rarity, float density, int minY, int maxY, int height, int radius, int minSkew, int maxSkew, int minSlant, int maxSlant, float sign, Consumer<Pipe> optionals, Consumer<PlacedFeatureProperties> placement)`

  Parameters:
  - name: String- The name of the feature, the namespace will default to 'kubejs_tfc' if none is provided
  - replacementMap: List<VeinReplacementMapEntry>- A list of {Block[] -> WeightedBlockState[]} objects in string form that define the vein's replacement map
  - rarity: int- Sets the 'rarity' value of the vein
  - density: float- Sets the 'density' value of the vein
  - minY: int- Sets the 'min_y' value of the vein
  - maxY: int- Sets the 'max_y' value of the vein
  - height: int- Sets the 'height' value of the vein
  - radius: int- Sets the 'radius' value of the vein
  - minSkew: int- Sets the 'min_skew' value of the vein
  - maxSkew: int- Sets the 'max_skew' value of the vein
  - minSlant: int- Sets the 'min_slant' value of the vein
  - maxSlant: int- Sets the 'max_slant' value of the vein
  - sign: float- Sets the 'sign' value of the vein
  - optionals: Consumer<Pipe>- Sets the optional values of the vein through a consumer
  - placement: Consumer<PlacedFeatureProperties>- The placement properties

```
Creates a 'tfc:pipe_vein' configured feature and the matching placed feature
```

- `VeinReplacementMapEntry veinReplacement(List<String> blocks, List<String> blockStates)`

  Parameters:
  - blocks: List<String>- A list of strings, the registry names of blocks to be replaced
  - blockStates: List<String>- A list of string representations of a weighted block state

```
Creates a new block list to weighted block state list map entry for use in vein configured features
```

- `BoulderState boulderState(String block, List<String> blockStates)`

  Parameters:
  - block: String- The registry name of a block to be replaced
  - blockStates: List<String>- A list of string representations of a block state

```
Creates a new block to block state list map entry for use in boulder configured features
```

- `void discVein(String name, List<VeinReplacementMapEntry> replacementMap, int rarity, float density, int minY, int maxY, int size, int height, Consumer<Disc> optionals, Consumer<PlacedFeatureProperties> placement)`

  Parameters:
  - name: String- The name of the feature, the namespace will default to 'kubejs_tfc' if none is provided
  - replacementMap: List<VeinReplacementMapEntry>- A list of {Block[] -> WeightedBlockState[]} objects in string form that define the vein's replacement map
  - rarity: int- Sets the 'rarity' value of the vein
  - density: float- Sets the 'density' value of the vein
  - minY: int- Sets the 'min_y' value of the vein
  - maxY: int- Sets the 'max_y' value of the vein
  - size: int- Sets the 'size' value of the vein
  - height: int- Sets the 'height' value of the vein
  - optionals: Consumer<Disc>- Sets the optional values of the vein through a consumer
  - placement: Consumer<PlacedFeatureProperties>- The placement properties

```
Creates a 'tfc:cluster_vein' configured feature and the matching placed feature
```

- `void clusterVein(String name, List<VeinReplacementMapEntry> replacementMap, int rarity, float density, int minY, int maxY, int size, Consumer<Cluster> optionals, Consumer<PlacedFeatureProperties> placement)`

  Parameters:
  - name: String- The name of the feature, the namespace will default to 'kubejs_tfc' if none is provided
  - replacementMap: List<VeinReplacementMapEntry>- A list of {Block[] -> WeightedBlockState[]} objects in string form that define the vein's replacement map
  - rarity: int- Sets the 'rarity' value of the vein
  - density: float- Sets the 'density' value of the vein
  - minY: int- Sets the 'min_y' value of the vein
  - maxY: int- Sets the 'max_y' value of the vein
  - size: int- Sets the 'size' value of the vein
  - optionals: Consumer<Cluster>- Sets the optional values of the vein through a consumer
  - placement: Consumer<PlacedFeatureProperties>- The placement properties

```
Creates a 'tfc:cluster_vein' configured feature and the matching placed feature
```

- `void boulder(String name, List<BoulderState> states, Consumer<PlacedFeatureProperties> placement)`

  Parameters:
  - name: String- The name of the feature, the namespace will default to 'kubejs_tfc' if none is provided
  - states: List<BoulderState>- A list of {Block -> BlockState[]} objects in string form that define the boulder's state property
  - placement: Consumer<PlacedFeatureProperties>- The placement properties

```
Creates a boulder configured feature and the matching placed feature
```

- `void geode(String name, String outer, String middle, List<String> innerValues, Consumer<PlacedFeatureProperties> placement)`

  Parameters:
  - name: String- The name of the feature, the namespace will default to 'kubejs_tfc' if none is provided
  - outer: String- Sets the outer block state of the geode
  - middle: String- Sets the middle block state of the geode
  - innerValues: List<String>- A list of weight block state in string form, sets the inner state of the geode
  - placement: Consumer<PlacedFeatureProperties>- The placement properties

```
Creates a geode configured feature and the matching placed feature
```

- `void ifThen(String name, String if_, String then, Consumer<PlacedFeatureProperties> placement)`

  Parameters:
  - name: String- The name of the feature, the namespace will default to 'kubejs_tfc' if none is provided
  - if_: String- A placed feature id, that will always try to place
  - then: String- A placed feature id, that will only place if the first feature is placed
  - placement: Consumer<PlacedFeatureProperties>- The placement properties

```
Creates a 'tfc:if_then' configured feature and the matching placed feature
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
TFCEvents.worldgenData((event) => {
	// This space (un)intentionally left blank
});
```

