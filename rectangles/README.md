# Rectangles

The *area* of a single rectangle is equal to the it's *width* multiplied by it's *height*.

![no overlap](http://i.imgur.com/IefYcFj.png)

Computing the area of two rectangles is a little more challenging. They can either be separate and thus have their areas calculated individually. They can also intersect, in which case you calculate their individual areas, and subtract the area of the intersection.

![no overlap](http://i.imgur.com/6GzHGrh.png)

Once you get to 3 rectangles, there are multiple possibilities: no intersections, one intersection of two rectangles, two intersections of two rectangles, or one intersection of three rectangles (plus three intersections of just two rectangles).

At that point it becomes impractical to account for each situation individually but it might be possible. But what about 4 rectangles? 5 rectangles? N rectangles?

## Goals
Given any number of rectangles and their position/dimensions, find the area of the resultant overlapping (combined) shape.

## Input
Each input will have a number of lines. The first line is a positive integer that indicates the number of rectangles. The proceeding lines will describe the coordinates of each rectangle.

The co-ordinates describe opposite corners of N rectangles, in the form:
```
x1 y1 x2 y2
```
Where the rectangle's opposite corners are the co-ordinates `(x1, y1)` and `(x2, y2)`.
Note that the corners given will be the top-left and bottom-right co-ordinates, in that order.
Assume top-left is (0, 0).

## Output
You must print out the area (as a number) of the compound shape given. No units are necessary.

## Sample Input
```
3
0 1 3 3
2 2 6 4
1 0 3 5
```

## Sample Output
```
18
```


## Challenge
```
18
1.6 1.2 7.9 3.1
1.2 1.6 3.4 7.2
2.6 11.6 6.8 14.0
9.6 1.2 11.4 7.5
9.6 1.7 14.1 2.8
12.8 2.7 14.0 7.9
2.3 8.8 2.6 13.4
1.9 4.4 7.2 5.4
10.1 6.9 12.9 7.6
6.0 10.0 7.8 12.3
9.4 9.3 10.9 12.6
1.9 9.7 7.5 10.5
9.4 4.9 13.5 5.9
10.6 9.8 13.4 11.0
9.6 12.3 14.5 12.8
1.5 6.8 8.0 8.0
6.3 4.7 7.7 7.0
13.0 10.9 14.0 14.5
```