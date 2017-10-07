# Field Operation Specialist Route

**onerent** employs `Field Operations Specialists` to inspect and qualify homes before they can be listed as available for renting.

You must plan a route for the field operation specialist to visit each of 26 houses and then return home. The requirement is to get a good solution. Not the guaranteed optimal one.

## Input
Houses are `x` `y` points, and the distance between them is the floor of the pythagoran distance.
Home is the first at: `0 0`
```
  0   0
689 291
801 724
388 143
143 832
485 484
627 231
610 311
549 990
220  28
 66 496
693 988
597 372
753 222
885 639
897 594
482 635
379 490
923 781
352 867
834 713
133 344
835 949
667 695
956 850
535 170
583 406
```

## Output
```
total distance of itinerary:  14193 pythagores
route order: 0 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 0
```

Or a much shorter route if you can generate a better one

### Tips
* This is a well known problem called The Travelling Salesman.
* Genetic algorithms are considered a good fit for time constrained solutions.
* Clustering and then travelling among clusters can reduce the permutation space significantly. Similarly, finding close pairs and/or triplets creates good candidate clusters.