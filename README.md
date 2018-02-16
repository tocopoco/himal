# himal
3D visualisation of Himalaya
HimalViewer
The web app will  use the open source programs CesiumJS and Nodejs server.
HimalViewer will help mountaineering and trekking society to create archives of mountaineering in  Himalaya - and any other mountain region of the Earth, in future  also  other planets , which have  a Digital Planet Model.  CesiumJS supurts Digital Earth Model delivered by Google Earth and Bing API, but also other DEM models can be loaded.
HimalViewer will suport GEOREFERENCING which means:
If you know a place on the map or geo-location  ( latitude and longitude , opotionally altitude ) the viewer will create   360 degrees  view  from the place - virtually created from the DEM.
HimalViewer will suport REVERSE PHOTO-REFERENCING , which means :  
For a mountain panorama ( in the form of JPG , PNG etc.)   where you recognise some  named peaks  or landmarks with known geographic coordinates - the viewer will help to find a place where the camera was situated and oriented.  Then the viuew created by GEOREFERENCING will show a similar virtual panorame with  all the  names of   visible landmarks which are in the database.
 Himal Viewer will be interractive, alowing the admin to  add names of topographic features  and names  landmarks , and in case of  summits, passes and mountain faces - date of  first ( and other ) ascents , and names of summiters.. The search will allow to find in the records a place-name or summiter's name.
The diference with other GIS projects , 3D API like Google Earth or Bing :
1 HimalViewer will offer consistent ordering  of all mountain  features in a linear order - it means that each summit  , mountain pass, valley , mountain face will have well defined index from the mathematic concept of a node in the hydrological graph and a node in the graph of mountain ridges. Practically it will allow to find automatically ( without user or admin input )
1. all valleys in a neighbourhood of a mountain
2. all mountains in the surrounding of a valley, and their mountai faces in the order - from left to roght ( looking up )
UNCLIMBED MOUNTAINS
For any geo-location - it will be easy to display all named and   unnamed  ( but important ) topographic objects - in the same valley or on the same ridge.  Of course "importance" must be classified mathematically   as many secondary  summits, passes and tributary valleys are not considered important and they must be cut  off in the graphs and not added to database.   The topographic criteria for valleys and rivers are to some extend defined in methods of computational hydrology , but for ridges, mountains and passes the hydrological rules have limited value ( only in case of cutting  off secondary ridges similar with secondary tributaries of rivers )  and for mountain summits  and passes  there is necessary to define rules slightly described  in the international classificator of mountains in the   http://www.theuiaa.org/mountaineering/mountain-classification/ .  
In the last clasification  there are  two variables of "autonomy criterium " - minimal path  distance dX  ( let us say 1000 meters ) , and minimal altitude difference  dY = 30 meters  -  ., and passes or summits with smaller path and altitude difference are ignored.
It is obvious that for bigger dX and bigger dY the selection  will  choose less peaks and passes - so they can be considered  more important  This way we can add to the database all sufficiently "important" summits  often unnamed and unclimbed  , what has some significance for  climbers.
