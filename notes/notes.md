# Grab.js

#### or:

## Gestures in Browsers	

Eran Weissenstern / eranws

// presentation link: http://eranws.github.io/grab.js/notes
// feel free to read it during the lecture

---
## About
###### who am I?

* Ex-Primesense's apps team
* Gesture based control
* Natural User Interfaces.
* Software engineering & design

// presale 
// games -> UX 

---

## Our Mission
#### What are we going to do

To create a simple and fun natural interaction:

* play/pause
* navigate and select 
* paint

// natural - easy to learn, no long explanation. only by seeing.

---
## Plan
#### How we are going to do it?

* WATCH - cool demos
* LEARN - javascript tricks
* HACK - connect stuff together, prototype

// hack - not from scratch. code re/abuse

--
##Reach UX
<iframe data-autoplay width="640" height="480" src="//www.youtube.com/embed/IVOPxYKhqZ0?rel=0" frameborder="0" allowfullscreen></iframe>

--
## puzzle

<iframe data-autoplay width="640" height="480" src="//www.youtube.com/embed/vVlANzCHL2Y?rel=0" frameborder="0" allowfullscreen></iframe>

---
## 'Angry Birds' with Kinect

<iframe data-autoplay width="640" height="480" src="//www.youtube.com/embed/u_jmQY4QEBY?rel=0" frameborder="0" allowfullscreen></iframe>

<p class="fragment">
did you notice anything missing?
</p>
					

--
## Grab and The Missing 'Click'

The Problem:
- no tactile feedback, surface to touch or click
- detecting an action is hard (for the programmer) and not fun (to the user)

// Kinect hacks 
// http://www.kinecthacks.com/top-10-best-kinect-hacks/

--

## Grab and The Missing 'Click'

Possible solutions:

* 'time click'  :(
* virtual screen (hand distance from screen/camera/shoulder?)
* tap detection (by speed)
* grab

--

## Grab
### tech demo

<iframe data-autoplay width="640" height="480" src="//www.youtube.com/embed/PurcczCZOO8?rel=0" frameborder="0" allowfullscreen></iframe>

* hand position real world (x,y,z in millimeters)
* grab - yes/no

// sample from primesense Labs

--
## Grab
### simple canvas test
<iframe  width="640" height="480" src="localhost:9093" frameborder="0"></iframe>


---
## What's between?
#### (the man and the machine)

The 'Stack':

* hardware
* driver
* middleware
* server
* client

//	Q: how many are programmers? what language?

--
## hardware
### Primesensor / 'Kinect'

* IR projector
* camera
* chip

//	Q: who knows what 'kinect' is?
// Some background about depth, Ir, sensors
// over USB to driver...

--
## driver
### openni

* software low-level
* reads the "Depth Frame" to the PC

// written in C
// freenect?

--
## middleware
### NiTE 
* Primesense's computer vision layer
* Scene analysis, segmentation, tracking
* #### Gesture recognition!

// written in C++

--
## server

on each frame, the server:
* reads data from the camera
* analyzes it to find interest points 
* sends data to the client over websockets 

// two threads
// this enables multiplayer apps, since the app can run on another device
// divide and conquer - easy to develop 

--
## client

The topmost level. handles UI, graphics 
* application
* game
* In our case - a Browser

// well, almost topmost.
// after the break we'll see why. (we develop on top of the browser)

---

# < intermission >
## server install

--

# TODO
installation links

---


## Browser - a Powerful Development tool
	Good seperation of worker and waiter, (client/server), cpu bound / io bound
	Runtime - C++, websockets, Browser - Javascript
	Recent advances in GPUs, internet standards (HTML5, WebGL) - Three.js
	http://acko.net/

	programming is easy and fast

// Why javascript? 
--

## Web hacking 101?
#### a crash course / walkthrough
	* F12 - open dev tools
	* console (ESC)
	* * ctrl+shift+J

	* inspect, ( / )

	* debug (breakpoint)
//ex - easy debugging example, famous website

---

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