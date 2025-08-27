<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Gymkhana Interactiva · Ribera del Fresno</title>
  <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" />
  <style>
    html, body { height: 100%; margin: 0; }
    #map { height: 100%; width: 100%; }
    .legend {
      position: absolute;
      bottom: 12px; left: 12px;
      background: rgba(255,255,255,0.9);
      padding: 10px 12px; border-radius: 12px;
      font: 14px/1.3 system-ui;
      box-shadow: 0 2px 10px rgba(0,0,0,0.12);
    }
    input.answer {
      width: 100%;
      margin: 4px 0;
      padding: 4px;
    }
    button.check {
      background: #0066cc; color: white;
      border: none; padding: 6px 12px;
      border-radius: 6px; cursor: pointer;
    }
    button.check:hover { background: #004c99; }
  </style>
</head>
<body>
  <div id="map"></div>
  <div class="legend">
    <h3>Gymkhana Ribera del Fresno</h3>
    <p>Responde a las preguntas en cada punto para desbloquear el siguiente 📍</p>
  </div>

  <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"></script>
  <script>
    const CENTER = [38.55119, -6.23892];

    const map = L.map('map', {
      center: CENTER,
      zoom: 15
    });

    L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
      maxZoom: 20,
      attribution: '&copy; OpenStreetMap contrib.'
    }).addTo(map);

    // Ruta de coordenadas
    const rutaCoords = [
      [38.550345, -6.239568],
      [38.551175, -6.240724],
      [38.551484, -6.245389],
      [38.552921, -6.241576],
      [38.552462, -6.241404],
      [38.553049, -6.240185],
      [38.55280432227918, -6.23993727809947],
      [38.55144056550526, -6.238620520015142],
      [38.55128534155161, -6.2385139022066936],
      [38.550866442060396, -6.238834186614105],
      [38.55015145200217, -6.238097052075162],
      [38.54869703810946, -6.2371061695026455]
    ];

    const preguntas = [
      { q: "¿Qué color es vuestro equipo?", a: ["rojo","verde","azul","amarillo","rosa"] },
      { q: "¿Cómo se llama el objeto de madera donde se posan los cántaros?", a: ["burropalo"] },
      { q: "¿Con qué otro caño está conectado el pilar?", a: ["el cañito","cañito"] },
      { q: "¿Qué convento se encontraba en el edificio actual del Ayuntamiento?", a: ["el convento de jesús y maría","convento de jesús y maría"] },
      { q: "¿Qué peculiaridad tiene la estructura de esta parroquia?", a: ["sus dos torres gemelas","dos torres gemelas"] },
      { q: "¿Qué se aprecia en la parte superior de las rejas de la Casa de la Cultura?", a: ["la cruz de santiago","cruz de santiago"] },
      { q: "¿Cuál es el milagro más conocido de San Juan Macías?", a: ["el milagro del arroz","milagro del arroz"] },
      { q: "¿Qué iniciales se encuentran en la entrada de este edificio?", a: ["fga"] },
      { q: "¿Cuántos años tenía cuando murió Juan Meléndez Valdés?", a: ["63 años","63"] },
      { q: "¿Qué árbol es el que encontramos en dicha plaza?", a: ["el fresno","fresno"] },
      { q: "¿Busca la fecha y di la suma de los dígitos?", a: ["23"] },
      { q: "¿Cuántos arcos interiores y exteriores posee la Ermita del Cristo de las Misericordias?", a: ["27","veintisiete"] }
    ];

    let markers = [];

    function crearPopup(i) {
      return `
        <b>Pregunta ${i+1}:</b><br>${preguntas[i].q}<br><br>
        <input type='text' id='answer${i}' class='answer' placeholder='Escribe tu respuesta'/>
        <button class='check' onclick='checkAnswer(${i})'>Responder</button>
      `;
    }

    window.checkAnswer = function(i) {
      const input = document.getElementById('answer'+i);
      if (!input) return;
      const respuesta = input.value.trim().toLowerCase();
      if (preguntas[i].a.includes(respuesta)) {
        alert("✅ ¡Correcto! Se desbloquea el siguiente punto.");
        markers[i].closePopup();
        if (i+1 < markers.length) {
          markers[i+1].addTo(map).openPopup();
        } else {
          alert("🎉 ¡Has completado la gymkhana!");
        }
      } else {
        alert("❌ Respuesta incorrecta, inténtalo de nuevo.");
      }
    }

    // Crear marcadores ocultos
    for (let i=0; i<rutaCoords.length; i++) {
      const m = L.marker(rutaCoords[i]).bindPopup(crearPopup(i));
      markers.push(m);
    }

    // Mostrar solo el primero al inicio
    markers[0].addTo(map).openPopup();
  </script>
</body>
</html>
