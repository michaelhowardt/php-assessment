<h1>Assesment</h1>

<h2>Scenario</h2>
We need a drone delivery system that sends packages between clients. \
You can generate 10 clients upon program startup but note that their locations will change.


<h2>Orders</h2>

<h3>The properties of an order are the following:</h3>

* id - Auto Increment Id managed within your application
* client's name
* client's location
* client's contact number 1
* client's contact number 2
* client's contact number 3

<h3>The properties of a drone are the following:</h3>

* id - Auto increment ID
* drone name
* drone location (latitude, longitude)
* drone contact number 1
* drone contact number 2
* drone contact number 3

<h3>Drones</h3>
There are 10 drones starting in the centre of the map.

<h3>Allocation Rules</h3>

Orders should be randomly placed every 30 seconds with randomized client locations.

So the rules for allocation are the following:
* Order is allocated to a drone if a drone is not currently busy with another order
* Order is allocated to the closest available drone first and then the 2nd and so forth.
* If no drones are available a retry policy should be followed.

<h3>Process of an order</h3>

* Allocate drone to Order 
* Deliver to Client (Time to deliver from collect: random between 1 and 10 plus the distance in seconds)

<h3>Front End Requirements:</h3>
* Basic UI map (1000 by 1000 units) rectangle
* View order information
* View Current Drone and state
    * What order is he busy with
    * Which step of the process is he busy with

<h3>Basic Tech Requirements</h3>

* An RDBMS Database
* Code should be easy to understand
* Bonus if RESTful framework is used
* Bonus if view can update components without refreshing
* Git practices will also be reviewed so make sure to make regular commits etc.
