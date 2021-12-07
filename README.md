# VR-Project
//Some code I used to practice in making a VR game.
VR project

<html>
 <head>
   <script src="https://aframe.io/releases/1.0.4/aframe.min.js"></script>
 </head>
 <body>
   <a-scene>
     <a-assets>
       <img id="sky" src="mountains1.jpg">
       <img id="grass" src="grass1.jpg">
       <a-asset-item
         id="codey"
         src="codey.gltf"></a-asset-item>
     </a-assets>
    
     <a-sky src="#sky"></a-sky>
     <a-plane
       src="#grass"
       rotation="-90 0 0"
       width="20"
       height="20"></a-plane>
     <a-entity
       text="value: Welcome!; color: #FFD500; align: center"
       position="0 3 -4"
       scale="6 6 6"
       animation="property: object3D.position.y;
         to: 3.2;
         dir: alternate;
         dur: 2000;
         loop: true"></a-entity> 
     <a-entity
       gltf-model="#codey"
       position="0 2 -4"
       scale="0.5 0.5 0.5"
       animation="property: object3D.position.y;
         to: 2.2;
         dir: alternate;
         dur: 2000;
         loop: true"></a-entity>
     <!-- Add the code below: -->
     <a-light
     type="point"
 intensity="2"
 position="2 4 4"></a-light>
 
   </a-scene>
 </body>
</html>
