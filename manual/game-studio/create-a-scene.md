# Create and open a scene

<span class="label label-doc-level">Beginner</span>
<span class="label label-doc-audience">Level Designer</span>

When you create a new project, Game Studio creates an initial scene and populates it with basic entities such as a light, a camera, and a skybox.

You can create scenes like any other asset. As they are complex assets, they have a dedicated editor, the **scene editor**.

## Create a scene

1. In the **asset view** (by default in the bottom pane), click **Add asset** and select **Scenes**.

    ![Add a scene](media/add-scene.png)

2. Select the appropriate **scene template**.

    Template | Result
    ---------|--------
    Empty scene | An empty scene with no entities or preconfigured rendering pipeline
    Scene with HDR pipeline | A scene containing basic entities and preconfigured for HDR rendering
    Scene with LDR pipeline | A scene containing basic entities and preconfigured for LDR rendering

## Open a scene in the scene editor

In the **asset view**:

![Select a scene in the asset view](media/open-scene-from-asset-view.png)

* double-click the scene asset, or
* right-click the asset and select **Edit asset**, or 
* select the asset and type **Ctrl + Enter**

> [!TIP]
> You can have several scenes open simultaneously.

## Use the scene editor

![Scene editor](media/create-a-scene-default-scene-editor.png)

The **scene editor tabs** (A) display the open scenes. You can switch between open scenes using the tabs.

The **entity tree** (B) shows the hierarchy of the entities included in the scene. The same entity hierarchy is applied at runtime. You can use the entity tree to browse, select, rename, and reorganize your entities.

You can use the **tool bar** (C) to modify entities and change the scene editor display.

The **main window** (D) shows a simplified representation of your scene, with your entities positioned inside it. For entities that have no shape (E), Game Studio represents them with **2D gizmos**; for example, cameras are represented with camera icons.

## See also

* [Navigate in the scene editor](navigate-in-the-scene-editor.md)
* [Manage scenes](manage-scenes.md)
* [Load scenes](load-scenes.md)
* [Add entities](add-entities.md)
* [Manage entities](manage-entities.md)