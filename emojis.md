---
layout: page
title: Emojis
search_exclude: true
permalink: /emojis/
---

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mood-Based Emoji Generator</title>
    <style>
        body {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
            font-family: Arial, sans-serif;
            background-color: #f5f5f5;
        }

        h1 {
            font-size: 2rem;
            margin-bottom: 20px;
        }

        #emoji {
            font-size: 5rem;
            margin: 20px 0;
        }

        select {
            padding: 10px;
            font-size: 1.2rem;
            margin-bottom: 20px;
        }

        button {
            padding: 10px 20px;
            font-size: 1.2rem;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        button:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>

    <h1>Mood-Based Emoji Generator</h1>
    
    <!-- Mood Selection Dropdown -->
    <select id="mood">
        <option value="">Select Your Mood</option>
        <option value="happy">Happy</option>
        <option value="sad">Sad</option>
        <option value="angry">Angry</option>
        <option value="excited">Excited</option>
        <option value="surprised">Surprised</option>
    </select>
    
    <div id="emoji">🙂</div>
    
    <button onclick="generateEmoji()">Generate Emoji</button>

    <script>
        // Define emojis for each mood
        const moodEmojis = {
            happy: ["😀", "😁", "😊", "😄", "😃", "😆"],
            sad: ["😢", "😭", "😞", "😔", "😟"],
            angry: ["😡", "😠", "🤬", "😤", "👿"],
            excited: ["🤩", "🥳", "😎", "🎉", "👏"],
            surprised: ["😱", "😲", "😯", "🤯", "😳"]
        };

        function generateEmoji() {
            // Get selected mood
            const selectedMood = document.getElementById("mood").value;
            
            // Check if a mood is selected
            if (selectedMood && moodEmojis[selectedMood]) {
                // Get random emoji from the selected mood's emojis
                const emojis = moodEmojis[selectedMood];
                const randomIndex = Math.floor(Math.random() * emojis.length);
                const randomEmoji = emojis[randomIndex];
                
                // Display the random emoji
                document.getElementById("emoji").textContent = randomEmoji;
            } else {
                alert("Please select a mood!");
            }
        }
    </script>

</body>
</html>
