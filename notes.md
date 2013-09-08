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
* ???

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

* 'time click'
* virtual screen (hand distance from body)
* tap detection (by speed)
* 'Grab'

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

--
## driver
### openni

* software low-level
* reads the "Depth Frame" to the PC

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

// this enables multiplayer apps, since the app can run on another device

--
## client

The topmost level. handles UI, graphics, sound, etc.

* application
* game
* In our case - a Browser

<p class="fragment">
well, almost topmost, since we develop on top of the browser
</p>

---

# < intermission >
## server install

--
## installation links

Currently supports windows 32bit only :(

* Install device drivers from openni <a href="http://www.openni.org/openni-sdk/?download=http://www.openni.org/wp-content/uploads/2013/07/OpenNI-Windows-x86-2.2.zip" target="_blank">website</a>.
* Download and Install <a href="https://www.google.com/intl/en/chrome/browser/" target="_blank">Chrome</a>
* Download and Run the server: <a href="https://dl.dropboxusercontent.com/u/3685114/grab.js/grabServer.zip">grabServer</a>

---
## Why Browser?
#### a Powerful Development tool

Seperation of client/server, cpu / io bound

Runtime - C++, websockets, Browser - Javascript

Advances in internet standards (HTML5, WebGL, websockets)

Example: [Three.js](http://chandlerprall.github.io/Physijs/examples/jenga.html)

Programming is easy and fast

// dynamic language javascript

--
## Web hacking 101?
#### a crash course / walkthrough

* press *F12* to open dev tools
* press *ESC* to open console

ctrl+shift+J directly to console

* type: "2+3", press enter

* inspect (magnifying glass)
* debug (breakpoint)


---
time to
## hack'n'slash

take working examples
replace the wiring

---
## Links

* Presentation was made easy with: [Reveal.js](http://lab.hakim.se/reveal-js/)

---

# Thank You!
### Eran Weissenstern / eranws