<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>¿Cómo estás?</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      margin-top: 100px;
    }
    #respuesta {
      display: none;
      margin-top: 30px;
    }
    img {
      max-width: 300px;
      margin-top: 20px;
    }
    button {
      padding: 10px 20px;
      margin: 10px;
      font-size: 16px;
      cursor: pointer;
    }
  </style>
</head>
<body>

  <h1>¿Cómo estás?</h1>

  <button onclick="mostrarRespuesta('feliz')">FELIZ</button>
  <button onclick="mostrarRespuesta('triste')">TRISTE</button>

  <div id="respuesta">
    <h2>Escucha esto</h2>
    <img id="albumImagen" src="" alt="Álbum">
  </div>

  <script>
    function mostrarRespuesta(estado) {
      const imagen = document.getElementById('albumImagen');
      const respuestaDiv = document.getElementById('respuesta');

      if (estado === 'feliz') {
        imagen.src = "https://media.giphy.com/media/l4FGzQdu1a2f1gWlS/giphy.gif"; // Canción Animal GIF
      } else if (estado === 'triste') {
        imagen.src = "https://media.giphy.com/media/l3q2K5jinAlChoCLS/giphy.gif"; // Bocanada GIF
      }

      respuestaDiv.style.display = 'block';
    }
  </script>

</body>
</html>
