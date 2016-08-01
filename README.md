# demo_mozilla_floating_logo
An Introduction to CSS3 Transitions by Software RVG  Posted by Rober Villar Garcia - Mozilla  MDN and  Mozilla Hispano contributor.  CSS3 Transitions are a presentational effect which allow property changes in CSS values, such as those that may be defined to occur on :hover or :focus, to occur smoothly over a specified duration – rather than happening instantaneously as is the normal behaviour.  Transition effects can be applied to a wide variety of CSS properties, including background-color, width, height, opacity, and many more. Keep reading for further details of supported properties.  At present the CSS3 Transitions module is at the working draft stage of development, and as such elements of the specification and syntax could still be liable to change. Although browser support is relatively widespread, for the time being you’ll need to use several vendor prefixes in your code for a cross-browser solution.  Here’s a basic example. The boxes below initially have an orange background, with the color set to change to green on :hover. For the first box no transition is specified, so the change occurs instantaneously. For the second box a transition with a duration of 5 seconds is specified, as such the change occurs smoothly over the given duration and automatically reverses when the mouse is moved off the element. 


<!DOCTYPE html>
+<html >
+  <head>
+    <meta charset="UTF-8">
+
+
+    <title>CodePen - demo mozilla CSS 3 floating logo  by Software RVG</title>
+    
+    
+    <link rel="stylesheet" href="//codepen.io/assets/reset/normalize.css">
+
+    
+        <style>
+      body {
+  min-height: 450px;
+  height: 100vh;
+  margin: 0;
+  background: -webkit-radial-gradient(circle, #0077ea, #1f4f96, #1b2949, #000000);
+  background: radial-gradient(circle, #0077ea, #1f4f96, #1b2949, #000000);
+}
+
+.stage {
+  height: 300px;
+  width: 500px;
+  margin: auto;
+  position: absolute;
+  top: 0;
+  right: 0;
+  bottom: 0;
+  left: 0;
+  -webkit-perspective: 9999px;
+          perspective: 9999px;
+  -webkit-transform-style: preserve-3d;
+          transform-style: preserve-3d;
+}
+
+.layer {
+  width: 100%;
+  height: 100%;
+  position: absolute;
+  -webkit-transform-style: preserve-3d;
+          transform-style: preserve-3d;
+  opacity: 0;
+  -webkit-animation: ಠ_ಠ 5s infinite alternate ease-in-out -7.5s, o_O 0.1s 1;
+          animation: ಠ_ಠ 5s infinite alternate ease-in-out -7.5s, o_O 0.1s 1;
+  -webkit-animation-fill-mode: forwards;
+          animation-fill-mode: forwards;
+  -webkit-transform: rotateY(40deg) rotateX(33deg) translateZ(0);
+          transform: rotateY(40deg) rotateX(33deg) translateZ(0);
+}
+
+.layer:after {
+  font: 200px/0.65 metabold;
+  content: 'mozilla \A \A  ';
+  white-space: pre;
+  text-align: center;
+  height: 100%;
+  width: 100%;
+  position: absolute;
+  top: 50px;
+  color: whitesmoke;
+  letter-spacing: -5px;
+  text-shadow: 4px 0 10px rgba(0, 0, 0, 0.13);
+}
+
+.layer:nth-child(1):after {
+  -webkit-transform: translateZ(0px);
+          transform: translateZ(0px);
+}
+
+.layer:nth-child(2):after {
+  -webkit-transform: translateZ(-2px);
+          transform: translateZ(-2px);
+}
+
+.layer:nth-child(3):after {
+  -webkit-transform: translateZ(-4px);
+          transform: translateZ(-4px);
+}
+
+.layer:nth-child(4):after {
+  -webkit-transform: translateZ(-6px);
+          transform: translateZ(-6px);
+}
+
+.layer:nth-child(5):after {
+  -webkit-transform: translateZ(-8px);
+          transform: translateZ(-8px);
+}
+
+.layer:nth-child(6):after {
+  -webkit-transform: translateZ(-10px);
+          transform: translateZ(-10px);
+}
+
+.layer:nth-child(7):after {
+  -webkit-transform: translateZ(-12px);
+          transform: translateZ(-12px);
+}
+
+.layer:nth-child(8):after {
+  -webkit-transform: translateZ(-14px);
+          transform: translateZ(-14px);
+}
+
+.layer:nth-child(9):after {
+  -webkit-transform: translateZ(-16px);
+          transform: translateZ(-16px);
+}
+
+.layer:nth-child(10):after {
+  -webkit-transform: translateZ(-18px);
+          transform: translateZ(-18px);
+}
+
+.layer:nth-child(11):after {
+  -webkit-transform: translateZ(-20px);
+          transform: translateZ(-20px);
+}
+
+.layer:nth-child(12):after {
+  -webkit-transform: translateZ(-22px);
+          transform: translateZ(-22px);
+}
+
+.layer:nth-child(13):after {
+  -webkit-transform: translateZ(-24px);
+          transform: translateZ(-24px);
+}
+
+.layer:nth-child(14):after {
+  -webkit-transform: translateZ(-26px);
+          transform: translateZ(-26px);
+}
+
+.layer:nth-child(15):after {
+  -webkit-transform: translateZ(-28px);
+          transform: translateZ(-28px);
+}
+
+.layer:nth-child(16):after {
+  -webkit-transform: translateZ(-30px);
+          transform: translateZ(-30px);
+}
+
+.layer:nth-child(17):after {
+  -webkit-transform: translateZ(-32px);
+          transform: translateZ(-32px);
+}
+
+.layer:nth-child(18):after {
+  -webkit-transform: translateZ(-34px);
+          transform: translateZ(-34px);
+}
+
+.layer:nth-child(19):after {
+  -webkit-transform: translateZ(-36px);
+          transform: translateZ(-36px);
+}
+
+.layer:nth-child(20):after {
+  -webkit-transform: translateZ(-38px);
+          transform: translateZ(-38px);
+}
+
+.layer:nth-child(n+10):after {
+  -webkit-text-stroke: 3px rgba(0, 0, 0, 0.25);
+}
+
+.layer:nth-child(n+11):after {
+  -webkit-text-stroke: 15px dodgerblue;
+  text-shadow: 3px 0 3px #ff4000, 2px 2px 2px #ff4000, 0 3px 3px #ff4000;
+}
+
+.layer:nth-child(n+12):after {
+  -webkit-text-stroke: 15px #0077ea;
+}
+
+.layer:last-child:after {
+  -webkit-text-stroke: 17px rgba(0, 0, 0, 0.1);
+}
+
+.layer:first-child:after {
+  color: #fff;
+  text-shadow: none;
+}
+
+@-webkit-keyframes ಠ_ಠ {
+  100% {
+    -webkit-transform: rotateY(-40deg) rotateX(-43deg);
+            transform: rotateY(-40deg) rotateX(-43deg);
+  }
+}
+
+@keyframes ಠ_ಠ {
+  100% {
+    -webkit-transform: rotateY(-40deg) rotateX(-43deg);
+            transform: rotateY(-40deg) rotateX(-43deg);
+  }
+}
+@-webkit-keyframes o_O {
+  100% {
+    opacity: 1;
+  }
+}
+@keyframes o_O {
+  100% {
+    opacity: 1;
+  }
+}
+.layer {
+  width: 100%;
+  height: 100%;
+  position: absolute;
+  -webkit-transform-style: preserve-3d;
+          transform-style: preserve-3d;
+  opacity: 0;
+  -webkit-animation: ಠ_ಠ 5s infinite alternate ease-in-out -7.5s, o_O 0.1s 1;
+          animation: ಠ_ಠ 5s infinite alternate ease-in-out -7.5s, o_O 0.1s 1;
+  -webkit-animation-fill-mode: forwards;
+          animation-fill-mode: forwards;
+  -webkit-transform: rotateY(40deg) rotateX(33deg) translateZ(0);
+          transform: rotateY(40deg) rotateX(33deg) translateZ(0);
+}
+    </style>
+
+    
+    
+    
+  </head>
+
+  <body translate="no" >
+
+     <meta charset="utf-8">
+    <meta name="generator" content="SOFTWARE RVG HTML Editor (www.software-rvg.com)">
+    
+  
+
+<div class="stage">
+  <div class="layer"></div>
+  <div class="layer"></div>
+  <div class="layer"></div>
+  <div class="layer"></div>
+  <div class="layer"></div>
+  <div class="layer"></div>
+  <div class="layer"></div>
+  <div class="layer"></div>
+  <div class="layer"></div>
+  <div class="layer"></div>
+  <div class="layer"></div>
+  <div class="layer"></div>
+  <div class="layer"></div>
+  <div class="layer"></div>
+  <div class="layer"></div>
+  <div class="layer"></div>
+  <div class="layer"></div>
+  <div class="layer"></div>
+  <div class="layer"></div>
+  <div class="layer"></div>
+</div>
+    
+    
+    
+    
+    
+    
+  </body>
+</html>
+ 
