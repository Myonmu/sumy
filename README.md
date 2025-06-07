![](resources/icon-small.jpg)

# sumy

Sumy is an Inky fork that works with the [sumi fork](https://github.com/Myonmu/sumi) of the ink compiler and runtime.

## Preprocessor Symbols
![image](https://github.com/user-attachments/assets/1242ef7a-b3bd-445c-a02c-749b006acce1)
Sumy supports sumi's preprocessor symbols. When editing in Sumy, `INKY` symbol is enabled by default. When exporting, however, no symbol will be fed to the compiler.
You can specify your own symbols with the `mainInkFileName.settings.json` file:
```json
{
    "inkySymbols": ["INKY", "SUMY", "SUMI"],
    "exportSymbols": ["SUMI"]
}
```
Here, `inkySymbols` will be fed to the live compiler when editing, and `exportSymbols` will be fed to the compiler when exporting json.
