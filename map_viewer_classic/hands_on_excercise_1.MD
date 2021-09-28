# Map Viewer Classic - Excercise 1
### Author: Dennis Milechin, Research Computing Services, Boston University


## Content
  * [Navigation](#navigation)
  * [Measure Tool](#measure-tool)
  * [Download Data](#download-data)
  * [Upload Shapefile to ArcGIS Online](#upload-shapefile-to-arcgis-online)
  * [Upload CSV File to ArcGIS Online](#upload-csv-file-to-arcgis-online)
  * [Add Layer in Map Viewer](#add-layer-in-map-viewer)
  * [Explore Attribute Table](#explore-attribute-table)
  * [Apply Symbology](#apply-symbology)
  * [Layer Order](#layer-order)
  * [Add Labels](#add-labels)
  * [Save](#save)
  * [Share Web Map](#share-web-map)
  
## Navigation
**Now let's learn how to use the Map Viewer.**

1. Log onto ArcGIS Online portal. (https://bucas.maps.arcgis.com/)
1. Top menu click on `Map`. This will load the map viewer.  
    
    <img src="snippets/18_map_page.png" width="700">

    **You might be asked if you want to try the Beta version of Map Viewer.  This tutorial will focus on the current stable release, so decline the request.**  
	
    **Let's review some basic navigation tools availabe in this environment.**

1. To pan, move the mouse to the map pane, left click and drag, and then release.
1. To zoom in, click the `+` button located at the top left of the map viewer.
1. To zoom out, click the `-` button.  
    
    <img src="snippets/19_zoom_in_out.png" width="100">

1. If you have a mouse with a scroll wheel or options, you can use that to zoom in and out as well.
1. To reset your view, click on the button that has the icon of a house, also known as the `default extent`, located between the `+` and `-` buttons.  
    
	<img src="snippets/19_zoom_in_out.png" width="100">
    
    **Near the top right, there is a `Find address or place` field where we can type in and address or location name.**  
    
	<img src="snippets/20_search_bu.png" width="700">

1. Type in `Boston University` and hit the enter key on your keyboard.
    
    **The result is the web map will zoom onto the location of Boston University Charles River Campus.  We can save this view by saving it as a bookmark.**

1. To the left of the `Find address or place` search field is a button titled `Bookmarks`.  Click on the button and then `Add Bookmark`.  
    
	<img src="snippets/21_add_bookmark.png" width="700">

1. Type in `Boston University` and hit enter on your keyboard.  This now saved this extent as a bookmark.
1. To test the book mark, click on the `Default Extent`, to return the view of the United States.  
    
	<img src="snippets/19_zoom_in_out.png" width="100">
	
1. Click on the `Bookmarks` button and then on `Boston University`.  This will zoom back to the extent of the bookmark.  
    
	<img src="snippets/22_click_bookmark.png" width="400">

\[[top](#content)\]

## Measure Tool
**ArcGIS Online provides us with some tools to measure things on the map. Let's learn more about the measure tool.**

1. Click on the `Measures` button which is to the left of the `Bookmarks` button.  
    
	<img src="snippets/23_click_measure.png" width="700">

    **There are three options for measuring tools: area, linear distance, and location.**

1. Select the `Area` button, which is located on the far left of the pop-up window.  
    
    <img src="snippets/24_click_area.png" width="400">

1. Move the mouse to the map, and left click to define the first vertex.
1. Move the mouse to another location and then left click to define the next vertex.
1. Continue the process to outline an area of interst.
1. When done, double left click to finalize the area, the results of the area is shown in the `Measure` pop-up window.  
    
	<img src="snippets/25_defined_area.png" width="500">

1. You can change the units of the result in the drop down menu on the far right, where it currently might be selected to `Sq Miles`.
    
    <img src="snippets/26_area_change_units.png" width="400">

    **For `Distance` it is the the button next to `Area`.  Using this tool is nearly identical on how the area tool is used.  For `Location` tool (far right button) shows the coordinates for a clicked location and also the coordinates of the mouse, when it is hovering over the map.**

\[[top](#content)\]

## Download Data
**First we need to download the data we will use.  Please download the CSV file linked below.**
1. Click on the link below to download the tutorial zip files..
    [tutorial_files.zip](https://rcs.bu.edu/examples/gis/tutorials/arcgis_online_portal/tutorial_files.zip)  
    https://rcs.bu.edu/examples/gis/tutorials/arcgis_online_portal/tutorial_files.zip
1. Unzip the zip files.

    **The zip file contains a directory called `mbta_rapid_transit` with a collection of files that represent a shapefile.  Additionally the zip file contains a CSV files called `mbta_subway_stations.csv`, which containts coordiante locations of MBTA subway stops and associated attributes.**

\[[top](#content)\]

## Upload Shapefile to ArcGIS Online

   **First let's upload the Shapefile.  We can only upload the shapefile if it is compressed into a zip file.**

1. Compress the `mbta_rapid_transit` directory into a zip file.  Use the method that is applicable to the operating system you are using.
1. Log onto ArcGIS Online portal. (https://bucas.maps.arcgis.com/)
1. At the top menu click on `Content` and `My Content`.  
    <img src="snippets/1_click_on_content.png" width="700">

1. Click on `Add Item` -> `From Your Computer`  
    <img src="snippets/2_Add_item.png" width="300">  

1. A new window will appear.  Click on `Your Device`.    
    <img src="snippets/3_choose_file.png" width="500"> 
1. Find and select the zip file you just created. 
1. In the next window, under "Item type", "Shapefile" should be selected.  If not, use the drop down menu to select the "Shapefile".  

    <img src="snippets/3.1_shapefile_select_type.png" width="800">

1. For question "How would you like to add this Shapefile"? Select "Add mbta_rapid_transit.zip and create a hosted feature layer".  

    <img src="snippets/3.1_how_to_import_shapefile_1.png" width="800">

1. Click "Next" button.

1. In the title field, append your username at the end. This is needed because the hosted table needs to be unique within the BU origanization.  So we all cannot create a hosted table with the same name.
1. Select the folder you want to save this layer in.
1. Add tags, such as `Boston` and `MBTA`.  
    <img src="snippets/4_add_file_form_shapefile.png" width="500">

1. Click "Save".

    **This will upload the file and take you to the description page for your new feature layer.**

    <img src="snippets/5_shapefile_desc_page.png" width="500">

\[[top](#content)\]


## Upload CSV File to ArcGIS Online

   **Next, let's upload the CSV files.**

1. Log onto ArcGIS Online portal. (https://bucas.maps.arcgis.com/)
1. At the top menu click on `Content` and `My Content`.  
    <img src="snippets/1_click_on_content.png" width="700">

1. Click on `Add Item` -> `From Your Computer`  
    <img src="snippets/2_Add_item.png" width="300">  

1. A new window will appear.  Click on "Your device" and find and select the CSV file that was downloaded.
    <img src="snippets/3_choose_file.png" width="500">  

1. For question "How would you like to add this CSV file"? Select "Add CSV and create a hosted feature layer".
    <img src="snippets/3.1_how_to_import_csv_2.png" width="800">

1. Click "Next" button.

1. Here we can select what columns to import from our CSV file and also change the column names by updating the "Display name". 
    <img src="snippets/3.2_csv_fields_review.png" width="800"> 
1. No changes required, click "Next".
1. On this next page we need to specify that we want to use coordinates to locate the stations.  Click on the drop down menu for "Location settings".  
    <img src="snippets/3.3_select_location_settings_stations.png">
1. Select "Latitude and longitude".
1. We need to specify location fields.  For "Latitude" select `POINT_Y`.
1. For "Logitude" select `POINT_X`.  
    <img src="snippets/3.4_select_location_fields.png" width="800">

1. Click "Next".
1. In the title field, append your username at the end. This is needed because the hosted table needs to be unique within the BU origanization.  So we all cannot create a hosted table with the same name.
1. Select the folder you want to save this layer in.
1. Add tags, such as `Boston` and `MBTA`.  
    <img src="snippets/4_add_file_form_csv_station.png" width="500">

1. Click "Save".

    **This will upload the file and take you to the description page for your new feature layer.**

    <img src="snippets/5_station_desc_page.png" width="500">

1. If you update the the CSV file and need to re-upload the CSV file.  Use the "Update Data" button on the right side.  
    <img src="snippets/5.1_update_data.png">


\[[top](#content)\]


## Add Layer in Map Viewer
**Nots let's add the data we uploaded.**

1. Log onto ArcGIS Online portal. (https://bucas.maps.arcgis.com/)
1. Click on `Map` on the top menu.
1. Top left, click the `Add` button --> `Search for Layers`.  
    
	<img src="snippets/27_search_layer.png" width="400">  
    
    **Left pane will change listing layers available in your `My Content` page.**
  
    <img src="snippets/27.1_add_layer_my_content.png" width="500">  

1. You should see the two layers we uploaded listed. Click on the `+` button on the bottom left of the layer listing to add them. 
    
	<img src="snippets/29_add_layer_click_plus_mbta.png" width="500">  
    
    **The layer appears in the map view pane.**
    
    <img src="snippets/30_layer_added_mbta.png" width="500">  

1. Click the back arrow located to the left of `My Favorites` to return to the content pane.  
    
	<img src="snippets/31_back_to_content.png" width="400">
1. Click on `Content` tab, which is to the right of `About`.   
    
	<img src="snippets/32_map_content_page_click_mbta.png" width="400">
    
    **This will show the layers that are available to be displayed on the map view.**

1. Click on "Legend" to see how the layers are symbolized.  
    <img src="snippets/32.1_click_legend.png">


\[[top](#content)\]


## Explore Attribute Table
**We want to symbolize the layer with the values from the attribute table.  Let's take a look at the attribute tables.**

1. Click on "Content".
1. Hover over the `mbta rapid transit...` layer and additional button will appear.  
    <img src="snippets/32.3_hover_over_layer.png">
1. Click on the `Show Table` icon.  
    <img src="snippets/32.4_show_table_icon.png" width="25">

    **The Attribute Table will appear at the bottom. We want to color each subway line with its associated line color using the `LINE` column.**

    <img src="snippets/32.5_mbta_transit_att_table.png">


\[[top](#content)\]

## Apply Symbology

**Let's change how the `mbta subway stations` point look.**

1. Hover over the `mbta subway stations...` layer and click on "Change style" button.  
     <img src="snippets/32.5_change_style_button.png" width="25">
1. For step 1, in the drop down menu, select "Show location only".
1. For step 2, click on the "OPTIONS" button under "Location (single symbol)".  
    <img src="snippets/32.10_symb_stations_single_location.png">

1. Click on the "Symbols" link to open a new window.  
    <img src="snippets/32.11_symbols_link.png">
1. Explore the symbology window and select a good symbol for subway station stops.
1. Click "OK" to close the symbology selection window.
1. Click "OK" in the left pane to save the options.
1. Click "DONE" to save the symbology settings.


**Now let's apply the symbology of the subway lines using the attribute table.**

1. On the left pane, make sure "Content" is selected.
1. Hover over the `mbta rapid transit...` layer until the additional button appear.
1. Click on the `Change Style` button:  
    <img src="snippets/32.5_change_style_button.png" width="25">

1. The left pane will go to the "Change Style" form.  For step 1, in the drop down menu select the attribute `LINE`.  
    <img src="snippets/32.6_change_style_select_attribute_line.png">

1. Step 2, we are going to symbolize by "Unique symbols".  Click on "Options" under "Types (Unique symbols)".  
    <img src="snippets/32.7_unique_symbols_options_transit.png">
1. The left window pane will now give you the option to change the individual colors.  Click on the colored lines to the left of the "LABEL" column to select a color that matches the LABEL.  
    <img src="snippets/32.8_change_transit_color.png">
1. Your selection and map should look similiar to this:  
    <img src="snippets/32.9_selected_colors.png">
1. Click on "OK" to save the Options settings.
1. Click on "Done" to save the symbology setup.



\[[top](#content)\]

## Layer Order
**On your map it might happen that the station stops appear below the subway lines.  The order of the layers in the "Content" pane matter.  The layer listed at the top will be drawn on top of all the other layers.  Here lets move the layers around.**

<img src="snippets/32.12_layer_order_sample.png">

1. Hover over a layer, so that the additional menu items appear.
1. Click on the three dots `...` button on the far right side.  
   <img src="snippets/32.13_three_dots_button.png">

1. Then click on either the "Move up" or "Move down" option.  
   <img src="snippets/32.14_move_up_down.png">

    **You should see the layer move up or down the list.  Observe the map viewing area and you should see the order of the layers being drawn change as well.**

\[[top](#content)\]

## Add Labels
**Let's add labels to the station stops.**
1. Hover over the layer `mbta subway stations`, and click on the three dots button `...`.  
    <img src="snippets/32.13_three_dots_button.png">
1. Click on "Create Labels".  
    <img src="snippets/32.15_create_label.png">
1. For the field "Text", in the drop down menu, select `STATION`.  As this is the attribute we want to use from our attribute table.  
    <img src="snippets/32.16_set_label_options.png">

    **At this point look at the map viewer and you should see a label next to each station, with it's station name.**
1. Adjust the font as desired.
1. Click "OK"

    
\[[top](#content)\]

## Save
**At this point it is good to save the map, so we don't lose our changes accidently.**

1. Upper mid-point of the window is a `Save` button.
    
	<img src="snippets/45_save_button.png" width="700">

1. Click on `Save` and then `Save As`.
1. A form will appear that you will need to fill out. Fill it out with the information below, but subsitute your username for my username where you see`_milechin`:
    
    <img src="snippets/46_save_map_form_mbta.png" width="500">
    
    **The map is now saved.  Periodically, click on the `Save` --> `Save` button to save any changes while progressing through this workshop.**

\[[top](#content)\]

## Share Web Map
**At this point you may want to share a map with someone else by giving them a url. Let's look at how this is done.**

1. Click n the `Share` button which is to the right of the `Save` button.
    <img src="snippets/72_map_share_button_click.png" width="300">
    
    **Before we can share the map, we need to change the permissions of who can view it.  The form contains several checkboxes for selecting with whom we want to share the map with.**
    * `Everyone (public)` will allow anyone in the world to see it.  
    * `Boston University College of Arts and Sciences` will restrict it to BU community who have an ArcGIS Online account.  
    * Finally, we can restrict access to a particular group.

1. Click the checkboxes for who you want to have access to this map. In this example I am only going to share it with the BU community by checking `Boston University College of Arts and Sciences`.
    
	<img src="snippets/73_map_share_permission_select.png" width="700">

1. Further down the form there is a section `Link to this map` that contains a short URL you can share with others.
    <img src="snippets/74_map_share_link.png" width="500">

1. Click on `DONE`.

    **The permissions are now set and you can share the map with others.  You can also copy the link that is at the top of the browser and share that with others as well.**
    
    **Let's take a closer look permissions from `My Content` page.**

1. Navigate to `Content` --> `My Content`
    
    **Look at the permissions column for the items listed and you will see that the permission icon changed for the web map we shared.**
    

1. Click on the permissions icon.
    
    **A new window will appear which will allow you to modify permissions for that particular item.**
    
    <img src="snippets/76_my_content_permissions_change.png" width="300">

1. Once you chose the permission level you want for this item, `OK`.

\[[top](#content)\]
