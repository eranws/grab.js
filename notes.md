# Grab.js
### A HANDS-ON WORKSHOP FOR BUILDING HANDS-OFF EXPERIENCES


Eran Weissenstern / eranws

---
## About
###### who am I?

* Ex-Primesense's apps team
* Gesture based control
* Natural User Interfaces
* Software engineering & design

--
##Reach UX
<iframe data-autoplay width="640" height="480" src="//www.youtube.com/embed/IVOPxYKhqZ0?rel=0" frameborder="0" allowfullscreen></iframe>

---
## About
###### previous workshop picks

<iframe data-autoplay width="640" height="480" src="http://www.youtube.com/embed/x96QjirblXE?list=PL69B166657034606C&amp;hl=en_US" frameborder="0" allowfullscreen></iframe>

* Game oriented
* 'Unity3d' game engine for development

---

## Our Mission
#### Gestures in Browsers	

Create simple and fun gesture-based interaction

for example:
* play/pause
* navigate and select 
* paint

// natural - easy to learn, without explanation. only by seeing.

---
## Plan
#### How we are going to do it?

* WATCH - cool demos
* LEARN - javascript tricks
* HACK - connect stuff together, prototype

// hack - not from scratch. code re/abuse

--
## puzzled

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

* no tactile feedback, surface to touch or click
* detecting an action is hard (for the programmer)
* usage is not fun (to the user)

--

## Grab and The Missing 'Click'

Possible solutions:

* 'time click'  :(
* virtual screen (hand distance from screen/camera/shoulder)
* tap detection (by speed)
* grab

--

## Grab tech demo

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
## installation links

Currently supports windows 32bit only :(

* Install device drivers from openni <a href="http://www.openni.org/openni-sdk/" target="_blank">website</a>.   
* Download and Run the <a href = "https://dl.dropboxusercontent.com/u/3685114/grab.js/grabServer.zip">grabServer</a> - 


---
## Browser
#### a Powerful Development tool
Good seperation of worker and waiter, (client/server), cpu bound / io bound
Runtime - C++, websockets, Browser - Javascript
Recent advances in GPUs, internet standards (HTML5, WebGL) - Three.js
http://acko.net/

	programming is easy and fast

// dynamic language javascript

--
## Web hacking 101?
#### a crash course / walkthrough

1. press *F12* to open dev tools
2. press *ESC* to open console
3. type: "2+3", press enter

* inspect, (magnifying glass)
* debug (breakpoint)

//ex - easy debugging example, famous website
// ctrl+shift+J directly to console

---
time to
## hack'n'slash
#### (or: hot Coture)

take working examples
replace the wiring

// TODO: exercise. (youtube/your favorite website)
// if you want to start something from scratch, now it's the time.

---
## Links

* Presentation was made easy with: [Reveal.js](http://lab.hakim.se/reveal-js/)

---

# Thank You!
### Eran Weissenstern / eranws