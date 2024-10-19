### Simple Asset Manager
This class scans folders and prefabs in **Resources** folder and creates a C# script file that contains enums based on it.

So you can create prefab like this:
```Unity
Instantiate(AssetManager.GetPrefab(Prefab.UI.SpawnButton_1));
```
This is designed specifically for my side scroller project.
- I made this in order to streamline the process of registering and creating prefabs.
- You can see the whole code from [3D-Side-Scroller](https://github.com/DevSongOfficial/3D-Side-Scroller).

#
### How To Use
1. Place any prefab you want to access at runtime through AssetManager.cs into the **Resources** folder.
2. Based on the structure, After clicking **Save Prefabs** Button in your custom editor, a corresponding **Prefab.cs** file will be automatically generated.
3. Now you can create your prefabs by calling `AssetManager.GetPrefab(enum prefabName);`
4. Prefabs placed in the General folder will be automatically added to the editor UI, allowing you to drag and drop them into the scene. (See LevelEditorUI.cs for details.)
#
