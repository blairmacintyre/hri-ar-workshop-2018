<!-- .slide: data-background="resources/textures/logo-splash.png" data-transition="fade-in fade-out" -->
------

<!-- .slide: data-state="title" data-background="resources/textures/background-radial.jpeg" data-transition="fade-in fade-out" -->

<div class="talk-title">
	<h1>WebXR</h1>
	<h2>Bringing Mixed Reality to the Web</h2>
    <p class="talk-info">
		Mozilla <b>Emerging Technologies</b>
		<br><br>
		@blairmacintyre / bmacintyre@mozilla.com<br>
		@joshmarinacci / jmarinacci@mozilla.com<br>
		@trevorfsmith / trsmith@mozilla.com<br>
    </p>
</div>

<!-- NOTES -->

------
<!-- .slide: data-state="title" data-background="resources/textures/background-radial.jpeg" data-transition="fade-in fade-out" -->
<div style="background: rgba(32, 32, 32, 0.5);">

<h1> Hands on Workshop </h1> 
<p>Laptop for editing, view on <em>iOS</em> or <em>Android</em></p>
<p>Using our <em>WebXR Viewer</em> on iOS</p>
<p>Using Google's <em>WebARonARCore</em> on Android</p>
</div>
------

<!-- .slide:  data-background-video="resources/videos/shadow-movie4-720p.mov" -->

<div style="background: rgba(32, 32, 32, 0.5);">

<h1>Goal: Expand WebVR to include AR</h1>
<h2>Support full range of Mixed Reality</h2>

<p>A <i>webby</i> approach to MR that</p>

<ul>
<li> Supports AR and VR web apps in one API</li>
<li> Leverages platform capabilities efficiently</li>
<li> Supports geospatial AR, custom CV</li>
<li> Leaves door open for multi-augmentation</li>
<li> Respects people's privacy</li>
</ul>
<br>
AR/VR that keeps the user in control!

</div>

------

<!-- .slide: data-background="resources/textures/argonjs-github.png" data-background-position="top left" -->

<br>
<br>
<br>
<br>
<br>
<br>
<blockquote style="background: rgba(32, 32, 32, 0.5);">
  Inspired by WebVR 2.0  and <em>argon.js</em> / <em>Argon4</em> "reality" architecture <br>(<em>argon.js</em> project at <em>http://argonjs.io</em>)
</blockquote>

------
<!-- .slide: data-state="xrslide" data-transition="fade-out" -->

<div style="background: rgba(32, 32, 32, 0.5);">

<h1>What's where?</h1>

<p>WebXR API design and discussion: https://github.com/mozilla/webxr-api</p>
<p>WebXR polyfill and examples: https://github.com/mozilla/webxr-polyfill</p>
<p>WebXR iOS app: https://github.com/mozilla-mobile/webxr-ios</p>
<br>
Hosted on netlify.com in webxrexperiments.com
</div>

------

<!-- .slide: data-background="resources/textures/background-radial.jpeg" -->

# WebVR 1.1 is shipping

An open virtual reality platform with the advantages of **the Web**

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

------

<!-- .slide: data-background="media/img/aframe.jpg" -->
<div style="background: rgba(32, 32, 32, 0.5);">
    <h2>Frameworks like AFrame Integrate VR with Everything</h1>

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

<!-- .slide: data-background-video="resources/videos/arjs-hole.mp4" -->

<h2>Simple AR Has Been Possible, but Terrible</h2>
<p>WebRTC <span class="green">getUserMedia</span> + JS tracking</p><br>
<br>
<br><br>
<br>

<br>
<br>
<br>
<br>
<small><a href="https://github.com/jeromeetienne/AR.js">https://github.com/jeromeetienne/AR.js</a><br>
<a href="https://twitter.com/jerome_etienne/status/836754117964017664">https://twitter.com/jerome_etienne/status/836754117964017664</a></small>
