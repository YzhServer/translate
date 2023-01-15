Space has a custom resource pack which does not need to be installed, as the plugin can automatically enable it if the user follows the steps below:

1. Leave the server, click "Edit Server", and enable "Server Resource Packs".

![Image unavailable](https://i.imgur.com/Gknsa51.png)

2. Join the server and type `/space`.

![Image unavailable](https://i.imgur.com/FFENcaG.png)

3. Click the "Resource Pack" icon.

![Image unavailable](https://i.imgur.com/BF8ibLE.png)

4. The resource pack is now enabled!

![Image unavailable](https://i.imgur.com/yJdysMA.png)

# Other notes (For server owners wanting to use their own resource packs)

Servers can change the resource pack link located in `config.yml` to their own custom resource packs, so not all Space servers will look the same. If you're planning on doing this, use the Space resource pack as a reference by using the CustomModelData tags in the `models` folder. The CustomModelData tags are configurable, but the default is `1234567`. Other models using the same item will add an amount to the tag (E.G. `1234568`).

## Merging Resource Packs

If multiple resource packs are conflicting with each other, the packs must be merged:

1. Make a new pack for the merged pack.
2. Copy one of the `pack.mcmeta` files from either pack, or create a new one. It is recommended to differentiate the `pack.mcmeta` from the original packs' to avoid confusion.
3. Open the `assets\minecraft` directory in both packs and search through each directory.
4. If any files are shared in both packs (E.G., both packs have `assets\minecraft\models\item\arrow.json`), open both versions and combine the content from both files. Typically, for models, this will involve adding entries to the `overrides` tag. Place all entries from both files into the combined file, and ensure that the predicates' numeric values are in ascending order. Note that all overrides must be separated by commas.

<details>
    <summary>Example</summary>

File 1

```json
{
    "parent": "minecraft:item/generated",
    "textures": {
        "layer0": "minecraft:item/arrow"
    },
    "overrides": [
        {"predicate": {"custom_model_data": 1}, "model": "foo:item/example"}
    ]
}
```

File 2

```json
{
    "parent": "minecraft:item/generated",
    "textures": {
        "layer0": "minecraft:item/arrow"
    },
    "overrides": [
        {"predicate": {"custom_model_data": 2}, "model": "something:folder/etc"}
    ]
}
```

Combined

```json
{
    "parent": "minecraft:item/generated",
    "textures": {
        "layer0": "minecraft:item/arrow"
    },
    "overrides": [
        {"predicate": {"custom_model_data": 1}, "model": "foo:item/example"},
        {"predicate": {"custom_model_data": 2}, "model": "something:folder/etc"}
    ]
}
```
</details>

5. If `sounds.json` is present in both packs, the entries must be combined again. Unlike with model overrides, the order does not matter for sounds.
6. If, after loading the combined pack, missing textures are present, follow these troubleshooting tips:
    * If every instance of an item is a 2D missing texture, the JSON file likely has incorrect syntax.
    * If only some overrides of an item are 2D missing textures, the paths to the models in the overrides may be invalid.
    * If overrides are rendering models correctly but are missing textures, the paths to the textures in the model files may be invalid.
    * If the pack is not appearing in the resource pack list at all, the `pack.mcmeta` file may be missing or have invalid syntax. 

## Resetting your resource pack cache
1. Close your instance of Minecraft
2. Head over to `%AppData%/.minecraft/`
3. Delete the `server-resource-packs` folder
4. Restart your game
5. Done!