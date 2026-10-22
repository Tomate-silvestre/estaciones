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
     <a-sky color="#f10ede"></a-sky>
      <a-plane
        position="0 0 -4"
        rotation="-90 0 0"
        width="30"
        height="30"
        color="#ec0c0c">
      </a-plane>
      <a-box position="-1 0.5 -3" color="#a51285"
animation__click="property: rotation; from: 0 0 0; to: 0 360 0; dur: 1000; startEvents: click">
      </a-box>
        <a-sphere
        position="1 1.2 -4"
        radius="0.7"
        color="#1a9c0f"
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