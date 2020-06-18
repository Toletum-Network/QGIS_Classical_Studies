# 2. Module: The Interface
After completing this section, you will be able to correctly identify the main elements of the screen in QGIS and know what each of them does. You will also be able to load a layer into QGIS.


## 2.1. Lesson: Adding your first layer
We will start the application, and create a basic map to use for examples and exercises.
**The goal for this lesson:** To get started with an example map.

Note
Before starting this exercise, QGIS must be installed on your computer. Also, you should have downloaded the [sample data](https://drive.google.com/drive/folders/1S8lygvwGiy5UBM8SGo_LSB1tShKqPbV2) to use. **NEEDS TO REFER TO REPOSITORY IN GITHUB**
Launch QGIS from its desktop shortcut, menu item, etc., depending on how you configured its installation.

**! Note**
The screenshots for this course were taken in [QGIS 3.10.6 LTR](https://www.qgis.org/en/site/) running on Windows. Depending on your setup, the screens you encounter may well appear somewhat different. However, all the same buttons will still be available, and the instructions will work on any OS. You will need QGIS 3.10.6 LTR (the latest LTR at the time of writing to use this course).
Let’s get started right away!

### 2.1.1. ![Basic](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/basic.png) Follow Along: Prepare a map
1. Open QGIS. You will have a new, blank map.
![2.1.1 A Blank Map](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Screenshots/2.1.1%20A%20Blank-map.png)

2. The **Data Source Manager** dialog allows you to choose the data to load depending on the data type. We’ll use it to load our dataset: click the ![Data Source Manager](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/Open%20Data%20Source%20Manager.png) *Open Data Source Manager* button.
If you can’t find the icon, check that the **Data Source Manager** toolbar is enabled in the **View ‣ Toolbars** menu.
![2.1.1 B Toolbar](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Screenshots/2.1.1%20B%20Toolbar.png)


3. Load the _**provinces.shp**_ vector dataset:
* Click on the **Vector** tab.
* Enable the ![radiobutton](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/radiobuttonon.png) **File** source type.
* Press the **…** button next to **Vector Dataset(s)**.
* Select the [_**exercise_data/shapefile/provinces.shp**_](https://drive.google.com/drive/folders/16C_g2qheeME3CCTDUAJbRj8oyoqrFKDR) file in your training directory.
* Click Open. You will see the original dialog, with the file path filled in.
![2.1.1 C browser vector data](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Screenshots/2.1.1%20C%20browser%20vector%20data.png)

* Click **Add** here as well. The data you specified will now load: you can see a _**provinces**_ item in the **Layers panel** (bottom left) with its features shown in the main map canvas.

Congratulations! You now have a basic map. Now would be a good time to save your work.

1. Click on the **Save As** button: ![Save as](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/mActionFileSaveAs.png)
2. Save the map under a _**solution**_ folder next to _**exercise_data**_ and call it _**basic_map.qgz**_.

### 2.1.2. ![Basic](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/basic.png) Try Yourself
Repeat the steps above to add the _**places.shp**_ and _**rivers.shp**_ layers from the same folder (_**exercise_data/shapefile**_) to the map.

[Check your results](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Training_Manual/Answer_Sheet/Answer_sheet.md)

### 2.1.3. In Conclusion
You’ve learned how to add a layer from a Shapefile dataset and create a basic map!

### 2.1.4. What’s Next?
Now you’re familiar with the basic function of the **Open Data Source Manager** button, but what about all the others? How does this interface work? Before we go on, let’s first take a look at the layout of the QGIS interface. This is the topic of the next lesson.

## 2.2. Lesson: An Overview of the Interface
We will explore the QGIS user interface so that you are familiar with the menus, toolbars, map canvas and layers list that form the basic structure of the interface.
The goal for this lesson: To understand the basics of the QGIS user interface.

### 2.2.1. ![Basic](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/basic.png) Try Yourself: The Basics
![2.2.1 A interface](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Screenshots/2.2.1%20A%20gui_numbered.png)
The elements identified in the figure above are:
1. Layers List / Browser Panel
2. Toolbars
3. Map canvas
4. Status bar
5. Side Toolbar
6. Locator bar

#### 2.2.1.1. ![Basic](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/basic.png)  The Layers List
In the Layers list, you can see a list, at any time, of all the layers available to you.
Expanding collapsed items (by clicking the arrow or plus symbol beside them) will provide you with more information on the layer’s current appearance.
Hovering the layer will give you some basic information: layer name, type of geometry, coordinate reference system and the complete path of the location on your device.
Right-clicking on a layer will give you a menu with lots of extra options. You will be using some of them before long, so take a look around!

**! Note**
A vector layer is a dataset, usually of a specific kind of object, such as roads, trees, etc. A vector layer can consist of either points, lines or polygons.

#### 2.2.1.2. ![Basic](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/basic.png)  The Browser Panel
The QGIS Browser is a panel in QGIS that lets you easily navigate in your database. You can have access to common vector files (e.g. ESRI Shapefile or MapInfo files), databases (e.g. PostGIS, Oracle, SpatiaLite, GeoPackage or MSSQL Spatial) and WMS/WFS connections. You can also view your GRASS data.
If you have saved a project, the Browser Panel will also give you quick access to all the layers stored in the same path of the project file under in the ![Project file](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/mIconQgsProjectFile.png) **Project Home** item.
Moreover, you can set one or more folder as Favorites: search under your path and once you have found the folder, right click on it and click on _**Add as a Favorite**_. You should then be able to see your folder in the ![Favorite](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/mIconFavourites.png) **Favorites** item.

**! Tip**
It can happen that the folders added to Favorite item have a really long name: don’t worry right-click on the path and choose _**Rename Favorite...**_ to set another name.

##### 2.2.1.3. ![Basic](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/basic.png)  Toolbars
Your most often used sets of tools can be turned into toolbars for basic access. For example, the File toolbar allows you to save, load, print, and start a new project. You can easily customize the interface to see only the tools you use most often, adding or removing toolbars as necessary via the **View ‣ Toolbars** menu.
Even if they are not visible in a toolbar, all of your tools will remain accessible via the menus. For example, if you remove the **File** toolbar (which contains the **Save** button), you can still save your map by clicking on the **Project** menu and then clicking on **Save**.

##### 2.2.1.4. ![Basic](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/basic.png)  The Map Canvas
This is where the map itself is displayed and where layers are loaded. In the map canvas you can interact with the visible layers: zoom in/out, move the map, select features and many other operations that we will deeply see in the next sections.

#### 2.2.1.5. ![Basic](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/basic.png)  The Status Bar
Shows you information about the current map. Also allows you to adjust the map scale, the map rotation and see the mouse cursor’s coordinates on the map.

##### 2.2.1.6. ![Basic](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/basic.png)  The Side Toolbar
By default the Side toolbar contains the buttons to load the layer and all the buttons to create a new layer. But remember that you can move all the toolbars wherever it is more comfortable for you.

#### 2.2.1.7. ![Basic](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/basic.png)  The Locator Bar
Within this bar you can access to almost all the objects of QGIS: layers, layer features, algorithms, spatial bookmarks, etc. Check all the different options in the [Locator Settings](https://docs.qgis.org/testing/en/docs/user_manual/introduction/qgis_configuration.html#locator-options) section of the QGIS User Manual.

**! Tip**
With the shortcut Ctrl+K you can easily access the bar.

### 2.2.2. ![Basic](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/basic.png)  Try Yourself 1
Try to identify the four elements listed above on your own screen, without referring to the diagram above. See if you can identify their names and functions. You will become more familiar with these elements as you use them in the coming days.

[Check your results](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Training_Manual/Answer_Sheet/Answer_sheet.md)

### 2.2.3. ![Basic](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/basic.png)  Try Yourself 2
Try to find each of these tools on your screen. What is their purpose?
1. ![Save As](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/mActionFileSaveAs.png)
2. ![Zoom to layer](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/mActionZoomToLayer.png)
3. ![Invert selection](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/mActionInvertSelection.png)
4. ![Toggle Render](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/toggle_render.png)
5. ![Measure](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/mActionMeasure.png)

**! Note**
If any of these tools is not visible on the screen, try enabling some toolbars that are currently hidden. Also keep in mind that if there isn’t enough space on the screen, a toolbar may be shortened by hiding some of its tools. You can see the hidden tools by clicking on the double right arrow button in any such collapsed toolbar. You can see a tooltip with the name of any tool by holding your mouse over the tool for a while.

[Check your results](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Training_Manual/Answer_Sheet/Answer_sheet.md)

### 2.2.4. What’s Next?
Now you’ve seen how the QGIS interface works, you can use the tools available to you and start improving on your map! This is the topic of the next lesson.

## 2.3. Lesson: Navigating the Map Canvas
This section will focus on basic QGIS navigation tools used to navigate within the Map Canvas. These tools will allow you to visually explore the layers at different scales.

The goal for this lesson: Learn how to use Pan and Zoom tools within QGIS and learn about map scale.

### 2.3.1. ![Basic](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/basic.png) Follow Along: Basic Navigation Tools
Before learning how to navigate within the Map Canvas, let’s add two additional layers that we can explore during this tutorial.

1. Use the steps learnt in [Create a Map lesson](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Training_Manual/Module_The_Interface.md#211--follow-along-prepare-a-map) to add ESRI Shapefiles _**roads.shp**_ and _**buildings.shp**_ as layers to the current project. The result view should look similiar to the snippet below:
**INSERT SCREENSHOT 2.3.1 A**
Let’s first learn how to use the Pan Tool.

* In the Map Navigation Toolbar, make sure the ![pan](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/mActionPan.png)_Pan_ button is activated.
* Move the mouse to the center of the Map Canvas area.
* Left-click and hold, and drag the mouse in any direction to pan the map.

Next, let’s zoom in and take a closer look at the layers we imported.

* In the _Map Navigation Toolbar_, click on the ![zoomIn](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/mActionZoomIn.png)_Zoom In_ button.
* Move your mouse to approximately the top left area of where there is the highest density of buildings and roads.
* Left click and hold.
* Then drag the mouse, which will create a rectangle, and cover the dense area of buildings and roads.
**INSERT SCREENSHOT 2.3.1 B**
* Release the left click. This will zoom in to include the area that you selected with your rectangle.
**INSERT SCREENSHOT 2.3.1 C**
* To zoom out, select the ![zoomOut](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/mActionZoomOut.png)_Zoom Out_ button and perform the same action as you did for zooming in.

As you pan, zoom in, or zoom out, QGIS saves these views in a history. This allows you to backtrack to a previous view.

* In the _Map Navigation Toolbar_, click on ![zoomLast](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/mActionZoomLast.png)_Zoom Last_ button to go to your previous view.
* Click on ![zoomNext](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/mActionZoomNext.png)_Zoom Next_ button to proceed to move forward in your history.

Sometimes after exploring the data, we need to reset our view to the extent of all the layers. Instead of trying to use the Zoom Out tool multiple times, QGIS provides us with a button to do that action for us.

* Click on the ![zoomFullExtent](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/mActionZoomFullExtent.png)_Zoom Full Extent_ button.

As you zoomed in and out, notice that the **Scale** value in the Status Bar changes. The **Scale** value represents the Map Scale. In general, the number to the right of **:** represents how many times smaller the object you are seeing in the Map Canvas is to the actual object in the real world.

![2.3.1 D map scale](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Screenshots/2.3.1%20D%20map_scale1.png)
You can also use this field to set the Map Scale manually.

* In the Status Bar, click on the Scale textfield.
* Type in _50000_ and press Enter. This will redraw the features in the Map Canvas to reflect the scale you typed in.
* Alternatively, click on the options arrow of the **Scale** field to see the preset map scales.
![2.3.1 E map scale options](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Screenshots/2.3.1%20E%20map_scale_options.png)

Select 1:5000. This will also update the map scale in the Map Canvas.

Now you know the basics of navigating the Map Canvas. Check out the User Manual on [Zooming and Panning](https://docs.qgis.org/testing/en/docs/user_manual/introduction/general_tools.html#zoom-pan) to learn about alternative ways of navigating the Map Canvas.

### 2.3.2. In Conclusion
Knowing how to navigate the Map Canvas is important, as it allows one to explore and visually inspect the layers. This could be done for initial data exploration, or to validate output of a spatial analysis.
