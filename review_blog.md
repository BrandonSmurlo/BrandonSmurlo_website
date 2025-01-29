---
layout: base 
title: Sprint 5 Review
search_exclude: true

---


<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>1. Functions</title>
    <style>
        img {
            margin-bottom: 40px;
        }
        section {
            margin-top: 40px;
        }
        h2 {
            margin-top: 50px;
        }
    </style>
</head>
<body>
    <header>
        <h1>Functions</h1>
    </header>
      
    <img src="images/Screenshot 2025-01-27 at 6.53.49 PM.png" alt="Screenshot of my code" width="450" />
    
    <section>
        <h2>Our Program</h2>
        <p>My feature collects user preferences about music which is then stored in a backend table database. The group program's purpose is to collect information for the user's profile on the webpage so that they can have an experience tailored just for them.</p>
    </section>

   <img src="images/Screenshot 2025-01-27 at 10.21.30 PM.png" alt="Screenshot" width="575" />

        <h2>2. Creating the Database Model</h2>
        <p>The <code>MusicPref</code> model represents a user's music preferences in the database.</p>
        <h3>Key Features:</h3>
        <ul>
            <li><strong>id</strong>: Primary key for each entry.</li>
            <li><strong>name</strong>: User's name.</li>
            <li><strong>uid</strong>: Unique identifier for the user.</li>
            <li><strong>favorites</strong>: A list of the user's favorite artists.</li>
            <li><strong>music_platform</strong>: Platform the user listens to music on (e.g., Spotify).</li>
            <li><strong>learn_preference</strong>: How the user discovers new music.</li>
            <li><strong>listening_frequency</strong>: Frequency of music listening.</li>
            <li><strong>favorite_era</strong>: Favorite music era (e.g., 90s, modern).</li>
            <li><strong>important_aspect</strong>: What aspect of music is most important to the user (e.g., vocals, rhythm).</li>
        </ul>
</body>
</html>

 <img src="images/Screenshot 2025-01-27 at 6.37.27 PM.png" alt="Screenshot of my code" />


 <section>
        <h2>3. Defining Methods in the Model</h2>
        <p>The model has several methods to manage data:</p>
        <ul>
            <li><strong>create()</strong>: Creates a new user or updates an existing user's preferences.</li>
            <li><strong>add_favorite()</strong>: Adds a new favorite artist to the user's preferences.</li>
            <li><strong>remove_favorite()</strong>: Removes an artist from the user's favorites.</li>
            <li><strong>update()</strong>: Updates the user's preferences.</li>
            <li><strong>delete()</strong>: Deletes the user's preferences from the database.</li>
            <li><strong>restore()</strong>: Synchronizes data, creating or updating user preferences as needed.</li>
        </ul>
        <img src="images/Screenshot 2025-01-27 at 9.52.47 PM.png" alt="Screenshot" width="450" />

<ul>
  <li>Checks if a user exists in the database by <code>_uid</code>.</li>
  <li>
    If user exists:
    <ul>
      <li>Updates their details and saves changes.</li>
    </ul>
  </li>
  <li>
    If user doesn’t exist:
    <ul>
      <li>Adds the new user to the database and commits it.</li>
    </ul>
  </li>
  <li><code>create_or_update_music_pref(data)</code> method:</li>
  <ul>
    <li>Searches for a user by <code>uid</code>.</li>
    <li>
      If user exists:
      <ul>
        <li>Updates their data using <code>update(data)</code>.</li>
      </ul>
    </li>
    <li>
      If user doesn’t exist:
      <ul>
        <li>Creates a new user with <code>create()</code>.</li>
      </ul>
    </li>
  </ul>
</ul>

    <section>
        <h2>4. Setting Up the API</h2>
        <p>Using Flask-RESTful, we define API resources for managing the music preferences.</p>
        <p><strong>MusicPrefResource</strong> handles <code>GET</code>, <code>POST</code>, <code>PUT</code>, and <code>DELETE</code> requests.</p>
        <ul>
            <li><strong>POST</strong>: Create a new user or update their preferences.</li>
            <li><strong>GET</strong>: Retrieve all users' music preferences.</li>
            <li><strong>PUT</strong>: Update a user's preferences.</li>
            <li><strong>DELETE</strong>: Delete a user's preferences.</li>
        </ul>
        
<img src="images/Screenshot 2025-01-27 at 10.04.57 PM.png" alt="Screenshot" width="450" />
<ul>
  <li>Initializes an empty list <code>restored_records</code>.</li>
  <li>Loops through <code>data</code>, checking if each record exists by <code>id</code>.</li>
  <li>If record exists, it updates it and adds to <code>restored_records</code>.</li>
  <li>If record doesn't exist, creates a new one and adds to the list.</li>
  <li>Catches errors, rolls back, and prints an error message if needed.</li>
  <li>Returns the list of updated/created records.</li>
</ul>
    <section>
        <h2>5. Adding Sample Data</h2>
        <p>To initialize the database with sample users, we define the <code>initMusicPref()</code> function. It creates a user with their music preferences for testing purposes.</p>
      
<img src="images/Screenshot 2025-01-27 at 10.08.08 PM.png" alt="Screenshot of my code" />
    <section>
        <h2>6. Using the API</h2>
        <p>Now, we can interact with the API:</p>
        <ul>
            <li><strong>GET</strong> <code>/api/musicpref</code>: Fetch all music preferences.</li>
            <li><strong>POST</strong> <code>/api/musicpref</code>: Add or update a user's music preferences.</li>
            <li><strong>PUT</strong> <code>/api/musicpref</code>: Update a user's music preferences by <code>uid</code>.</li>
            <li><strong>DELETE</strong> <code>/api/musicpref</code>: Delete a user's music preferences by <code>uid</code>.</li>
        </ul>
    </section>
<img src="images/Screenshot 2025-01-27 at 6.58.55 PM.png" alt="Screenshot of my code" />
    <footer>
       
