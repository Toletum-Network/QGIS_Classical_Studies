#2. Module: The Interface
After completing this section, you will be able to correctly identify the main elements of the screen in QGIS and know what each of them does. You will also be able to load a layer into QGIS.


## 2.1. Lesson: Adding your first layer
We will start the application, and create a basic map to use for examples and exercises.
**The goal for this lesson:** To get started with an example map.

Note
Before starting this exercise, QGIS must be installed on your computer. Also, you should have downloaded the [sample data](https://drive.google.com/drive/folders/1S8lygvwGiy5UBM8SGo_LSB1tShKqPbV2) to use. **NEEDS TO REFER TO REPOSITORY IN GITHUB**
Launch QGIS from its desktop shortcut, menu item, etc., depending on how you configured its installation.

Note
The screenshots for this course were taken in QGIS 3.10 running on Windows. Depending on your setup, the screens you encounter may well appear somewhat different. However, all the same buttons will still be available, and the instructions will work on any OS. You will need QGIS 3.10 (the latest version at time of writing) to use this course.
Let’s get started right away!

###2.1.1.  Follow Along: Prepare a map
Open QGIS. You will have a new, blank map.

The Data Source Manager dialog allows you to choose the data to load depending on the data type. We’ll use it to load our dataset: click the  Open Data Source Manager button.
If you can’t find the icon, check that the Data Source Manager toolbar is enabled in the View ‣ Toolbars menu.



Load the provinces.shp vector dataset:
Click on the Vector tab.
Enable the File source type.
Press the … button next to Vector Dataset(s).
Select the exercise_data/shapefile/provinces.shp file in your training directory.
Click Open. You will see the original dialog, with the file path filled in.



Click Add here as well. The data you specified will now load: you can see a provinces item in the Layers panel (bottom left) with its features shown in the main map canvas.




Congratulations! You now have a basic map. Now would be a good time to save your work.
Click on the Save As button: 
Save the map under a solution folder next to exercise_data and call it basic_map.qgz.
2.1.2.  Try Yourself
Repeat the steps above to add the places.shp and rivers.shp layers from the same folder (exercise_data/shapefile) to the map.
Check your results
2.1.3. In Conclusion
You’ve learned how to add a layer from a Shapefile dataset and create a basic map!
2.1.4. What’s Next?
Now you’re familiar with the basic function of the Open Data Source Manager button, but what about all the others? How does this interface work? Before we go on, let’s first take a look at the layout of the QGIS interface. This is the topic of the next lesson.
2.2. Lesson: An Overview of the Interface
We will explore the QGIS user interface so that you are familiar with the menus, toolbars, map canvas and layers list that form the basic structure of the interface.
The goal for this lesson: To understand the basics of the QGIS user interface.
2.2.1.  Try Yourself: The Basics

The elements identified in the figure above are:
Layers List / Browser Panel
Toolbars
Map canvas
Status bar
Side Toolbar
Locator bar
2.2.1.1.  The Layers List
In the Layers list, you can see a list, at any time, of all the layers available to you.
Expanding collapsed items (by clicking the arrow or plus symbol beside them) will provide you with more information on the layer’s current appearance.
Hovering the layer will give you some basic information: layer name, type of geometry, coordinate reference system and the complete path of the location on your device.
Right-clicking on a layer will give you a menu with lots of extra options. You will be using some of them before long, so take a look around!
Note
A vector layer is a dataset, usually of a specific kind of object, such as roads, trees, etc. A vector layer can consist of either points, lines or polygons.
2.2.1.2.  The Browser Panel
The QGIS Browser is a panel in QGIS that lets you easily navigate in your database. You can have access to common vector files (e.g. ESRI Shapefile or MapInfo files), databases (e.g. PostGIS, Oracle, SpatiaLite, GeoPackage or MSSQL Spatial) and WMS/WFS connections. You can also view your GRASS data.
If you have saved a project, the Browser Panel will also give you quick access to all the layers stored in the same path of the project file under in the  Project Home item.
Moreover, you can set one or more folder as Favorites: search under your path and once you have found the folder, right click on it and click on Add as a Favorite. You should then be able to see your folder in the  Favorites item.
Tip
It can happen that the folders added to Favorite item have a really long name: don’t worry right-click on the path and choose Rename Favorite... to set another name.
2.2.1.3.  Toolbars
Your most often used sets of tools can be turned into toolbars for basic access. For example, the File toolbar allows you to save, load, print, and start a new project. You can easily customize the interface to see only the tools you use most often, adding or removing toolbars as necessary via the View ‣ Toolbars menu.
Even if they are not visible in a toolbar, all of your tools will remain accessible via the menus. For example, if you remove the File toolbar (which contains the Save button), you can still save your map by clicking on the Project menu and then clicking on Save.
2.2.1.4.  The Map Canvas
This is where the map itself is displayed and where layers are loaded. In the map canvas you can interact with the visible layers: zoom in/out, move the map, select features and many other operations that we will deeply see in the next sections.
2.2.1.5.  The Status Bar
Shows you information about the current map. Also allows you to adjust the map scale, the map rotation and see the mouse cursor’s coordinates on the map.
2.2.1.6.  The Side Toolbar
By default the Side toolbar contains the buttons to load the layer and all the buttons to create a new layer. But remember that you can move all the toolbars wherever it is more comfortable for you.
2.2.1.7.  The Locator Bar
Within this bar you can access to almost all the objects of QGIS: layers, layer features, algorithms, spatial bookmarks, etc. Check all the different options in the Locator Settings section of the QGIS User Manual.
Tip
With the shortcut Ctrl+K you can easily access the bar.
2.2.2.  Try Yourself 1
Try to identify the four elements listed above on your own screen, without referring to the diagram above. See if you can identify their names and functions. You will become more familiar with these elements as you use them in the coming days.
Check your results
2.2.3.  Try Yourself 2
Try to find each of these tools on your screen. What is their purpose?





Note
If any of these tools is not visible on the screen, try enabling some toolbars that are currently hidden. Also keep in mind that if there isn’t enough space on the screen, a toolbar may be shortened by hiding some of its tools. You can see the hidden tools by clicking on the double right arrow button in any such collapsed toolbar. You can see a tooltip with the name of any tool by holding your mouse over the tool for a while.
Check your results
2.2.4. What’s Next?
Now you’ve seen how the QGIS interface works, you can use the tools available to you and start improving on your map! This is the topic of the next lesson.
