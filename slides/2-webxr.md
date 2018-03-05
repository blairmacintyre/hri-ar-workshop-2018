<!-- .slide: data-background="resources/textures/fast-for-good.png" data-background-size="contain" data-background-repeat="no-repeat" -->

<!-- NOTES -->
I'm at mozilla, why?


------
<!-- .slide: data-background="resources/textures/argonjs-github.png" data-background-size="contain" data-background-repeat="no-repeat" -->

------
<!-- .slide: data-background="resources/textures/background-radial.jpeg"  -->

<div class="talk-title">
	<h1>Making the Hidden Visible<br>in a Safe and Secure Way<br>in Highly Distributed Applications</h1>
    <p class="talk-info">
		<b><a href="http://blairmacintyre.me">Blair MacIntyre</a></b>
		<br>
		Principal Research Scientist, Mozilla <br>
		Professor, School of Interactive Computing, Georgia Tech<br>
		@blairmacintyre / bmacintyre@mozilla.com / blair@cc.gatech.edu <br>
    </p>
</div>
------
<!-- .slide: data-background="resources/textures/background-radial.jpeg" -->

# WebXR 

An open platform for VR and AR with the advantages of **the Web**

<div class="captioned-image-row">
  <div>
    <img class="plain" data-src="media/img/web-is-open.png">
    <i>Open</i>
  </div>
  <div>
    <img class="plain" data-src="media/img/web-is-connected.png">
    <i>Connected</i>
  </div>
  <div>
    <img class="plain" data-src="media/img/web-is-instant.png">
    <i>Instant</i>
  </div>
</div>

<!-- NOTES -->
Open, accessible, and secure
“Just a URL”
Security and privacy in browser, not app
Every device has a browser
Integrates with existing web services, content, and development team
No app store gatekeepers or one-off IT infrastructure
Immediate publishing/iteration without app store review



WebVR is...virtual reality in the browser, powered by the Internet

Open:
- Anyone can publish
- Open source culture with open standards

Connected:
- Traverse worlds

Instant:
- Click a link on Twitter or Weibo, immediate VR experiences
- No installs
- Imagine for long tail experiences: shopping & personal spaces
- Great for long tail bite-sized experiences

Transition:
- Web has advantages that make it the best platform for the people
- Need to act to make it reality, can't wait for VR to bake and crystallize
- Get involved

------

<!-- .slide: data-background="resources/textures/background-radial.jpeg" -->

<img src="resources/textures/HDP-eyes.png" height="300">
<img src="resources/textures/volcano-fever.png" height="300">


<!-- NOTES -->

------
<!-- .slide: data-background="resources/textures/background-radial.jpeg" -->

# Let's start with VR

<div class="image-row">
  <div><img class="plain" data-src="media/img/google-cardboard.png"></div>
  <div><img class="plain" data-src="media/img/google-daydream.png"></div>
  <div><img class="plain" data-src="media/img/samsung-gearvr.png"></div>
</div>

<div class="image-row">
  <div><img class="plain" data-src="media/img/oculus-rift.png"></div>
  <div><img class="plain" data-src="media/img/playstation-vr.png"></div>
  <div><img class="plain" data-src="media/img/htc-vive.png"></div>
</div>

<!-- NOTES -->
- Backed by the largest corporations in the world, everyone wants in
- Range from cheap to expensive, tethered and untethered, controllers, tracking
- HTC Vive with Steam currently offers the most compelling experiences, but never know
- See a lot of different devices, systems, platforms competing against each other...


------

<!-- .slide: data-background="resources/textures/background-radial.jpeg" -->

<img class="plain" class="stretch" data-src="media/img/webvr.png">

Browser APIs that enable WebGL rendering to headsets and access to VR
sensors

https://immersive-web.github.io/webvr/

<!-- NOTES -->
API:
- Optimized rendering path to headsets
- Access position and rotation (pose) data

History:
- Initial WebVR API by Mozilla
- Working W3C community group
- Mozilla, Google, Samsung, Microsoft, community currently iterating WebVR 1.0 API

Not just a specification, it's implemented...

------


<!-- .slide: data-background="resources/textures/background-radial.jpeg" -->

https://webvr.rocks

<div class="captioned-image-row small">
  <div>
    <img class="plain" data-src="media/img/firefox-nightly.png">
    <i>Firefox Nightly</i>
  </div>
  <div>
    <img class="plain" data-src="media/img/edge.jpg">
    <i>Microsoft Edge</i>
  </div>
  <div>
    <img class="plain" data-src="media/img/chromium.png">
    <i>Chromium</i>
  </div>
</div>

<div class="captioned-image-row small">
  <div>
    <img class="plain" data-src="media/img/chrome.jpg">
    <i>Chrome for Android</i>
  </div>
  <div>
    <img class="plain" data-src="media/img/carmel.jpg">
    <i>Oculus Carmel</i>
  </div>
  <div>
    <img class="plain" data-src="media/img/samsung-browser.png">
    <i>Samsung Internet</i>
  </div>
  <div>
    <img class="plain" data-src="media/img/google-cardboard.png">
    <i>Mobile Polyfill</i>
  </div>
</div>

<!-- NOTES -->
- Firefox + Chrome WebVR 1.0 hits release channels by early 2017
- Currently behind Nightly, custom builds, and flags
- Mobile Polyfill: use device motion / orientation sensors to polyfill on smartphones
- With all the browsers behind it...

------
<!-- .slide: data-background="resources/textures/caniuse.png" data-background-size="contain" data-background-repeat="no-repeat" -->
<blockquote style="background: rgba(32, 32, 32, 0.5);">
WebVR support available on all platforms from at least one major browser (Vive, Rift, Daydream, WindowsMR, etc)
</blockquote>

<br>
<br>
<br>
<br>
<br>
<br>

<br>
<br>
<br>
<br>
<br>
<br>

------


<!-- .slide: data-background="media/img/aframe.jpg" -->
<div style="background: rgba(32, 32, 32, 0.5);">
    <h2>Frameworks like AFrame Integrate VR with Web Tools</h1>

  <div class="captioned-image-row">
    <div>
      <img class="plain" data-src="media/img/d3.png">
      <i>d3.js</i>
    </div>
    <div>
      <img class="plain" data-src="media/img/vue.png">
      <i>Vue.js</i>
    </div>
    <div>
      <img class="plain" data-src="media/img/react.png">
      <i>React</i>
    </div>
    <div>
      <img class="plain" data-src="media/img/redux.png">
      <i>Redux</i>
    </div>
    <div>
      <img class="plain" data-src="media/img/jquery.png">
      <i>jQuery</i>
    </div>
    <div>
      <img class="plain" data-src="media/img/angular.png">
      <i>Angular</i>
    </div>
  </div>
</div>
---
<!-- .slide: data-background="media/img/cadavr.gif" -->

# Education - *CadaVR*

@drryanjames

---
<!-- .slide: data-background="media/img/syria.gif" -->

# Journalism - *Fear of the Sky*

Amnesty International UK

---

<!-- .slide: data-background="media/img/mars.jpg" -->

# Journalism - *Journey to Mars*

The Washington Post

---

<!-- .slide: data-background="media/img/adit.gif" -->

# Data Visualization - *Adit*

@datatitian

---

<!-- .slide: data-background="media/img/a-blast.gif" -->

# Gaming - *A-Blast*

@mozillavr

---

<!-- .slide: data-background="media/img/math.gif" -->

# Mathematics - *MathworldVR*

@sleighdogs

------

<!-- .slide: data-background="media/img/scene-collage.jpg" -->

------
<!-- .slide: data-background="resources/textures/background-radial.jpeg" -->

<div class="captioned-image-row">
  <div>
    <img class="plain" data-src="resources/textures/arShadows-circ.png">
    <i>WebXR adds AR to WebVR</i>
  </div>
</div>

------

<!-- .slide: data-background="resources/textures/background-radial.jpeg" -->

<div class="image-row">
  <div><img class="plain" data-src="resources/textures/ardisplay-hololens-circ.png"></div>
  <div><img class="plain" data-src="resources/textures/ardisplay-daqri-circ.png"></div>
  <div><img class="plain" data-src="resources/textures/ardisplay-odg-circ.png"></div>
  <div><img class="plain" data-src="resources/textures/ardisplay-meta-circ.png"></div>
</div>
<div class="image-row">
  <div><img class="plain" data-src="resources/textures/ardisplay-vuzix-circ.png"></div>
  <div><img class="plain" data-src="resources/textures/lenovo-phab2-lowes-circ.png"></div>
  <div><img class="plain" data-src="resources/textures/iphone7plus-circ.png"></div>
  <div><img class="plain" data-src="resources/textures/ardisplay-magic-leap-goggles-circ.png"></div>

<!-- NOTES -->

------
<!-- .slide: data-background-video="resources/videos/shadow-movie4-720p.mov" -->

<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<blockquote style="background: rgba(32, 32, 32, 0.5);">
    It will finally be possible to mix media with a <br>
    person's perception of the world<br>
    <span class="green">_registered in 3D_</span>
    <span class="green">, _in real-time_</span>,<br>
    <span>_in a commodity web browser_</span>
</blockquote>


------

<!-- .slide: data-background-video="resources/videos/arjs-hole.mp4" -->

<h2>Folks Have Done Simple AR on the Web</h2>
<p>WebRTC <span class="green">getUserMedia</span> + JS tracking</p><br>
<br>
<br><br>
<br>

<br>
<br>
<br>
<br>
<br>
<br>
<small><a href="https://github.com/jeromeetienne/AR.js">https://github.com/jeromeetienne/AR.js</a><br>
<a href="https://twitter.com/jerome_etienne/status/836754117964017664">https://twitter.com/jerome_etienne/status/836754117964017664</a></small>

------

<!-- .slide: data-background="resources/textures/levelhead.png" -->

<br>
<br>
<br>
<br>
<br>
<br>
<h1>This Simple Approach is Insufficient</h1>
<blockquote style="background: rgba(32, 32, 32, 0.5);">
    <span><h3>Very Little World Knowledge,<br>
    Tightly Coupled to Specific Technology,<br>
    Doesn't Leverage Platform Capabilties</h3></span>
</blockquote>

<br>
<p><small>Julian Oliver "Levelhead" 2008</small></p>



------

<!-- .slide: data-background-video="resources/videos/tango-cat-trim.m4v" -->

<h2>Platform-Specific Sensing is Diverse</h2>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<blockquote style="background: rgba(32, 32, 32, 0.5);">
    <span>SLAM capabilities in Google Tango, Microsoft Hololens, Facebook Camera, Wikitude, Kudan, etc.</a>
    </span>
</blockquote>

------

<!-- .slide: data-background-video="resources/videos/hololens-trim-noaudio.mp4" -->

<h2>Display Tech Also Diverse: See-through vs Video-Mixed vs ...</h2>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>

------

<!-- .slide: data-background="resources/textures/home-HoloLens-crop.jpg" -->

<div style="background: rgba(32, 32, 32, 0.5);">

<h1>AR Tech in the Browser, AR Apps Inside</h1>

<p>A "webby" approach to AR must</p>

<ul>
<li> Support platform independent web apps</li>
<li> Leverage platform capabilities efficiently</li>
<li> Enable user privacy</li>
</ul>

<p>http://blairmacintyre.me/2017/05/20/its-not-webar-yet/</p>

</div>
------

<!-- .slide: data-background="resources/textures/background-radial.jpeg" -->


<h2>Adding AR to WebXR this Year</h1>
<p>Build on Advanced Web Tech: WebVR, Servo, WebAssembly, ...</p>
<p>Leverage Native Tech: ARKit, ARCore, various HMDs, Vision SDKs, ...</p>
<p>Enable Web-Based AR Tech: computer vision, sensor fusion, geospatial data, ...</p>

------
<!-- .slide: data-background="resources/textures/servo.org.png" data-background-size="contain" data-background-repeat="no-repeat" -->


------
<!-- .slide: data-background-video="resources/videos/servo-page-3d.mp4" -->
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<blockquote style="background: rgba(32, 32, 32, 0.5);">
<h3>Experiment with XR capabilities in Servo</h3>
<em>2D DOM content in 3D, XR Browser, XR extensions for CV, ... </em>
</blockquote>
------
<!-- .slide: data-background-video="resources/videos/playcanvas-scene-1080p.mp4" -->
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<blockquote style="background: rgba(32, 32, 32, 0.5);">
<h3>High Performance Graphics with WebGL2</h3>
<em>Playcanvas demo, iMac, Firefox</em>
</blockquote>
------
<!-- .slide: data-background="resources/textures/social-mr-blog-v2-min.gif" -->
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<blockquote style="background: rgba(32, 32, 32, 0.5);">
<h3>Social and Multiuser</h3>
<em>Services to support drop-in multi-user social experiences<br>with voice/avatars/etc</em>
</blockquote>

------
<!-- .slide: data-background="resources/textures/iss-ar.png" -->
<blockquote style="background: rgba(32, 32, 32, 0.5);">
<h2>Web Ecosystem is Rich and Diverse</h2>
<p>Many tools, from the simple to the elaborate</p>
<p>Mashups may suggest new ways of creating 3D!</p>
</blockquote>
<br>
<br>
<br>
<br>
<br>
<blockquote style="background: rgba(32, 32, 32, 0.5);">
    <span><em>ISS Maintenance using PRIDE w/ Traclabs</em></span>
</blockquote>


------
<!-- .slide: data-state="xrslide vrslide" -->

## This Presentation is Running in our WebXR Viewer</h2>
<p><em>on an iPhone</em></p>
<p>Using webxr.js + reveal.js + three.js</p>


------
<!-- .slide: data-state="xrslide vrslide boombox" style="text-align: left; top: 0px;" -->

<h2>VR</h2>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>

------

<!-- .slide: data-state="xrslide arslide boombox" style="text-align: left;" -->

<h2>AR</h2>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>

------
<!-- .slide: data-state="xrslide arslide 3deffects boombox" style="text-align: left;" -->

<h2>Arbitrary 3D Effects (e.g., bloomv + film effect)</h2>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
