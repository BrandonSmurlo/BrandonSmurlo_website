---
layout: page
title: Interactive Map
search_exclude: true
permalink: /Interactive Map/
---

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Map</title>
    <!-- Leaflet CSS -->
    <link rel="stylesheet" href="https://unpkg.com/leaflet/dist/leaflet.css" />
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
        }
        #map {
            height: 100vh; /* Full viewport height */
            width: 100%; /* Full width */
        }
        .leaflet-popup-content-wrapper {
            background-color: #fff;
            border-radius: 8px;
            box-shadow: 0 2px 6px rgba(0, 0, 0, 0.3);
        }
        .leaflet-popup-tip {
            background-color: #fff;
        }
    </style>
</head>
<body>

    <div id="map"></div>

    <!-- Leaflet JS -->
    <script src="https://unpkg.com/leaflet/dist/leaflet.js"></script>
    <script>
        // Initialize the map
        const map = L.map('map').setView([51.505, -0.09], 13); // Coordinates for initial view and zoom level

        // Add tile layer to the map
        L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
            attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors'
        }).addTo(map);

        // Define locations and information for markers
        const locations = [
            {
                coords: [51.505, -0.09],
                title: "Big Ben",
                info: `<b>Big Ben</b><br>
                       Located in the heart of London, Big Ben is the nickname for the Great Bell of the clock at the north end of the Palace of Westminster. It is one of the most famous landmarks in the UK.` 
            },
            {
                coords: [51.515, -0.1],
                title: "London Eye",
                info: `<b>London Eye</b><br>
                       The London Eye is a giant Ferris wheel situated on the South Bank of the River Thames. It offers breathtaking views of the city and is a popular tourist attraction.` 
            },
            {
                coords: [51.525, -0.12],
                title: "Trafalgar Square",
                info: `<b>Trafalgar Square</b><br>
                       Trafalgar Square is a public square in central London, named after the Battle of Trafalgar. It features the Nelson's Column and is a hub of cultural and social activity.` 
            }
            // Add more markers as needed
        ];

        // Add markers to the map
        locations.forEach(location => {
            L.marker(location.coords)
                .addTo(map)
                .bindPopup(location.info);
        });
    </script>

</body>
</html>
