# I. Epigraphic Data in QGIS

[Exercise data and Additional eductional material](https://drive.google.com/drive/folders/1q3xprKgpIYMI-sxLS_GJ_d5CzwamfFd3)

This section is created by [Pieter Houten](https://orcid.org/my-orcid?orcid=0000-0002-7872-782X) for the Summer Course [De la piedra a tu pantalla](https://github.com/Toletum-Network/QGIS_Classical_Studies/blob/6e620c8c056454c908a899416d2eb0c27e007521/Summer%20course%20De%20la%20piedra%20a%20tu%20pantalla.pdf) in Zaragoza. The section is a basic instruction to map and analyse epigraphic data. As such the page holds basic insctructions treated in more detail in other modules. For the more detailed inscructions follow the links to the main course. If you are new to QGIS it might be best to quickly review [Module 2](https://github.com/Toletum-Network/QGIS_Classical_Studies/blob/master/Training_Manual/2.%20Module:_The_Interface.md#2-module-the-interface) to get an idea of the interface.

**``! Note``** <br>
The [QGIS Online Course for Classical Studies](https://github.com/Toletum-Network/QGIS_Classical_Studies#qgis-online-course-for-classical-studies) uses 3.16 LTR screenshots. We will be using the QGIS 3.22 LTR ([Download here](https://qgis.org/en/site/forusers/download.html#)) which might have a slightly different User Interface (UI).

The the project file in our drive is set to the Portuguese Coordinate Reference System: EPSG: 3763 ERTS89/ Portugal TM06.
It is advised to download all the data from the Drive and save it on your local drive. Files in the could tend to get corrupted due to network failures.

## I.1. Epigraphic Data

For our epigraphic data we resort to the publications in corpora and journals or to the epigraphic databases. In the past years we have seen a rise in databases providing different (sub)sets of epigraphy. Each of these has their own focus and thereby also pitfalls. One of the major problems of the epigraphic datasets is the limited spatial information. Often databases chose to select a (modern) place to represent all epigraphy of a specific region (e.g. the modern capital of a municipality for all epigraphy within this municipality). This decision might be to avoid the problems we encounter when we start entering findspots: are these the primary location of the inscription, or was it found in a secondary location? Despite these issues we can gather and combine information from these datasets and where needed improve spatial information.

The databases used for the data of our course are:

* [Hispania Epigraphica](http://eda-bea.es/)
* [Epigraphik-Datenbank Clauss/Slaby](https://db.edcs.eu/epigr/epi.php?s_sprache=en)
* [Epigraphic Database Heidelberg](https://edh.ub.uni-heidelberg.de/)
* [Trismegistos](https://www.trismegistos.org/)

Much of the data we will be using has been curated within the ERC-Project [LatinNow](latinnow.eu), which aims at publishing its [LatinNow database](https://latinnow.eu/online-resources-2/databases-and-data/) in September 2022, and the ANR/DFG-project [ATLAS](http://atlas-cities.com/) and its work-in-progress [Huma-Num database](https://geoapps.huma-num.fr/adws/app/5b1c0f10-7386-11ec-b348-11e51a07f6b0/).

**The goal for this lesson:** Understanding and using QGIS for spatial analysis of epigraphic data.

**``! Note``** <br>
We will use the epigraphic data on the Conventus Pacensis. This data is digitally obtained via above mentioned datasets and improved using the publications by d'Encarnação *IRCP* and *IRCP 25 anos depois*.

## I.2 ![Basic](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/basic.png) Starting our map
Open the project file [*Pacensis_NAME.qgz*](https://drive.google.com/drive/folders/1q3xprKgpIYMI-sxLS_GJ_d5CzwamfFd3).

### I.2.1 ![Basic](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/basic.png) Base layer
When we have the project open we should have a base layer from the Consortium of Ancient World Mappers ([CAWM](http://cawm.lib.uiowa.edu/index.html))

A base layer helps us to find our bearing within the project. Depending on the type of base layer we can obtain different forms of infomation. For instance the geography, as in our case. The base layer we are using is a WMTS (Web Map Tile Service), this is an online layer composed of tiles. You will notice that when we zoom in and out the map will slowly fill the tiles. This type has the advantage that we don't have to save a large file. However, when we find ourselves without an internet connection, we will not have a base layer.

### I.2.2 ![Basic](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/basic.png) Adding vector data
Besides a neat base layer we need some other data to work with. Before adding the epigraphy we will add some more data. All this data is in vector shape. To understand more about Vector data you can review Modules [4](https://github.com/Toletum-Network/QGIS_Classical_Studies/blob/master/Training_Manual/4.%20Module:%20Classifying%20Vector%20Data.md), [6](https://github.com/Toletum-Network/QGIS_Classical_Studies/blob/master/Training_Manual/6.%20Module:%20Creating%20Vector%20Data.md) and [7](https://github.com/Toletum-Network/QGIS_Classical_Studies/blob/master/Training_Manual/7.%20Module:%20Vector%20Analysis.md).<br>
There are three main types of vector data:
* Point
* Line 
* Polygon

These correspond to the data we will be uploading:
* Settlements
* Roads 
* Territories

Let's add the first layers. The **``Data Source Manager``** dialog allows you to choose the data to load depending on the data type. We’ll use it to load our dataset: click the ![Data Source Manager](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/Open%20Data%20Source%20Manager.png) **``Open Data Source Manager``** button.

If you can’t find the icon, check that the **``Data Source Manager``** toolbar is enabled in the **``View ‣ Toolbars``** menu.

![2.1.1 B Toolbar](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Screenshots/2.1.1%20B%20Toolbar.png)

Load the _**Pacensis_Settlements.shp**_ vector dataset:
* Click on the ![image](https://user-images.githubusercontent.com/66669249/175533646-13e606fc-b39a-444e-968a-3ed247228800.png) **``Vector``** tab.
* Enable the ![radiobutton](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/radiobuttonon.png) **``File``** source type.
* Press the **``…``** button next to **``Vector Dataset(s)``**.
* Select the _**Pacensis_Settlements.shp**_ file in your directory with the files for the course.
* Click **``Open``**. You will see the original dialog, with the local file path filled in.

![2.1.1 C browser vector data](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Screenshots/2.1.1%20C%20browser%20vector%20data.png)

* Ignore the **``Options``** fields.
* Click **``Add``** here as well. The data you specified will now load: you can see a _**Pacensis_Settlements.shp**_ item in the **Layers panel** (bottom left) with its features shown in the main map canvas.
* Close the **``Data Source Manager``** dialog

Congratulations! You now have a basic map. Now would be a good time to save your work.

### I.2.3 ![Basic](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/basic.png) Try Yourself
Repeat the steps above to add the _**Pacensis_Roads.shp**_ and _**Pacensis_Territories.shp**_ layers from the same folder to the map. You can order your layers in the Layer Panel by dragging them: left click the layer you want to move, hold and drag up or down. If the CAWM layer covers your other layers, drag it to the lowest postion in the Layers Panel. 

## I.3 ![Basic](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/basic.png) Working with Vector Data
All these layers are in a very simple layout. Depending on the layer order (ideally we have point layer, line layer, polygon layer and last base layer) we can see the different layers. But there is no differentation in the points and lines. Since our datasets have attributes ([more on attributes in Module 3](https://github.com/Toletum-Network/QGIS_Classical_Studies/blob/master/Training_Manual/3.%20Module:_Creating_a_Basic_Map.md#311--follow-along-viewing-layer-attributes)) we can categorize our data.

### I.3.1 ![Basic](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/basic.png) Polygon Data
We will start with the polygon data, or our territories. These are based on a 6 hour walking distance from the centres of self-governing communities of Pacensis (Houten 2021). When we right click the layer _**Territories**_ we can open the **`Properties`**. Then **`Symbology`**. Here we can start creating a new way of displaying the layer. We have multiple options:
* No Symbols
* Single symbol (this is default)
* Categorized
* Graduated
* Rule-based
* Merged Features
* Inverted Polygons
* 2.5 D

We will continue with Single Symbol, but change the way it looks. Our polygons are now with a fill, which hides the base layer. As we want to see the base layer we are going to change the fill.

Click *``Simple Fill``*. You will see the ``Fill color``. By clicking the small arrow on the right of the bar with the ``Fill color`` we can check the box for ``Transparent Fill``.

![image](https://user-images.githubusercontent.com/66669249/175313712-2e26ca21-d0b7-42ee-ad47-6b80e46e039e.png)

Next we want the outline of our territories to be a less strong and follow a dotted pattern. We set the ``Stroke Width`` to '0.20' and the ``Stroke Style`` to 'Dot Line'.

Now we can see our base layer and have the territories less prominent on our map. 

### I.3.2 ![Basic](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/basic.png) Line Data
Next up are the roads. When we right click the layer _**Roads**_ we can open the **`Properties`** again. We follow through until we see the options of **`Symbology`**:
* No Symbols
* Single symbol (this is current)
* Categorized
* Graduated
* Rule-based
* Merged Features
* Embedded Symbols

We see that there are some differences with the polygon layer. This has to do with the different nature of the datatype. It is important to consider your data and what you want to do with it before deciding on what type of vector layer you are using. Let's continue with changing the symbology of our layer.

We will use the categorized. Under value we choose '*LAYER*' and the Symbol will be a simple line (should be default). Then we click **``Classify``** on the bottom left. 
Now we have _Main Road_, _Secondary Road_ and _all other values_. Double click the line symbol before _Main Road_ to get the 'Symbol Selector' pane.

![image](https://user-images.githubusercontent.com/66669249/175317210-c5e8108e-1735-452b-abc9-520493069551.png)

Your pane will have only one Simple Line for your _Main Road_. Change the **``Color``** of this line to white and **``Stroke With``** to _0.2_. Click on ![image](https://user-images.githubusercontent.com/66669249/175535447-a8ed30c3-601c-4762-ac0e-51fac08376bd.png) to add another line below the white line. Change the **``Color``** of this new line to black and **``Stroke With``** to _0.4_. Click **``OK``**.
Change the Secondary Road **``Color``** to black and **``Stroke With``** to _0.15_.

Now we have a map with a clear differentation between the types of roads. Moreover, on the left hand pane we can now see that the Layers panel has the option to deselect the types. If we want we can create a map with only the Main Roads.

### I.3.3 ![Basic](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/basic.png) Point Data
Lastly we will turn to the most complicated dataset of these sets: the Settlements. Let us first get an idea of our data. 

Right click the ``Settlements layer`` and select ``Open Attribute Table``.<br>
You will now see the table with the different columns and rows. 

![image](https://user-images.githubusercontent.com/66669249/175321093-7208601d-665c-405e-9b22-8d4373f6ad12.png)

The column _id_  is mandatory for shapefiles to differentiate between the features. We add the _Name_, as it is often easier for us to remember names than numbers. Then we find the column _Type_, we will use this column for the symbology. Upon closer look we find that some Type attributes have more than one data point. For instance Lisboa, being a ``Municipium; Port; Balnea``. This makes differentiating slightly more complicated, the simple **``Categorized``**, which we used for our Line data, will not work.

Let's see what happens if we use **``Categorized``** as the way to differentiate the``Type`` of our layer.

After we have clicked  **``Classify``**, we can see all types in our list. It is difficult to differentiate between the different juridical status of the communities. In an ideal dataset we create separate columns for these kinds of data. Sometimes we find that data is not entered as we would like to see.
However, we can solve this issue rather simply with another way of working with symbology: **``Rule-based``**.

When we change **``Categorized``** to **``Rule-based``** we notice that we now have rules for each label. We can rewrite the rules and then have a different classification. By double clicking a rule we open the **``Edit Rule``** pane and can start editing.

![image](https://user-images.githubusercontent.com/66669249/175337793-04170392-22ff-4f7f-bcb3-530030b48aaa.png)

In Filter we rewrite the rule by simply replacing the = with 'LIKE' and add % before and after the word. If we start with the Balnea we change ``"Type" = 'Balnea'`` to ``"Type" LIKE '%Balnea%'``.
As you might notice the balnea now also includes the place Caldas do Monchique (entered as 'Balnea cult') and Lisboa (Municipium; Port; Balnea). The ``%`` has the rule neglect all before and after the ``%``. This way we can reorganize our classification by changing all entries to LIKE statements filtering on one type:
* Balnea
* Civitas
* Colonia
* Conventus Capital
* Provincial Capital
* Epigraphy
* Mine
* Municipium
* Port
* Quarry
* Rural
* Sanctuary
* Settlement
* Vicus
* Villa

In our dataset it is not needed to do this for all types, as some are not combined. For example, Villa works perfectly fine without the LIKE, as there are no combinations. However, we might change the data and then end up combining villa with something else.

Our next step is to change the symbology as to easily identify our different settlements. For this we can use different markers. Double clicking the marker opens the Edit Rule pane again. We see that we can change the Symbol here. 

![image](https://user-images.githubusercontent.com/66669249/175337793-04170392-22ff-4f7f-bcb3-530030b48aaa.png)

Several of the Symbols used in the example are chosen from the standard symbols. The civitas symbol is the ``topo pop capital``, with a size _2.2_. Similarly, the municipium, colonia and provincial capital are based of the diamond shaped symbols with size _2.2_.

For the mine, quarry, port and sanctuary we will use another type of marker: ``SVG Marker``.

Click the marker of the Mine. Again the ``Edit Rule`` pane opens. Under Symbol and the Marker we see ``Simple Marker``. When clicking this ``Simple Marker`` we see that the options below change. Now we select ``SVG Marker`` in *``Symbol layer type``*. The marker should have changed to a `?`.
Scroll down to the ``SVG Browser`` and select the symbol with two hammers in the SVG Images pane:

![image](https://user-images.githubusercontent.com/66669249/175344575-15435bca-255b-4966-b05b-c8951f08e6ee.png)

Change the ``Size`` of the SVG Marker to _4.0_ and the ``Fill color`` to black.

**``! Note``** <br>
You can also edit a marker by double clicking it in the ``Layers`` panel on the left.

For Quarry select the same symbol and make the ``Fill color`` white, make sure the ``Stroke color`` is black and ``Stroke width`` _0.2_.
repeat the steps for the Port (anchor) and sanctuary (temple).

You will notice that the port symbol and that of the municipium are overlapping in the cases of Lisboa and Balsa. We can edit the Port marker so it is slightly offset. Under our editing options we find the **``Anchor point``**. Change the _``VCenter``_ to _``Top``_. This moves the SVG image slightly down.

![image](https://user-images.githubusercontent.com/66669249/175347306-2cbad6ba-e742-4229-b6c5-46419720bf22.png)

Your map should look something like this:

![image](https://user-images.githubusercontent.com/66669249/175347983-148bcdc3-9004-4f71-a793-18d5702cb08a.png)


### I.3.4 ![Basic](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/basic.png) Sheets to QGIS
Often we tend to work in sheets (Excel, OpenOffice, Google etc.) with our data. It would be great to have the possibility to upload this data directly into our QGIS.<br>
This is possible if we use the CSV (Comma Separated Value) format. When saving our sheets we can opt to save it as a CSV.

#### I.3.4.1 ![Basic](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/basic.png) Adding a Delimited Text layer
We can upload the CSV via the **``Data Source Manager``** dialog allows you to choose the data to load depending on the data type. We’ll use it to load our datast on Emerita Augusta in Late Antiquity. This data has been collected within the [ATLAS-project](www.atlas-cities.com) and is mostly based on the [CILAE](https://cil2digital.web.uah.es/) database.

Click the ![Data Source Manager](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/Open%20Data%20Source%20Manager.png) **``Open Data Source Manager``** button. Select the ![image](https://user-images.githubusercontent.com/66669249/175493332-d80bc172-3e4e-4031-800f-6761694af71e.png) Delimited text tab and click the **``...``** to open the directory. Locate the CSV ``Emerita_epigraphie``. 

![image](https://user-images.githubusercontent.com/66669249/175494217-8bc04792-0941-4846-9543-a557b7da2405.png)

As CSV or Delimited text files can be very different we have to check our data before uploading it. The **``Data Source Manager``** gives us a multitude of options to tweak how we enter our CSV. Let's have a look at it from top to bottom ([More info on QGIS page](https://docs.qgis.org/3.22/en/docs/user_manual/managing_data_source/opening_data.html#geometry-definition)).

First we have our``File name`` with the directory. Followed by the ``Layer name``, in this case ``Emerita_epigraphie``. And the ``Encoding`` of our file. Note that this is an important field to check. Often this is set on ``UTF-8`` or ``Latin-9``. At the bottom of the screen we see our **``Sample data``**. Before importing the data it is good to keep an eye on the changes here. If we find unexpected or strange signs in our attribute values, then we need to change the ``Encoding``.

Next we turn to **``File Formart``**. Here we select the way our data is constrcuted. When we open the csv in excel we can see the delimiter. In our case it is a semi-colon ``;``, so we have to select **``Custom delimiters``** and select _Semicolon_. 

**``! Note``** <br>
When working with a Delimited text it is important to decide on the delimiter and NEVER use this delimiter in your attribute values. This way we avoid problems woith uploading our data. In the case you are working with data obtained from others (without a good practice of delimiters) we can select multiple delimiters in the "Custom delimiters".

The **``Record and Field Options``** allows us to discard rows under ``Number of header lines to discard``. And indicate the Header of the colums with the ``First record has field names``.

**``Geometry Definition``** handles our spatial information. When working with our epigraphy in a sheet we have to collect the spatial data. This can be done in different formats (here given for Zaragoza):
* Sexagesimal [DMS](https://en.wikipedia.org/wiki/Degree_(angle)#Subdivisions): 41°39′0″ N, 0°53′0″ W
* [Decimal Degrees](https://en.wikipedia.org/wiki/Decimal_degrees): 41.65, -0.883333 (note that we find them with ° as well, this has to be deleted)
* [UTM](https://en.wikipedia.org/wiki/Universal_Transverse_Mercator_coordinate_system): 4613082 676259 30T (UTM needs the Zone, in this case 30T)

As the **DMS** and **UTM** can easily lead to mistakes (or typos) it is best to use the **DD** (Decimal Degrees) format. We label our fields X/Y or Longitude/Latitude. 
Then we select our ``Geometry CRS`` using the ![image](https://user-images.githubusercontent.com/66669249/175505355-8a54a79b-64ae-45dd-ba94-ffe4dcdc73da.png). We can alwas change the CRS later in our ``Layers panel``. For our data we use the ``CRS`` **EPSG: 4326 - WGS 84**.
 
Click **``Add``**, you can check the data in the project and if it is good, then click **``Close``**. 

Now we have added the CSV to our project. We can manipulate the symbology in the same manner as the shapefiles we have been doing before. The downside of the Delimited text layer is that we cannot edit it within QGIS. You will notice that the ![image](https://user-images.githubusercontent.com/66669249/175506009-b40aa1ef-3cbe-4801-967d-ef3150aa019c.png) ``Edit`` icon is grey. If we want to edit the attribute values we need to do this in the CSV and then save the CSV file. After hitting the ![image](https://user-images.githubusercontent.com/66669249/175506680-3bc64ce5-2c65-44f3-bdcd-22755cb9ea0d.png) ``Refresh`` button we will see the changes in QGIS.

**``! Note``**<br>
If you work with a CSV in QGIS and need to change anything else than attribute values (e.g. the name of the file, directory of the file, the names of columns or the number of columns), you will need to add the layer again.

#### I.3.4.2 ![Basic](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/basic.png) Delimited text to Shapefile
If we want to work with the data as Vector data in shapefile format we can save it as a ESRI Shapefile. Richt click the layer in the layer panel. Then **``Export ‣ Save Features As...``** and the "Save Vector Layer As..." panel opens. 
It should have ESRI Shapefile as default format. Choose the directory under File Name via ``...``, select the preferred folder.
Leave all other field to default. make sure the box "Add saved file to map" is checked and hit ``OK``. 

For more info on editing Vector data see [Module 6](https://github.com/Toletum-Network/QGIS_Classical_Studies/blob/master/Training_Manual/6.%20Module:%20Creating%20Vector%20Data.md#6-module-creating-vector-data).

## I.4 Analysing Epigraphic Data
Now we have a basic map of Pacensis and we can upload the shapefile with the inscriptions from the conventus Pacensis. The inscriptions are all as single dots on the map. This way we have no way to work with them. Take a look at the attribute table to see the dataset and get an idea of our possibilities.<br>
This data has been collected within the [LatinNow](latinnow.eu) project.

### I.4.1 ![moderate](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/moderate.png) Filtering Data
We will query and filter this data to create different kinds of maps. For this we will go one step deeper into writing expressions in SQL (the language we already used for the Rule-based symbology). If you want to learn more on SQL you can follow an [online tutorial](https://www.w3schools.com/sql/default.asp). 

Click ![image](https://user-images.githubusercontent.com/66669249/175481361-437bda00-12dc-45e8-b5f3-fc23bb7c5e49.png) next to the **``Filter``** to open the **``Expression String Builder``**. Here we can write criterion for our filter. The central pane gives us the different expressions.

To sort the epigraphy we need to select the field (column) that we are going to select on. Let us start with Funerary epigraphy: Double click _`Fields and Values ‣ Text Type`_. You will see that on the left side we now have the start of an expression: "Text Type". If we click **`All Unique`** on the right side we can have a look at the way our Text Type data is ordered. It is clear we need the % to get all our Funerary epigraphy.

Complete the expression: "Text Type" LIKE '%Funerary%'.

Now we are going to add another filter. We want to only see the funerary inscriptions on marble. The statement for this would be "Material" LIKE '%Marble%'. To combine these we need the operator AND. Leading to the following expression:

"Text Type" LIKE  '%Funerary%' <br>
AND <br>
"Material" LIKE '%Marble%'
 
**``! Note``** <br>
It is not needed to write each statement on one line. However, for readability of larger expressions it is good practice to write each statement on a separate line.

When we have written our expression correctly we will see to the bottom left "Preview: 0". If we have a mistake the Preview states "Expression is invalid". Check your expression for mistakes. Note that these could also be in the quotation marks " or '.

### I.4.2 Quantifying Data
Even after our filtering we have the issue that in one location we might have multiple inscriptions. There are different ways of demonstrating this, the easiest ways are found under **``Symbology``**. here we findthat point data has a few options we have not yet treated:
* Point displacement
* Point Cluster
* Heatmap
These will be the focus of this section.

First set the _**``Inscriptions``**_ layer back to ``Single symbol``.

#### I.4.2.1 ![Basic](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/basic.png) Point Cluster
Under symbology we can switch the ``Symbology`` of our _**``Inscriptions``**_ to ``Point Cluster``. The single dots now have a number if we find more than one feature (inscription) in a location. Note that when we zoom out we see that the clusters become fewer. This can be changed with the ``Distane``. When we set the distance to _3000_ Meters at scale, we create clusters based on 3 km areas. We can choose the distance we consider useful for our analysis.

![image](https://user-images.githubusercontent.com/66669249/175771405-2a48bdad-dd98-4fcf-8e26-e8752ee8c8d8.png)

#### I.4.2.2 ![moderate](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/moderate.png) Point Displacement
Point displacement is not really an ideal way of showing data with multiple features on one location. It can quickly become a very cluttered map. However, it can be a quick way to establish what we have and what to pay attention to.

When we switch the ``Symbology`` of our _**``Inscriptions``**_ to ``Point Displacement`` we will end up with large circles all over the map. Similar to the ``Point Cluster`` we find the total number of features (inscriptions) indicated on the location.

Our first step is the change **``Placement method``** to ``Concentric Rings``. This brings our data closer to the location and when we zoom in we can start recognizing some patterns regarding high and low concentrations. 

The ``Point Displacement`` provides us the possibility to use the other options of the  ``Symbology``to differentiate our data. Let's switch our **``Renderer``** from ``Single Symbol`` to ``Categorized``. We will categorize our selection based on _``Material``_.

When we have done this you will notice that the concentric rings now have a colourful palette. We can now delete the non-stone materials and colour the stone materials in a way that we can interpret it:

![image](https://user-images.githubusercontent.com/66669249/175772881-c9e477e6-24c1-4a3b-8cde-3d5573e8a515.png)

I have opted to colour a few stone types. Stone is red (note that stone is often the default in epigraphic corpora, leading to a very problematic set). As we can see the data still needs some curation. The double entries still need to be checked (these are the result of automatically combining different datasets). Nonetheless, all that holds _marble_ is white, _granite_ is grey, _sandstone_ orange and _slate_ is black.

Click ``Apply``. Now the map is easier to read. Note that the numbers on the location now only refer to the stome material inscriptions!

![image](https://user-images.githubusercontent.com/66669249/175772973-06da3ce8-bf2e-4b33-9548-34f7465d84ab.png)

When we open the **``Renderer``** and uncheck the box before ``Stone``. We can filter out these unspecified stone types and see a pattern. The use of Granite is mostly found in the north, whereas limestone is used in the south. Marble concentrates in the centre, which is little suprising as we find the quarries of Estremoz in this region.

#### I.4.2.3 ![moderate](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/moderate.png) Heatmap
The last method for our course is the ``Heatmap``. This allows us to quickly display concentrations of epigraphy. Again we find a few parameters to tweak our map. First the ``color ramp``, the default setting is white to black (where black shows high concentration). <br>
We can play with the colors and even set the lowest value to transparant:
* Click the ``color ramp`` to open the ``Select Color Ramp`` pane.
* Double click on the Color Ramp in the pane to add a Gradient stop (preferably just to the right of the left stop).
* Now we have two adjacient stops on the left side. 
* Select the utmost left stop by clicking it
* Set opacity to 0%
* Click ``OK``
You will now see that the Heatmap is limited.

The ``Maximum value`` can be very helpful when we have one place with a very high concentration of epigraphy. That is, if we find that our map has one black centre and the rest is white.<br>
When we change our ``maximum value`` to _100_ we see that the other areas become clearer. However, Pacensis has no extremes, so it is not really needed. In the case of the epigraphy of the cnventus Tarraconensis the ``Maximum value`` is certainly needed to limit the effect of Tarraco with its high concentration of epigraphy.

For the epigraphy we cannot use the ``Weight points by``, this allows to weight your points by a numerical attribute. For example, if we were to plot settlements we could have them weighted by their size attribute. This way we are looking at concentrations of settlements (clusters will create a concentration) and large settlements as they would appear based on the weight.

Lastly we have the ``Rendering quality``. This is a handy tool to quickly see your results. In the case of large datasets the ``Heatmap`` function can take a while to calculate. When ``Rendering quality``is set to _Fastest_ we get a very pixelated map, but it gives us an idea of what parameters we might have to change. After we have the Heatmap we want to show we can then set ``Rendering quality``to _Best_ for mapping.

## I.5 Mapping our results
After doing our analyses and demonstration we often want a printed map for publication. Unfortunately the course has limited time for QGIS. <br>
Creating maps is explained in the online course in [Module 5: Creating Maps](https://github.com/Toletum-Network/QGIS_Classical_Studies/blob/master/Training_Manual/5.%20Module:%20Creating%20Maps.md#5-module-creating-maps).

[Back to Start](https://github.com/Toletum-Network/AutumnSchool_2020#autumnschool-2020)

