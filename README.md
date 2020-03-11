## MCMETA file

Is a JSON file that identifies your data pack.

Format:

```
{
  "pack": {
    "pack_format": 5,
    "description": "Tutorial Data Pack"
  }
}
```

## Data Folder

The data folder will contain the code to your data pack. The folder inside it will be the namespace for the functions and other features.

### data/namespace

The namespace folder is used to prevent conflicts between two data packs on the game with similar functions. Entries in data packs have namespaced IDs in a fashion of namespace:path. Example: a function of ID foo:handler/bar_call would be located at data/foo/functions/handler/bar_call.mcfunction.

The convention for namespaces are lower_case_with_underscores (lower snake case).

### [data/namespace/functions](https://minecraft.gamepedia.com/Function_(Java_Edition))

In this folder will be located all functions of the data pack, files with the .mcfunction extension or other subfolders of functions.Your function will be named in the game as (namespace):(name) or (namespace):(subfolder1)/(subfolder2)/.../(name) when the function file is located in a subfolder.

### [data/namespace/loot_tables](https://minecraft.gamepedia.com/Loot_table)

Loot tables will tell Minecraft what should be dropped when a mob dies or what should be generated inside containers, like chests, when opened for the first time.

### [data/namespace/tags](https://minecraft.gamepedia.com/Tag)

To utilize block, item, or function tags the JSON files must be placed in a data pack inside the data/(namespace)/tags/blocks, data/(namespace)/tags/items, data/(namespace)/tags/entity_types or data/(namespace)/tags/functions folder respectively.
