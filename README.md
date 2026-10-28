# estaciones
<!DOCTYPE html>
<html lang="es">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Mi primera experiencia WebXR</title>
    <script src="https://aframe.io/releases/1.8.0/aframe.min.js"></script>
  </head>

  <body>
    <a-scene cursor="rayOrigin: mouse">
    
  <a-assets>
    <a-asset-item
      id="modelo-silla"
      src="./activos/silla.glb">
    </a-asset-item>
  </a-assets>

  <a-entity
    gltf-model="#modelo-silla"
    position="0 0 -3"
    rotation="0 0 0"
    scale="1 1 1">
  </a-entity>

  <a-sky color="#3cbff3"></a-sky>
      <a-plane
        position="0 0 -4"
        rotation="-90 0 0"
        width="30"
        height="30"
        color="#73e3f7">
    
   </a-plane>
      <a-box position="-1 0.5 -3" color="#fcfbfb"
      animation__click="property: rotation; from: 0 0 0; to: 0 360 0; dur: 1000; startEvents: click" animation__enter="property: scale; to: 1.2 1.2 1.2; dur: 200; startEvents: mouseenter" animation__leave="property: scale; to: 1 1 1; dur: 200; startEvents: mouseleave">
      </a-box>
        <a-sphere
        position="1 1.2 -4"
        radius="0.7"
        color="#cde213"
        animation="property: position;
                   to: 1 2 -4;
                   dir: alternate;
                   dur: 1800;
                   loop: true">
      </a-sphere>
      <a-text
        value="Mi primera experiencia WebXR"
        position="0 3 -5"
        align="center"
        color="#ffffff"
        width="6">
      </a-text>
         <a-camera position="0 1.6 0"></a-camera>

    
  </a-scene>
  </body>
</html>