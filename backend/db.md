# Database Schema - MongoDB

## Project

| **id** | **project_name** | 
|--------|------------------|
| a234adsfa | TFO Tour |
| asd87f3f2 | Realgymnasium Tour |

## Container
**type** can be:
* text
* image
* video
* audio

| **id**| **page_id** | **name** | **x_coordinate** | **y_coordinate** | **width** | **height** | **type** | **content_id** |
|---------------|---------|--------------|------------------|------------------|-----------|------------|----------|----------------|
| 988a987s6324h | description | 282734hb234b | 40 | 20 | 100 | 200 | text | 3j46j34l53l3 |
| 786asd77234ff | logo_1 | h2hs634452s3 | 10 | 10 | 500 | 500 | image | kjhsdfh435h4 |

## Pages
Also stores the position of the page on the map.
There is always a main page, which has the map.
**name** is used for the route (/sn_labor) and for internatal id (The id field is created automatically by mongodb so we can ignore it). The **display_name** is the name that will be displayed on the page.

| **id** | **project_id** | **name** | **display_name** | **map_x** | **map_y** |
|--------|----------------|----------|------------------|-----------|-----------|
| 9823u4asd | a234adsfa | main | main | 0 | 0 |
| 9823u4asd | a234adsfa | sn_labor | SN Labor | 40 | 29 |
| la83u4a7z | asd87f3f2 | pc3 | PC Raum3 | 10 | 20 |

## Resources
The **type** can be:
* text
* image
* video
* audio 
* map (There is only one map on the main page) (Is actually an image used as a leaflet map)

| **id** | **type** | **blob** |
|--------|----------|----------|
| 23873h35 | text | 0393857584 |
| 982734h3 | image | 73648723423 |
| 203i4209 | map | 9827348927348 |
