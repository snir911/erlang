This is Autonomous Intersection Manager written in Erlang

Each car is autonomous it communicates with the road manager to receive
cars which are on the same lane and then interacts with them to prevent collision.
Before entering the intersection a car is asking the intersection manager to
allocate for itself (the car) a collision-free route (to its estimated arrival time).
In the intersection, each car enters the intersection only with approval.

Result: Cars are crossing the intersection simultaneously without collisions

#The video shows running example on:
 -4 beagleboards (each is responsible for one road part and the cars on that part)
 -1 laptop which runs the display module and the intersection module
 -all connected through switch

#Cars processes are being killed and load when crossing between the devices
 (between the laptop and the beagleBoards)

#Also tested on Intel Edison with wifi interface
