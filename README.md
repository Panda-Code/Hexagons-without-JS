Creating hexagon
======================

This simple html/css style creates a simple yet functional hexagon.
It uses the new CSS element: -webkit-clip-path to create the clipping effect.

CSS:
.hexagon {
	margin: 0 auto;
	width:225px;
	height: 200px;
	-webkit-clip-path: polygon(25% 0, 75% 0, 100% 50%, 75% 100%, 25% 100%, 0 50%);
	background:black;
	overflow:hidden;
	display:inline-block;
}

Everything here can be easily modified to suit your needs.
You can add and remove the polygons, to do more shapes.


Polygon position:
(25%  0,)
  x   y
  
  The position of the polygons follow the clock, so Top right, top left, bottom left, bottom right.
  
  in my case, since it has 2 more edges to count, top right, top left, center left, bottom left, bottom right, center right.
-webkit-clip-path: polygon(25% 0, 75% 0, 100% 50%, 75% 100%, 25% 100%, 0 50%);
