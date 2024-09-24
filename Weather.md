---
layout: page
title: Weather
search_exclude: true
permalink: /Weather/
---

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dynamic Weather Dashboard</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #f0f8ff;
            color: #333;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        h1 {
            font-size: 2.5rem;
            margin-bottom: 20px;
        }

        #weather {
            background-color: #fff;
            border-radius: 10px;
            padding: 20px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            text-align: center;
            width: 80%;
            max-width: 400px;
        }

        #weather img {
            width: 100px;
        }

        .info {
            margin: 10px 0;
            font-size: 1.2rem;
        }

        #loading {
            font-size: 1.5rem;
        }

        button {
            padding: 10px 20px;
            background-color: #007bff;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>
    <h1>Dynamic Weather Dashboard</h1>

    <div id="weather">
        <p id="loading">Fetching your weather...</p>
    </div>

    <script>
        const apiKey = 'YOUR_API_KEY';  // Replace with your OpenWeatherMap API Key
        const weatherDiv = document.getElementById('weather');

        function displayWeather(data) {
            const tempCelsius = (data.main.temp - 273.15).toFixed(1);
            const description = data.weather[0].description;
            const icon = `https://openweathermap.org/img/wn/${data.weather[0].icon}@2x.png`;

            weatherDiv.innerHTML = `
                <img src="${icon}" alt="Weather Icon">
                <div class="info">Location: ${data.name}</div>
                <div class="info">Temperature: ${tempCelsius}°C</div>
                <div class="info">Weather: ${description}</div>
                <div class="info">Wind Speed: ${data.wind.speed} m/s</div>
            `;
        }

        function fetchWeather(lat, lon) {
            const url = `https://api.openweathermap.org/data/2.5/weather?lat=${lat}&lon=${lon}&appid=${apiKey}`;
            fetch(url)
                .then(response => response.json())
                .then(data => displayWeather(data))
                .catch(err => {
                    weatherDiv.innerHTML = '<p>Error fetching weather data</p>';
                });
        }

        function getLocation() {
            if (navigator.geolocation) {
                navigator.geolocation.getCurrentPosition(position => {
                    const { latitude, longitude } = position.coords;
                    fetchWeather(latitude, longitude);
                });
            } else {
                weatherDiv.innerHTML = '<p>Geolocation is not supported by this browser.</p>';
            }
        }

        getLocation();
    </script>
</body>
</html>
