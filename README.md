# Procedural Jellyfish
<img width="800px" alt="Jellyfish Animation" src="assets/jellyfish.gif">

## Bell
The bell was created by revolving a bent line around the y-axis, using noise to vary the surface, and then extruding to add volume.
<br><br>
<img width="800px" alt="Jellyfish Bell" src="/assets/bellFinished.png">

## Arms
The arms were created by adding noise in the z-direction of a grid in the x-y plane and then twisting the grid. Vellum constraints were added to make the arms stretch and contract during animation as if the jellyfish were moving through water. After creating one arm, the copy node was used to place five evenly spaced arms around the center of the bell.
<br><br>
<img width="800px" alt="Jellyfish Arms" src="/assets/armsFinished.png">

## Veins
The veins were created by remeshing the bell shape and choosing start and end points for a shortest path node to create paths from single points at the top of the bell to multiple points along the curve of the bell. The veins were then animated to match the bell's motion using a point deform node.
<br><br>
<img width="800px" alt="Jellyfish Veins" src="/assets/veinsFinishedSide.png">
<img width="800px" alt="Jellyfish Veins" src="/assets/veinsFinished.png">

## Organs
The organs were created by bending a line and adding a slightly bumpy volume through a sweep node and then copying in a circle around the center of the bell.
<br><br>
<img width="800px" alt="Jellyfish Organs" src="/assets/organsFinished.png">

## Tentacles
The tentacles were created by getting a scatter of points from a torus of roughly the same size as the bell and then constraining those points to the bottom points of the bell. This was done using point deform nodes and ray nodes. The tentacles were animated using vellum constraints and a wind force to make them look like they would be swaying in the water as the jellyfish moves.
<br><br>
<img width="800px" alt="Jellyfish Tentacles" src="/assets/tentaclesFinished.png">
