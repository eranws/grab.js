
# Grab.js

### or:

## Gestures in Browsers	

grab it here: http://eranws.github.io/grab.js/

<h3>Eran Weissenstern / eranws</h3>

---

## Intro - who am i
	apps/presale/UX - connecting stuff together, prototyping
	software engineering & design

--
##Reach UX
<iframe data-autoplay width="640" height="315" src="//www.youtube.com/embed/IVOPxYKhqZ0?rel=0" frameborder="0" allowfullscreen></iframe>

--
## puzzle

<iframe data-autoplay width="640" height="720" src="//www.youtube.com/embed/vVlANzCHL2Y?rel=0" frameborder="0" allowfullscreen></iframe>

---

## Popularity of 3D sensors

### Kinect hacks 
http://www.kinecthacks.com/top-10-best-kinect-hacks/

//	Q: who knows what 'kinect' is?


---
## Angry birds
### with kinect

<iframe data-autoplay width="640" height="315" src="//www.youtube.com/embed/u_jmQY4QEBY?rel=0" frameborder="0" allowfullscreen></iframe>

do you notice anything missing?
--
## Grab

<iframe data-autoplay width="640" height="315" src="//www.youtube.com/embed/PurcczCZOO8?rel=0" frameborder="0" allowfullscreen></iframe>

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