---
layout: base
title: Javascript Shell
description: jc shell
hide: true
---
## Water Polo Jokes

<div style="border: 2px solid #2196F3; border-radius: 10px; padding: 15px; background-color: #e3f2fd;">
   <h2>Water Polo Joke Generator</h2>
   <p>Enjoy some humor related to water polo with the button below.</p>
   
   <button onclick="generateJoke()" style="background-color: #2196F3; color: white; border: none; padding: 10px 20px; font-size: 16px; border-radius: 5px; cursor: pointer;">
      Get a Joke
   </button>
   
   <p id="joke-output" style="margin-top: 10px; font-style: italic;"></p>
</div>

<script>
   var jokes = [
      { joke: "Why did the water polo player go to the bank? To get his 'current' account!", complexity: "O(1)" },
      { joke: "What’s a water polo player’s favorite type of music? Anything with a good beat!", complexity: "O(1)" },
      { joke: "Why do water polo players always have a good day? Because they’re always making a splash!", complexity: "O(1)" },
      { joke: "What do you call a water polo player who can sing? A water virtuoso!", complexity: "O(1)" },
      { joke: "Why did the water polo player refuse to play cards? Because he didn’t want to deal with the pressure!", complexity: "O(1)" },
      { joke: "How does a water polo player stay cool during a game? By swimming in their own pool of confidence!", complexity: "O(1)" },
      { joke: "Why did the water polo player bring a ladder to practice? To reach new heights!", complexity: "O(1)" },
      { joke: "What did the coach say to the water polo team? ‘Let’s make a big splash today!’", complexity: "O(1)" }
   ];

   function generateJoke() {
      var randomIndex = Math.floor(Math.random() * jokes.length);
      var selectedJoke = jokes[randomIndex];
      document.getElementById('joke-output').innerText = selectedJoke.joke + " (Complexity: " + selectedJoke.complexity + ")";
   }
</script>

