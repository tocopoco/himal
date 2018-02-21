# himal
3D visualisation of Himalaya

HimalViewer

The web app will  use Javascript , the open source programs CesiumJS and Nodejs server.

HimalViewer will help mountaineering and trekking societies to create archives of mountaineering in  any   mountain region on Earth, but the task starts in Western Himalasya , which is a relatively unexplored and poorly described region between Kashmir and Tibet, moreover with poor cartographic sources.  The program will use the open source CesiumJS, which  supports Digital Earth Model delivered by Google Earth and by Bing API,  and many other DEM models.

Target groups :   
- local population inhabiting mountain areas
- mountain guides
- mountaineers
- trekkers   
- mountaineering clubs and high-mountain magazines, their mountaineering archives
- ethnographers , in particular IALS ( Interernational Association of Ladakhi Studies )

 Main features:
 -  3D visualization of the terrain
 -  Geo referencing
 -  Reverse referencing of mountain photographs ( also historical ones )
 -  Search capabilities - alphabetical,  GPS ,  topographical ordering  along valleys and ridges
 -  Database  of mountaineering achievements, with personal index of ascents.
 -  Possibility to add ( crowd-sourcing ) names to the topographic objects , climbing routes and descriptions of ascents in the mountaineering layer 
 -  Possibility to add ( crowd-sourcing ) landmarks and descriptions of trails to the the cultural layer , in the format of KML/KMZ files.

DETAILS OF FEATURES :
HimalViewer will offer consistent ordering and a search engine for all mountain features in a linear order - in particular: each summit, mountain pass, valley, and mountain face. The feature will have well-defined index from the mathematical concept of a node in the graph. In fact we shall consider two graphs - the  graph of valleys and the graph of mountain ridges. The ordering is well-know concept in hydrology (see: Horton-Strahler method in:  http://hydrology.usu.edu/dtarb/hp91.pdf) but it seems that it has not been used to create an upside-down model of mountain ridges. If we change in the elevation model all elevations from positive to negative with the same absolute value - we notice that all ridges become "rivers", but many of them will flow to "pits" which in the positive mode are summits of mountains. The main problem will be here to decide which pits should be removed (as not autonomous = not important ), and which should remain in the graph - for instance the deepest pit which is Mt. Everest. The problem can be illustrated by the smaller southern summit of Mt Everest . Nobody consider it as an autonomous peak - as it might be identified as the second highest peak in the world instead of K2 in Karakorum. Therefore some rules must be used to remove "non-autonomous"  peaks from the graph and from the database, and also to leave only the deepest pass between two consecutive peaks in the ridge.

Some mathematical ( and heuristic ) criteria for an "autonomous summit" are introduced by the UIAA  ( International Union of Alpinist Associations ) - http://www.theuiaa.org/mountaineering/mountain-classification/ and of course only mathematical rules for topographic features can be used here , as all other (historical etc.)  are subjective and cannot be computed from the DEM., Using the mathematical rules the program will add automatically  to the graph  all  "autonomous" summits and passes, without paying attention if they are named or unnamed, climbed or unclimbed - so the outsourcing in their case will help to connect the summits ( and the passes ) with their names and mountasineering records.

Collecting the names from  mountaineering archives I will try to consider  also traditional names  ( alias ) in local languages and dialects,  in the crowd-sourcing in social media popular in native communities .It will be possible to add local names in non-European characters used by Hindi , Urdu , Nepali and Tibetan – and convert them by using standard romanisation ( transliteration ) , what can be useful for ethnographers and library catalog search.

The Cesium logo will be included  with the link https://cesiumjs.org into the program , according with their wish expressed in their Apache 2 license, and similar information about all other open sources and theoretical methods used in the project.
