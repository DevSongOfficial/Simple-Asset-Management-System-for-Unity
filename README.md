# How to Use Simple-Asset-Management-System

1. Place any prefab you want to access at runtime through AssetManager.cs into the Resources folder.
2. The folder structure should be: Resources - Prefabs - [Folder Name] - [Prefab Name]
3. Based on this structure, a corresponding [Prefab.cs] file will be automatically generated.
4. Prefabs placed in the General folder will be automatically added to the editor UI, allowing you to drag and drop them into the scene. (See LevelEditorUI.cs for details.)

Unity Addressable Asset System 보다 비용적으로 비효율적일 수 있음을 알고있지만,
1. Custom Asset Management System을 만들어보고 싶었으며,
2. 이를 통해 Prefab 등록을 위한 절차를 최대한 간소화시켜 작업 효율 및 유지보수성을 높이고 싶었다.
