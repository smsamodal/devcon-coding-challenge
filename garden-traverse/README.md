# Garden Traverse

![maze](http://www.livingasean.com/wp-content/uploads/2016/11/fea-1.jpg)

One of the properties that **onerent** manages includes a number of garden mazes. Help the property manager solve the garden maze by writing a program to solve mazes.

A maze will have all of it's walls are connected to each other. Take this example maze segment.
```
# # ### #
# #
# ### G #
#   # G #
# G # G #
# G   G #
# GGGGG #
#       #
#########
```
See how the wall drawn with Gs isn't connected to any other walls? That's called a floating wall. Our mazes contains no floating walls - ie. there are no loops in the maze.
Formal Inputs and Outputs

## Input

You will be given two numbers W and H. After that you will be given a textual ASCII grid, `W` wide and `H` tall, of walls `#` and `spaces`. In the maze there will be exactly one letter ``S`` and exactly one letter `E`. There will be no spaces leading to the outside of the maze - ie. it will be fully walled in.

## Output

To help guide our property manager. The program must print out the maze. Within the maze there should be a path drawn with askerisks `*` leading from the letter `S` to the letter `E`. Try to minimise the length of the path if possible - don't just fill all of the spaces with *!

## Sample Input and output

### Sample Input
sample.txt
```
15 15
###############
#S        #   #
### ### ### # #
#   #   #   # #
# ##### ##### #
#     #   #   #
# ### # ### ###
# #   # #   # #
# # ### # ### #
# # # # # #   #
### # # # # # #
#   #   # # # #
# ####### # # #
#           #E#
###############
```

### Sample Output
```
###############
#S**      #   #
###*### ### # #
#***#   #   # #
#*##### ##### #
#*****#   #   #
# ###*# ### ###
# #***# #   # #
# #*### # ### #
# #*# # # #***#
###*# # # #*#*#
#***#   # #*#*#
#*####### #*#*#
#***********#E#
###############
```

A separate file `challenge.txt` contains a larger map as an additional challenge input.
