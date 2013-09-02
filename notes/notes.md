
# Grab.js

### or:

## Gestures in Browsers	

Eran Weissenstern / eranws

presentation link: http://eranws.github.io/grab.js/notes


---
## About
###### who am I?


Primesense's apps team 

I was part of Primesense’s multidisciplinary UX group that design and develop gesture based control paradigms for Natural User Interfaces.

software engineering & design

// presale, UX 

---
## Intro

connecting stuff together, prototyping


--
##Reach UX
<iframe data-autoplay width="640" height="480" src="//www.youtube.com/embed/IVOPxYKhqZ0?rel=0" frameborder="0" allowfullscreen></iframe>

--
## puzzle

<iframe data-autoplay width="640" height="480" src="//www.youtube.com/embed/vVlANzCHL2Y?rel=0" frameborder="0" allowfullscreen></iframe>

---

## Popularity of 3D sensors

### Kinect hacks 
http://www.kinecthacks.com/top-10-best-kinect-hacks/

//	Q: who knows what 'kinect' is?


---
## Grab and The Missing 'Click'

### the problem:
once you dont have a surface to touch or click, deciding whether an action was made is much harder (for the programmer) and not fun (to the user)
--

## Grab and The Missing 'Click'
### 'Angry Birds' with Kinect

<iframe data-autoplay width="640" height="480" src="//www.youtube.com/embed/u_jmQY4QEBY?rel=0" frameborder="0" allowfullscreen></iframe>

did you notice anything missing?
--

## Grab and The Missing 'Click'

### Possible solutions:

* time click :(
* virtual screen (distance from screen/camera/shoulder?)
* tap detection (by speed)
* grab

--

## Grab

<iframe data-autoplay width="640" height="480" src="//www.youtube.com/embed/PurcczCZOO8?rel=0" frameborder="0" allowfullscreen></iframe>

--

<iframe  width="640" height="480" src="localhost:9093" frameborder="0"></iframe>

### tech demo

---

## the Stack

* hardware = sensor / camera & chip / (kinect). // Some background about depth, Ir, sensors
* driver - openni, "Depth Frame" (C)
* middleware - nite, recognition, "What is there?" (C++)
* server - websockets (C++) // this line enables multiplayer apps, since the app can run on another device
* client - app, game. In our case - browser (javascript)

//	Q: how many are programmers? what language?

--
## hardware
sensor / camera & chip / (kinect).
// Some background about depth, Ir, sensors
--
## driver
low-level openni, "Depth Frame"
(written in C)
### this 
--
## middleware
computer vision recognition, "What is there?" (C++)

* nite, 

--
## server - websockets (C++) // this line enables multiplayer apps, since the app can run on another device
--
## client - app, game. In our case - browser (javascript)



---

# < intermission >
## server install

--

install links

---


Browser - a Powerful Development tool
	Good seperation of worker and waiter, (client/server), cpu bound / io bound
	Runtime - C++, websockets, Browser - Javascript
	Recent advances in GPUs, internet standards (HTML5, WebGL) - Three.js

Why javascript? walkthrough
	inspect, (F12 / ctrl+shift+J - dev tools)
	hack (ESC - console)
	debug (breakpoint)
	* easy debugging example, famous website

event loop
each frame, the 'server' waits for a frame from the camera, process it, and sends out: 
	* hand position
	* grab state
	* (skeleton)

hack'n'slash (or: hotCoture)
	take working examples
	replace the wiring
	// exercise







---
## Links

* Presentation was made easy with: [Reveal.js](http://lab.hakim.se/reveal-js/)

---

# Thank You!
### Eran Weissenstern / eranws