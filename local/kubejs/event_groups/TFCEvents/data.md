# TFCEvents.data

## Basic info

- Valid script types: [SERVER]

- Has result? ✘

- Event class: TFCDataEventJS (third-party)

### Available fields:

| Name | Type | Static? |
| ---- | ---- | ------- |

Note: Even if no fields are listed above, some methods are still available as fields through *beans*.

### Available methods:

| Name | Parameters | Return type | Static? |
| ---- | ---------- | ----------- | ------- |
| itemHeat | Ingredient, float, Float, Float |  | void | ✘ |
| itemHeat | Ingredient, float, Float, Float, ResourceLocation |  | void | ✘ |
| itemSize | Ingredient, Size, Weight |  | void | ✘ |
| itemSize | Ingredient, Size, Weight, ResourceLocation |  | void | ✘ |
| lampFuel | FluidIngredient, BlockIngredient, int, ResourceLocation |  | void | ✘ |
| lampFuel | FluidIngredient, BlockIngredient, int |  | void | ✘ |
| sluicing | Ingredient, String |  | void | ✘ |
| sluicing | Ingredient, String, ResourceLocation |  | void | ✘ |
| panning | BlockIngredient, String, List<String>, ResourceLocation |  | void | ✘ |
| panning | BlockIngredient, String, List<String> |  | void | ✘ |
| metal | String, float, float, Ingredient, Ingredient, Ingredient, int |  | void | ✘ |
| metal | String, float, float, Ingredient, Ingredient, Ingredient, int, ResourceLocation |  | void | ✘ |
| support | BlockIngredient, int, int, int |  | void | ✘ |
| support | BlockIngredient, int, int, int, ResourceLocation |  | void | ✘ |
| climateRange | Consumer<BuildClimateRangeData>, ResourceLocation |  | void | ✘ |
| fertilizer | Ingredient, Number, Number, Number |  | void | ✘ |
| fertilizer | Ingredient, Number, Number, Number, ResourceLocation |  | void | ✘ |
| fuel | Ingredient, float, int, Float |  | void | ✘ |
| fuel | Ingredient, float, int, Float, ResourceLocation |  | void | ✘ |
| foodItem | Ingredient, Consumer<BuildFoodItemData> |  | void | ✘ |
| foodItem | Ingredient, Consumer<BuildFoodItemData>, ResourceLocation |  | void | ✘ |
| fauna | Consumer<Climate>, Consumer<BuildFaunaData>, ResourceLocation |  | void | ✘ |
| drinkable | FluidIngredient, Consumer<BuildDrinkableData>, ResourceLocation |  | void | ✘ |
| drinkable | FluidIngredient, Consumer<BuildDrinkableData> |  | void | ✘ |
| knappingType | Ingredient, int, int, ResourceLocation, boolean, boolean, boolean, ItemStack, ResourceLocation |  | void | ✘ |
| entityDamageResistance | String, Integer, Integer, Integer, ResourceLocation |  | void | ✘ |
| entityDamageResistance | String, Integer, Integer, Integer |  | void | ✘ |
| itemDamageResistance | Ingredient, Integer, Integer, Integer, ResourceLocation |  | void | ✘ |
| itemDamageResistance | Ingredient, Integer, Integer, Integer |  | void | ✘ |
| exit | Object |  | Object | ✘ |
| exit |  |  | Object | ✘ |
| success | Object |  | Object | ✘ |
| success |  |  | Object | ✘ |
| cancel | Object |  | Object | ✘ |
| cancel |  |  | Object | ✘ |


### Documented members:

- `void itemHeat(Ingredient ingredient, float heatCapacity, Float forgingTemperature, Float weldingTemperature)`

  Parameters:
  - ingredient: Ingredient- The ingredient the heat definition applies to
  - heatCapacity: float- Specifies how fast the ingredient heats up relative to others. Measured in Energy / °C
  - forgingTemperature: Float- Specifies the temperature °C required to work the ingredient. May be null to allow working at any temperature
  - weldingTemperature: Float- Specifies the temperature °C required to weld the ingredient. May be null to allow welding at any temperature

```
Adds a heat definition to the specified ingredient
```

- `void itemHeat(Ingredient ingredient, float heatCapacity, Float forgingTemperature, Float weldingTemperature, ResourceLocation name)`

  Parameters:
  - ingredient: Ingredient- The ingredient the heat definition applies to
  - heatCapacity: float- Specifies how fast the ingredient heats up relative to others. Measured in Energy / °C
  - forgingTemperature: Float- Specifies the temperature °C required to work the ingredient. May be null to allow working at any temperature
  - weldingTemperature: Float- Specifies the temperature °C required to weld the ingredient. May be null to allow welding at any temperature
  - name: ResourceLocation- The name of the heat definition

```
Adds a heat definition to the specified ingredient
```

- `void itemSize(Ingredient ingredient, Size size, Weight weight)`

  Parameters:
  - ingredient: Ingredient- The ingredient this item size definition applies to
  - size: Size- Sets the size of the definition, may be 'tiny', 'very_small', 'small', 'normal', 'large', 'very_large', 'huge', or null to not specify a size
  - weight: Weight- Sets the weight of the definition, may be 'very_light', 'light', 'medium', 'heavy', 'very_heavy', or null to not specify a weight

```
Adds an item size definition tot he specified ingredient
```

- `void itemSize(Ingredient ingredient, Size size, Weight weight, ResourceLocation name)`

  Parameters:
  - ingredient: Ingredient- The ingredient this item size definition applies to
  - size: Size- Sets the size of the definition, may be 'tiny', 'very_small', 'small', 'normal', 'large', 'very_large', 'huge', or null to default to 'medium'
  - weight: Weight- Sets the weight of the definition, may be 'very_light', 'light', 'medium', 'heavy', 'very_heavy', or null to default to 'medium'
  - name: ResourceLocation- The name of the item size definition

```
Adds an item size definition to the specified ingredient
```

- `void lampFuel(FluidIngredient fluidIngredient, BlockIngredient blockIngredient, int burnRate, ResourceLocation name)`

  Parameters:
  - fluidIngredient: FluidIngredient- The fluid ingredient which determines which fluids the the lamp fuel applies to
  - blockIngredient: BlockIngredient- The block ingredient which determines what (lamp) blocks are valid for this fuel
  - burnRate: int- How fast the lamp consumes fuel, in ticks per mB
  - name: ResourceLocation- The name of the lamp fuel

```
Defines a lamp fuel
```

- `void lampFuel(FluidIngredient fluidIngredient, BlockIngredient blockIngredient, int burnRate)`

  Parameters:
  - fluidIngredient: FluidIngredient- The fluid ingredient which determines which fluids the the lamp fuel applies to
  - blockIngredient: BlockIngredient- The block ingredient which determines what (lamp) blocks are valid for this fuel
  - burnRate: int- How fast the lamp consumes fuel, in ticks per mB

```
Defines a lamp fuel
```

- `void sluicing(Ingredient ingredient, String lootTable)`

  Parameters:
  - ingredient: Ingredient- The ingredient the sluicing definition applies to
  - lootTable: String- The location of a loot table to be dropped for this item

```
Adds a sluicing definition to the ingredient
```

- `void sluicing(Ingredient ingredient, String lootTable, ResourceLocation name)`

  Parameters:
  - ingredient: Ingredient- The ingredient the sluicing definition applies to
  - lootTable: String- The location of a loot table to be dropped for this item
  - name: ResourceLocation- The name of the sluicing definition

```
Adds a sluicing definition to the ingredient
```

- `void panning(BlockIngredient blockIngredient, String lootTable, List<String> models, ResourceLocation name)`

  Parameters:
  - blockIngredient: BlockIngredient- The block ingredient the definition applies to
  - lootTable: String- The location of a loot table to be dropped by the ingredient
  - models: List<String>- A list of model locations to be iterated through as panning progresses
  - name: ResourceLocation- The name of the panning definition

```
Adds a panning definition to the block ingredient
```

- `void panning(BlockIngredient blockIngredient, String lootTable, List<String> models)`

  Parameters:
  - blockIngredient: BlockIngredient- The block ingredient the definition applies to
  - lootTable: String- The location of a loot table to be dropped by the ingredient
  - models: List<String>- A list of model locations to be iterated through as panning progresses

```
Adds a panning definition to the block ingredient
```

- `void metal(String fluid, float meltTemperature, float heatCapacity, Ingredient ingot, Ingredient doubleIngot, Ingredient sheet, int tier)`

  Parameters:
  - fluid: String- The registry name of the fluid which corresponds to the metal
  - meltTemperature: float- The melting temperature °C of the metal
  - heatCapacity: float- Specifies how fast the metal heats up relative to others. Measured in Energy / (mB x °C)
  - ingot: Ingredient- The ingredient which specifies the metal's ingots, may be null
  - doubleIngot: Ingredient- The ingredient which specifies the metal's double ingots, may be null
  - sheet: Ingredient- The ingredient which specifies the metal's sheets, may be null
  - tier: int- The tier of the metal

```
Defines a metal
```

- `void metal(String fluid, float meltTemperature, float heatCapacity, Ingredient ingot, Ingredient doubleIngot, Ingredient sheet, int tier, ResourceLocation name)`

  Parameters:
  - fluid: String- The registry name of the fluid which corresponds to the metal
  - meltTemperature: float- The melting temperature °C of the metal
  - heatCapacity: float- Specifies how fast the metal heats up relative to others. Measured in Energy / (mB x °C)
  - ingot: Ingredient- The ingredient which specifies the metal's ingots, may be null
  - doubleIngot: Ingredient- The ingredient which specifies the metal's double ingots, may be null
  - sheet: Ingredient- The ingredient which specifies the metal's sheets, may be null
  - tier: int- The tier of the metal
  - name: ResourceLocation- The name of the metal

```
Defines a metal
```

- `void support(BlockIngredient blockIngredient, int up, int down, int horizontal)`

  Parameters:
  - blockIngredient: BlockIngredient- The block ingredient that defines what blocks the definition applies to
  - up: int- The number of blocks upwards the block supports
  - down: int- The number og blocks downwards the block supports
  - horizontal: int- The number of blocks horizontally the block supports

```
Defines a support definition
```

- `void support(BlockIngredient blockIngredient, int up, int down, int horizontal, ResourceLocation name)`

  Parameters:
  - blockIngredient: BlockIngredient- The block ingredient that defines what blocks the definition applies to
  - up: int- The number of blocks upwards the block supports
  - down: int- The number og blocks downwards the block supports
  - horizontal: int- The number of blocks horizontally the block supports
  - name: ResourceLocation- The name of the support definition

```
Defines a support definition
```

- `void climateRange(Consumer<BuildClimateRangeData> climateRange, ResourceLocation name)`

  Parameters:
  - climateRange: Consumer<BuildClimateRangeData>- Climate range properties for the given climate range
  - name: ResourceLocation- The name of the climate range

```
Specifies the climate range data of the given name
```

- `void fertilizer(Ingredient ingredient, Number nitrogen, Number phosphorous, Number potassium)`

  Parameters:
  - ingredient: Ingredient- The ingredient the fertilizer data applies to
  - nitrogen: Number- The nitrogen value of the fertilizer, may be null to not define a value, defaults to 0
  - phosphorous: Number- The phosphorous value of the fertilizer, may be null to not define a value, defaults to 0
  - potassium: Number- The potassium value of the fertilizer, amy be null to not define a value, defaults to 0

```
Adds a fertilizer definition to the specified ingredient
```

- `void fertilizer(Ingredient ingredient, Number nitrogen, Number phosphorous, Number potassium, ResourceLocation name)`

  Parameters:
  - ingredient: Ingredient- The ingredient the fertilizer data applies to
  - nitrogen: Number- The nitrogen value of the fertilizer, may be null to not define a value, defaults to 0
  - phosphorous: Number- The phosphorous value of the fertilizer, may be null to not define a value, defaults to 0
  - potassium: Number- The potassium value of the fertilizer, amy be null to not define a value, defaults to 0
  - name: ResourceLocation- The name of the fertilizer data

```
Adds a fertilizer definition to the specified ingredient
```

- `void fuel(Ingredient ingredient, float temperature, int duration, Float purity)`

  Parameters:
  - ingredient: Ingredient- The ingredient the fuel definition applies to
  - temperature: float- The temperature °C that the fuel burns at
  - duration: int- The number of ticks the fuel burns for
  - purity: Float- The purity of the fuel, may be null to not specify a value

```
Adds a fuel definition to the specified ingredient
```

- `void fuel(Ingredient ingredient, float temperature, int duration, Float purity, ResourceLocation name)`

  Parameters:
  - ingredient: Ingredient- The ingredient the fuel definition applies to
  - temperature: float- The temperature °C that the fuel burns at
  - duration: int- The number of ticks the fuel burns for
  - purity: Float- The purity of the fuel, may be null to not specify a value
  - name: ResourceLocation- The name of the fuel definition

```
Adds a fuel definition to the specified ingredient
```

- `void foodItem(Ingredient ingredient, Consumer<BuildFoodItemData> foodItemData)`

  Parameters:
  - ingredient: Ingredient- The ingredient the food definition applies to
  - foodItemData: Consumer<BuildFoodItemData>- The food item properties that are applied to the ingredient

```
Adds a food definition to the specified ingredient
```

- `void foodItem(Ingredient ingredient, Consumer<BuildFoodItemData> foodItemData, ResourceLocation name)`

  Parameters:
  - ingredient: Ingredient- The ingredient the food definition applies to
  - foodItemData: Consumer<BuildFoodItemData>- The food item properties that are applied to the ingredient
  - name: ResourceLocation- The name of the food item data

```
Adds a food definition to the specified ingredient
```

- `void fauna(Consumer<Climate> climate, Consumer<BuildFaunaData> fauna, ResourceLocation name)`

  Parameters:
  - climate: Consumer<Climate>- The fauna's climate requirements
  - fauna: Consumer<BuildFaunaData>- Additional fauna properties for the given fauna
  - name: ResourceLocation- The name of the fauna definition

```
Specifies the fauna data of the given name
```

- `void drinkable(FluidIngredient fluidIngredient, Consumer<BuildDrinkableData> drinkableData, ResourceLocation name)`

  Parameters:
  - fluidIngredient: FluidIngredient- The fluids this drinkable applies to
  - drinkableData: Consumer<BuildDrinkableData>- The drinkable properties that are applied to the fluid ingredient
  - name: ResourceLocation- The name of the drinkable data

```
Defines that a fluid is directly drinkable
```

- `void drinkable(FluidIngredient fluidIngredient, Consumer<BuildDrinkableData> drinkableData)`

  Parameters:
  - fluidIngredient: FluidIngredient- The fluids this drinkable applies to
  - drinkableData: Consumer<BuildDrinkableData>- The drinkable properties that are applied to the fluid ingredient

```
Defines that a fluid is directly drinkable
```

- `void knappingType(Ingredient ingredient, int ingredientCount, int amountToConsume, ResourceLocation clickSound, boolean consumeAfterComplete, boolean useDisabledTexture, boolean spawnsParticles, ItemStack jeiIconItem, ResourceLocation name)`

  Parameters:
  - ingredient: Ingredient- The ingredient of the knapping type's item stack ingredient
  - ingredientCount: int- The count of the knapping type's item stack ingredient
  - amountToConsume: int- The amount of items that get used by the recipe
  - clickSound: ResourceLocation- The registry name of a sound that plays when knapping occurs
  - consumeAfterComplete: boolean- If items should be consumed as soon as a square is clicked, or when the result is removed from the slot
  - useDisabledTexture: boolean- If true, a clicked slot will show a different texture rather than nothing at all
  - spawnsParticles: boolean- if true, the screen will show particles when knapping
  - jeiIconItem: ItemStack- An item stack, used as the category icon in the auto-generated jei category
  - name: ResourceLocation- The name of the knapping type

```
Defines a knapping type
```

- `void entityDamageResistance(String entityTag, Integer piercing, Integer slashing, Integer crushing, ResourceLocation name)`

  Parameters:
  - entityTag: String- The entity tag to apply the damage resistances to
  - piercing: Integer- The piercing value of this resistance, may be null to not specify a value
  - slashing: Integer- The slashing value of this resistance, may be null to not specify a value
  - crushing: Integer- the crushing value of this resistance, may be null to not specify a value
  - name: ResourceLocation- The name of the damage resistance

```
Adds an entity damage resistance to the specified entity tag
```

- `void entityDamageResistance(String entityTag, Integer piercing, Integer slashing, Integer crushing)`

  Parameters:
  - entityTag: String- The entity tag to apply the damage resistances to
  - piercing: Integer- The piercing value of this resistance, may be null to not specify a value
  - slashing: Integer- The slashing value of this resistance, may be null to not specify a value
  - crushing: Integer- the crushing value of this resistance, may be null to not specify a value

```
Adds an entity damage resistance to the specified entity tag
```

- `void itemDamageResistance(Ingredient ingredient, Integer piercing, Integer slashing, Integer crushing, ResourceLocation name)`

  Parameters:
  - ingredient: Ingredient- The ingredient this resistance applies to
  - piercing: Integer- The piercing value of this resistance, may be null to not specify a value
  - slashing: Integer- The slashing value of this resistance, may be null to not specify a value
  - crushing: Integer- the crushing value of this resistance, may be null to not specify a value
  - name: ResourceLocation- The name of the damage resistance

```
Adds an item damage resistance to the specified ingredient
```

- `void itemDamageResistance(Ingredient ingredient, Integer piercing, Integer slashing, Integer crushing)`

  Parameters:
  - ingredient: Ingredient- The ingredient this resistance applies to
  - piercing: Integer- The piercing value of this resistance, may be null to not specify a value
  - slashing: Integer- The slashing value of this resistance, may be null to not specify a value
  - crushing: Integer- the crushing value of this resistance, may be null to not specify a value

```
Adds an item damage resistance to the specified ingredient
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
TFCEvents.data((event) => {
	// This space (un)intentionally left blank
});
```

