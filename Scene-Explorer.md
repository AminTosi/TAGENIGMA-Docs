Scene Explorer
--------------


**Quick links**

<a target=_blank href="https://www.assetstore.unity3d.com/#/content/7984">[Scene Explorer]</a> is available in the Unity Asset Store.

<a target=_blank href="http://forum.unity3d.com/threads/179306-Scene-Explorer-Remote-scene-editing">[Unity Showcase Thread]</a>

**Audience**

Package contents are targeted towards artists and programmers wanting to find performance bottlenecks in their game or application as it runs on the target device.

**Compatibility**

This project is targeted for Unity 4.2.2 or better. The project was tested on Windows/Mac/Android/OUYA.

**Package**

Scene Explorer includes Client/Server networking which allows the editor extension to run as a Host accepting incoming connections. The clients connect passing their scene info to the host. The host can request scene info while remotely activating/deactivating scene elements. The user measures performance to find bottlenecks. The package also includes a tree view control which displays the scene in a familiar searchable hierarchy.

**Playlist**

Visit the <a target=_blank href="http://www.youtube.com/playlist?list=PL4mjXeDqRBMS5dFZvqV8NDkOz5ZXXTRiq&feature=view_all">[video playlist]</a> for feature overviews of Scene Explorer.

**Menu Items**

**Client**

* Components\Scene Explorer\Add Scene Explorer Client
* This component should be added to a selected GameObject and will automatically connect to the Host on start. This GameObject will not be destroyed so in the case where you have multiple scenes, you’ll want to add the client to your first scene.

**FPS**

* Components\Scene Explorer\Add Scene Explorer FPS
* Measuring frames per second is useful when checking the performance of your application or game. Add this component to an existing GUIText object and set the RefGUIText meta reference back to the GUIText object.

**Panel**

* Window\Open Scene Explorer
* Open the panel to start a Host or Client connection.

**Examples**

**Client**

* Assets\SceneExplorer\Scenes1
* This scene is setup for a client and includes an example scene with content that can be remotely de/activated. The SceneExplorerClient GameObject has an attached script that establishes the client connection. Enter the Host (IP if available) and Port of the Host. You can hit play to run the Unity editor as a client and/or publish to a device which will connect to the Host on Start. The example also includes a sample FPS counter on the SceneExplorerFPS GameObject.

<img src="http://d3j5vwomefv46c.cloudfront.net/photos/large/816995394.png?1382509589"/>

<img src="http://d3j5vwomefv46c.cloudfront.net/photos/large/816995518.png?1382509644"/>

**Host**

Open the Scene Explorer Panel from the Window menu and start a Host connection by clicking Create Host on the Host tab. Choose a TCP port that is not already in use. Clients  will automatically connect to the Host.
Select a connected Client and click on Request Scene. This will send a request to the client to send the scene hierarchy.
With the scene hierarchy displayed, you can check or uncheck GameObjects in the scene while measuring FPS performance to find and hunt for bottlenecks. The TreeView also supports a search feature to assist hunting for GameObjects by name.

<img src="http://d3j5vwomefv46c.cloudfront.net/photos/large/816995604.png?1382509681"/>

<img src="http://d3j5vwomefv46c.cloudfront.net/photos/large/816995658.png?1382509709"/>

**Change Log**

1.0 – Initial submission of project.

1.1 – Added inspection of components, fields, and properties, and remote editing for Vector position, rotation, and scale. Split the panel into 3 sections for scene, components, and fields/properties.

1.2 - Added editing component fields.

1.3 - Includes full source. Upgraded to Unity 4! The panel is now vertically collapsable.

1.4 - Changed description to say documentation is available online versus moved online.

1.5 - Fixed warnings. Removed an extra UnityVS folder.

**Author**

Tim Graupmann 

You can send comments/questions to tim@tagenigma.com and any feedback you send will turn into new features.
