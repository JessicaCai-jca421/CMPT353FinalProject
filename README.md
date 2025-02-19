# CMPT 353 Final Project
Data analysis software for obtaining geographical location through pictures

### Learning Objective
1. If I were to plan a tour of the city (by walking/biking/driving), where should I go? What are some paths that can walk me past interesting things and various landmarks?
2.  Some parts of the city have more chain restaurants (e.g. McDonald’s or White Spot franchises, not independently-owned places): is that true? Is there a way to find
these chained restaurants automatically and to visualize their density relative to non-chain restaurants?
3. If I was going to choose a hotel (or Airbnb), where should it be? What places have good amenities nearby?




### Install Packages in the Computer Prompt

```
pip install folium
pip install pillow
pip install exifread
pip install GPSphoto
pip install piexif
```

### Dependencies 
Please install these libraries first

* Pandas
* Numpy
* math

### Run the Project

Please use the command below the run the project and given order.

 ` python hotel_selection.py photos/DT1.jpg `</br>
 ` python recommendedPath.py 13358 Photos/DT1.jpg `

For chain_res_distribution.ipynb directly run without command.

### Note

1. Please transfer photos via USB cable or U disk! If you use discord or messenger to transfer, the geographic location of the photo will be lost, resulting in reading errors!



2. The hotel_selection.py will generate a hotel_list file and an amenities_near_hotel.html file. The hotel_list file includes the hotel information near the visitor's current location. The amenities_near_hotel.html file shows the hotel's location and nearby facilities on the map. In the command, the first parameter is the photos from the photos folder, and the second is the file used to save the hotel list. If the program shows cleaned_data_hotel.latitude cleaned_data_hotel.longitude does not exist, there is no hotel around this location in the database.



3. The recommended_Path.py will create two HTML files. The first all-amenities file contains all tourist attractions from the hotel to the destination, allowing users to choose freely. The second picture recommends the shortest route through different scenic spots from the starting point to the destination based on the nearest route algorithm, and each scenic spot will only pass once.

   

4. The chain_res_distribution.ipynb will generate the following four HTML files:

	- all_restaurant_plot.html will display the distribution of all restaurants in a dot graph.
	- all_restaurant.html will display the distribution of all restaurants in the form of a heat map.
	- chain_restaurant_plot.html will display the distribution of all chain restaurants in a dot graph.
	- chain_restaurant.html will display the distribution of all chain restaurants in the form of a heat map.
		
##### Group Member:
ZhuoLiu 
WangSiWei 
TeLiangYu
##### Language
Python
