# Answer Sheet
### 2.1.2 _Adding Your First Layer_
In the main area of the dialog you should see many shapes with different colors. Each shape belongs to a layer you can identify by its color in the left panel (your order and the colors may be different from the ones below):

![2.1.2 Answer](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Screenshots/2.1.2%20Answer.png)

[Back to text](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Training_Manual/2.%20Module:_The_Interface.md#212--try-yourself)
## 2.2 _An Overview of the Interface_
### 2.2.2 Try Yourself 1
![2.2.1 A interface](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Screenshots/2.2.1%20A%20gui_numbered.png)
The elements identified in the figure above are:

1. Layers List / Browser Panel
2. Toolbars
3. **Map canvas**
4. **Status bar**
5. **Side Toolbar**
6. **Locator bar**

[Back to text](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Training_Manual/2.%20Module:_The_Interface.md#222---try-yourself-1)

### 2.2.3 Try Yourself 2
1. **``Save as``**
2. **``Zoom to layer``**
3. **``Invert selection``**
4. **``Rendering on/off``**
5. **``Measure line``**

[Back to text](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Training_Manual/2.%20Module:_The_Interface.md#223---try-yourself-2)

### 3.1.2 Try Yourself Exploring Vector Data Attributes
There should be **8** fields in the **``roads``** layer:

1. Select the layer in the **``Layers``** panel.
2. Right-click and choose **``Open Attribute Table``**, or press the ![openTable](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/mActionOpenTable.png) button on the **``Attributes Toolbar``**.
3. Count the number of columns.

**``!Tip``**

A quicker approach could be to double-click the **``roads``** layer, open the **``Layer properties ‣ Fields``** tab, where you will find a numbered list of the table’s fields.

Information about places is available in the **``places layer``**. Open its attribute table as you did with the **``roads``** layer: there are **26** fields. The amount of data available might seem overwhelming at first. But when working with big data it is good practice to spend some time on understanding the _fields_ and _records_. 

[Back to text](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Training_Manual/3.%20Module:_Creating_a_Basic_Map.md#312--try-yourself-exploring-vector-data-attributes)

### 3.2.2 Try it Yourself colors
* Verify that the colors are changing as you expect them to change.
* It is enough to select the **``provinces``** layer in the legend and then click on the ![Symbology](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/symbology.png) _Open the Layer Styling panel_ button. Click the color and change the opacity of the color to 0%. The boundary of the province will remain black. You can choose to change this as well.

**!Note**
If you use the opacity of the layer, that is the blue slider in the layer styling, you will make the whole layer transparent.
If you want to work on only one layer at a time and don’t want the other layers to distract you, you can hide a layer by clicking in the checkbox next to its name in the layers list. If the box is blank, then the layer is hidden.

[Back to text](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Training_Manual/3.%20Module:_Creating_a_Basic_Map.md#322--try-yourself)

### 3.2.4 Try it Yourself Changing Symbol Structure
Your map should now look like this:

![3.2.4 B](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Screenshots/3.2.4%20A%20result%20symbology%202.png)

[Back to text](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Training_Manual/3.%20Module:_Creating_a_Basic_Map.md#324--try-yourself)

### 4.1.1. ![basic](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/basic.png) Follow Along: Attribute data

The _canon_name_ field is the most useful to show as labels. This is because all its values are unique for every object and are very unlikely to contain NULL values. If your data contains some NULL values, do not worry as long as most of your places have names.

[Back to text](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Training_Manual/4.%20Module:%20Classifying%20Vector%20Data.md#411--follow-along-attribute-data)

### 6.1.4 ![basic](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/basic.png) Digitizing
The symbology doesn’t matter, but the results should look more or less like this:

![Results 6.1.4 B](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Screenshots/6.1.4%20B.png)

[Back to text](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Training_Manual/6.%20Module:%20Creating%20Vector%20Data.md#614--try-yourself-digitizing-lines)

### 7.2.6. ![basic](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/basic.png) Try Yourself Distance from Tagili
The **``Buffer distance``** is **``5``** kilometer.

The **``Segments to approximate``** value is set to **``20``**. This is optional, but it’s recommended, because it makes the output buffers look smoother. Compare this:

![7.2.6 Answer A](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Screenshots/7.2.6%20Answer%20A.png)

To this:

![7.2.6 Answer B](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Screenshots/7.2.6%20Answer%20B.png)

The first image shows the buffer with the **``Segments to approximate``** value set to **``5``** and the second shows the value set to **``20``**. In our example, the difference is subtle, but you can see that the buffer’s edges are smoother with the higher value.

[Back to text](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Training_Manual/7.%20Module:%20Vector%20Analysis.md#726--try-yourself-distance-from-tagili)

### 7.2.8. ![basic](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/basic.png) Follow Along: One hour from Tagili

![7.2.8 Answer](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Screenshots/7.2.8%20Answer.png)

[Back to text](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Training_Manual/7.%20Module:%20Vector%20Analysis.md#728--follow-along-one-hour-from-tagili)

### 7.2.10. ![moderate](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/moderate.png) Try Yourself Further Filter

The **``Clipping tool``** should be filled as follows:

![7.2.10 Answer A](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Screenshots/7.2.10%20Answer%20A.png)
The final result should look like this:

![7.2.10 Answer B](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Screenshots/7.2.10%20Answer%20B.png)

[Back to text](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Training_Manual/7.%20Module:%20Vector%20Analysis.md#7210--try-yourself-further-filter)

### 7.3.3 ![moderate](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/moderate.png) Try Yourself Fastest path

Open **``Network Analysis ‣ Shortest Path (Point to Point)``** and fill the dialog as:

![7.3.3 A](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Screenshots/7.3.3%20A%20fastest_path_result.png)

Make sure that the **``Path type to calculate``** is _Fastest_.

Click on **``Run``** and close the dialog.

Open now the attribute table of the output layer. The **``cost``** field contains the travel time between the two points (as fraction of hours):

![7.3.3 B](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Screenshots/7.3.3%20B%20fastest_path_attribute.png)

[Back to text](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Training_Manual/7.%20Module:%20Vector%20Analysis.md#733--try-yourself-fastest-path)

### 9.1.2 ![moderate](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/moderate.png) Try Yourself

![9.1.2 A](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Screenshots/9.1.2%20A.png)

[Back to text](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Training_Manual/9.%20Module:%20Completing%20the%20Analysis.md#912--try-yourself)

### 9.2.3 ![moderate](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/moderate.png) Try Yourself Finishing the Analysis

The final result should be something like this:

![9.2.3](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Screenshots/9.2.3%20Answer.png)

[Back to text](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Training_Manual/9.%20Module:%20Completing%20the%20Analysis.md#923--try-yourself-finishing-the-analysis)

### 9.3 Assignment

Your final map should look something like this: 

![9.3](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Screenshots/9.3%20Answer.png)

Obviously the warning should not be included in your result. However, when making maps we have to realise that this will be taken as a reality by many people. We should always keep this in mind when creating maps, especially when we put these online.

As a visual aid to understand the landscape we have also activated the DEM we created in [Module 8.1.2](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Training_Manual/8.%20Module:%20Rasters.md#812--follow-along-create-a-virtual-raster) and the hillshade of [Module 8.3.1](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Training_Manual/8.%20Module:%20Rasters.md#831--follow-along-calculating-a-hillshade).

[Back to text](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Training_Manual/9.%20Module:%20Completing%20the%20Analysis.md#93-assignment)


### 12.1.4 ![moderate](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Icons/moderate.png)  Try Yourself Calculating the aspect

![12.1.4 Answer A](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Screenshots/12.1.4%20Answer%20A.png)
![12.1.4 Answer B](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Screenshots/12.1.4%20Answer%20B.png)

[Back to text](https://github.com/Toletum-Network/AutumnSchool_2020/blob/master/Training_Manual/12.%20Module:_Site_Catchment.md#1214--try-yourself-Calculating-the-aspect)
