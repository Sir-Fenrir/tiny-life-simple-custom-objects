# A custom table for in Tiny Life
**The texture is from the Example Mod by Ellpeck Games**

This mod is loaded using the (Simple Object Loader)[https://github.com/Sir-Fenrir/simple-object-loader] mod.

Instead of writing code, you can just create a JSON file (ending in '.simple.json'), which consists of key-value pairs, describing the object you want to add.

Here we have an example of the configuration you can use for a table. With some comments we will clarify why the properties are needed. Note that comments can't be placed in the JSON files themselves, it will break them.

```
{
  "modId":  "CustomTable", // The unique identifier for this mod.
  "categories": ["Table"], // The categories, required for knowing what the object should do (in this case, be a table)
  "price": 200,
  "name":  "CustomTable", // This is the INTERNAL name of the object, not the one shows in menus. Should correspond with the name in the atlas file (if any) and the localization files.
  "atlas": "CustomFurniture", // The name of the atlas file in the same directory (if any)
  "size": [ 1, 1 ], // To describe the size of the object, in squares (first is x, second is y)
  "colorSchemes": [ "SimpleWood" ], // The colorschemes to use.
  "TableSpots":  [1, 1] // How much of the table can be used as a table to slot seats and place items. I think it can be the same as the size.
}
```