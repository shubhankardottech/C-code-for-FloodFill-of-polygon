# Flood-Fill Algorithm:

It is a recursive function to replace previous color 'oldcolor' at  '(x, y)' and all  surrounding pixels of (x, y) with new color 'newcolor' and
floodfill(x, y, newcolor, oldcolor)

1) If x or y is outside the screen, then
   return.
   
2) If color of getpixel(x, y) is same as
   oldcolor, then 
   
3) Recur for top, bottom, right and left.
    floodFill(x+1, y, newcolor, oldcolor);
    floodFill(x-1, y, newcolor, oldcolor);
    floodFill(x, y+1, newcolor, oldcolor);
    floodFill(x, y-1, newcolor, oldcolor); 

Although this algorithm has some drawbacks:
1. It is very slow algorithm
2. It may fail for large polygons
3. the initial pixel require more knowledge about surrounding pixels.
