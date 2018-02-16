# himal
3D visualisation of Himalaya

HimalViewer

The web app will  use the open source programs CesiumJS and Nodejs server.

HimalViewer will help mountaineering and trekking society to create archives of mountaineering in  Himalaya - and any other mountain region of the Earth, and perhaps in future  also mountain ranges of the planets, which have  a Digital Planet Model and climbing history.  CesiumJS suports Digital Earth Model delivered by Google Earth or by Bing API, but also it allows to load other DEM models.

HimalViewer will suport GEOREFERENCING which means:

If you know a place on the map or geo-location  ( latitude and longitude , opotionally altitude ) the viewer will create   360 degrees  view  from that place . The view is virtually created from the DEM.

HimalViewer will suport REVERSE PHOTO-REFERENCING , which means :  

For a mountain panorama ( in the form of JPG , PNG etc.)   where you recognise some  named peaks  or landmarks with known geographic coordinates - the viewer will help to find a place where the camera was situated and oriented.  After that the virtual view ( see: GEOREFERENCING )  will show a similar virtual panorama with labels , showing all the  place-names which are in the database.

 Himal Viewer will be interractive, alowing the admin to  add names of topographic features  and names  landmarks , and in case of  summits, passes and mountain faces - date of  first ( and other ) ascents , and names of summiters.. The search will allow to find in the records a place-name or summiter's name.
 
The diference with other GIS apps ,  Google Earth or Bing :

1 HimalViewer will offer consistent ordering and search engine for all mountain  features in a linear order - in particular: each summit  , mountain pass, valley , mountain face. The feature will have well-defined index from the mathematic concept of a node in the graph. In fact we shall consider two graphs -  the hydrological graph and the graph of mountain ridges. 
Practically it will allow to generate  automatically ( without user or admin input, but with a filter, cutting off some less important nodes ):

1. all valleys in a neighbourhood of a mountain
2. all mountains in the surrounding of a valley, and their mountai faces in the order - from your left to  your right ( looking up )

UNCLIMBED MOUNTAINS
For any geo-location - it will be easy to display all named and  unnamed  ( but important ) topographic objects.
Of course "importance" must be classified mathematically   as many secondary nodes must be cut off and not added to database.   The topographic criteria for valleys and rivers are to some extend defined in methods of computational hydrology , but for ridges, mountains and passes the hydrological rules have limited value ( only in case of cutting  off secondary ridges similar with secondary tributaries of rivers ),

For mountain summits  and passes  there is necessary to define other rules deducted from the international classificator of mountains
  http://www.theuiaa.org/mountaineering/mountain-classification/ .  
In this clasification  there are  two variables of "autonomy criterium " - minimal path distance dX  ( let us say 1000 meters ) , and minimal altitude difference  dY = 30 meters   , and consecutive passes or summits in the ridge  with smaller distance and altitude  difference are ignored.
It is obvious that for bigger dX and bigger dY the selection  will  choose less peaks and passes - so they can be considered  more "important"  This way we can add to the database many "important" summits, which are unnamed and unclimbed, but this makes them interesting for some climbers.
