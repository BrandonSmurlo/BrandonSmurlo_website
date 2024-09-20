---
layout: page
title: Recipe Maker
search_exclude: true
permalink: /Recipe Maker/
---

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Recipe Generator</title>
    <style>
        body {
            background: url('https://example.com/kitchen-background.jpg') no-repeat center center fixed;
            background-size: cover;
            font-family: 'Arial', sans-serif;
            color: #333;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
            padding: 20px;
        }

        h1 {
            font-size: 2.5rem;
            margin-bottom: 20px;
            text-shadow: 2px 2px 5px rgba(255, 255, 255, 0.7);
        }

        select, button {
            padding: 15px 30px;
            font-size: 1.2rem;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            margin: 10px;
        }

        select {
            background-color: #ffcccb;
        }

        button {
            background-color: #4CAF50;
            color: white;
            transition: background-color 0.3s;
        }

        button:hover {
            background-color: #45a049;
        }

        #recipe {
            font-size: 1.5rem;
            margin: 20px 0;
            background-color: rgba(255, 255, 255, 0.8);
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
            display: none;
        }
    </style>
</head>
<body>

    <h1>Recipe Generator</h1>
    <select id="foodSelect">
        <option value="">Select a Food</option>
        <option value="spaghetti">Spaghetti🍝</option>
        <option value="tacos">Tacos🌮</option>
        <option value="salad">Salad🥗</option>
        <option value="pancakes">Pancakes🥞</option>
        <option value="pizza">Pizza🍕</option>
    </select>
    
    <button id="generateFoodBtn">Generate Recipe</button>
    
    <div id="recipe"></div>
    
    <button id="dessertBtn" style="display:none;">Generate Dessert Recipe🍰</button>
    <div id="dessert" style="display:none;"></div>
    
    <button id="resetBtn" style="display:none;">Reset</button>

    <script>
        const recipes = {
            spaghetti: "Spaghetti Recipe:\n1. Cook spaghetti noodles.\n2. Prepare sauce with tomatoes and spices.\n3. Combine and serve with cheese.",
            tacos: "Tacos Recipe:\n1. Cook meat and spices.\n2. Fill tortillas with meat and toppings.\n3. Serve with salsa.",
            salad: "Salad Recipe:\n1. Chop lettuce, tomatoes, and cucumbers.\n2. Add dressing and toss.\n3. Serve chilled.",
            pancakes: "Pancakes Recipe:\n1. Mix flour, eggs, and milk.\n2. Cook on a skillet until golden.\n3. Serve with syrup.",
            pizza: "Pizza Recipe:\n1. Prepare dough and spread sauce.\n2. Add toppings and cheese.\n3. Bake until golden.",
            dessert: "Dessert Recipe:\n1. Mix ingredients and bake for 30 mins.\n2. Let cool and serve with whipped cream."
        };

        document.getElementById("generateFoodBtn").onclick = function() {
            const foodSelect = document.getElementById("foodSelect");
            const selectedFood = foodSelect.value;
            if (selectedFood) {
                document.getElementById("recipe").textContent = recipes[selectedFood];
                document.getElementById("recipe").style.display = "block";
                document.getElementById("dessertBtn").style.display = "inline";
                document.getElementById("generateFoodBtn").style.display = "none";
            }
        };

        document.getElementById("dessertBtn").onclick = function() {
            document.getElementById("dessert").textContent = recipes.dessert;
            document.getElementById("dessert").style.display = "block";
            document.getElementById("dessertBtn").style.display = "none";
            document.getElementById("resetBtn").style.display = "inline";
        };

        document.getElementById("resetBtn").onclick = function() {
            document.getElementById("foodSelect").selectedIndex = 0;
            document.getElementById("recipe").style.display = "none";
            document.getElementById("dessert").style.display = "none";
            document.getElementById("dessertBtn").style.display = "none";
            document.getElementById("resetBtn").style.display = "none";
            document.getElementById("generateFoodBtn").style.display = "inline";
        };
    </script>

</body>
</html>
