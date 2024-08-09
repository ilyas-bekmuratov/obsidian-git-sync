#idea 
#animation
#gamedesign 

[A simple procedural animation technique](https://www.youtube.com/@argonautcode)

Chain method
1) create an anchor point
2) create a point somewhere and use a distant constraint that moves the point after the anchor of it's moved

now you have a worm

3) now each point has a parameter of size of the body segment
4) using the radius and direction of the body segment and parametric equations lets you mark left and right
5) now make an angular constraints for the angles between 3 consecutive points 

now you have a snake

6) side fins can be represented by rotated ellipsis
7) set their position relative to some body segments using similar parametric equations as above
8) set their rotation relative to the segments in front of the fins so it looks less stiff
9) dorsal and tail fins along the spine rely on the sum of the angular differences between each segment to get the value that shows how curved it is
10) for the fin on the spine it matches the curvature, and the offset (in the middle of the fin) is proportional to this curvature %
11) for the tail fin the back of the curve is offset

now you have a fish

12) draw circles at each joint and you can find the position of the hand using kinematics parametric equations
13) however, to find out the position of each joint if the hand must be on a certain point you have to use inverse kinematics, or an approximation FaBRIK - forward and backward reaching inverse kinematics
14) start from the anchor of the limb and pull its hand - second anchor - towards the target point so the arm stretches towards it
15) pull the arm back towards the bodypoint using the first anchor again
16) repeat until you have a configuration where your arm is on the target and your joint is on the body where it should be, or until your hand is stretched out in a single line (or as close as parametric equations of the joints allow)
17) now, imagine this fabric chain attached to a body
18) as the body moves back and forth, but the legs stays on the same place, fabric stretches
19) now mark a position relative to the body - next step
20) as the body moves, the limb lags behind this relative position and when it gets a certain distance apart - it makes a step

now you have a dipshit lizard
