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
       



<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        body {
            font-family: Arial, sans-serif;
            padding: 20px;
            background-color: white;
            color: black;
        }
        h1, h2 {
            text-align: center;
        }
        .code-container {
            background-color: #f4f4f4;
            padding: 10px;
            border-radius: 5px;
            border: 1px solid #ccc;
            white-space: pre-wrap;
            font-family: monospace;
        }
        .description {
            margin-top: 10px;
            font-style: italic;
        }
    </style>
</head>
<body>


    <h2>Setting Up the API</h2>
    <div class="code-container">
from flask import Blueprint, jsonify, Flask, request
from flask_restful import Api, Resource
from flask_cors import CORS

music_pref_api = Blueprint('music_pref_api', __name__, url_prefix='/api/musicpref')
api = Api(music_pref_api)
CORS(music_pref_api)
    </div>
    <p class="description">This initializes the Flask API, enabling communication between the frontend and backend.</p>

    <h2>Defining the Data Model</h2>
    <div class="code-container">
class MusicPref:
    def __init__(self, name, uid, favorites, music_platform, learn_preference, listening_frequency, favorite_era, important_aspect):
        self.name = name
        self.uid = uid
        self.favorites = favorites
        self.music_platform = music_platform
        self.learn_preference = learn_preference
        self.listening_frequency = listening_frequency
        self.favorite_era = favorite_era
        self.important_aspect = important_aspect
    </div>
    <p class="description"> Template for storing user music preferences. It says what kind of information (name, favorite artist, etc.) we will keep. This class represents a user’s music preferences, storing key attributes.</p>

    <h2>Handling API Requests</h2>
    <div class="code-container">
class MusicPrefAPI(Resource):
    def get(self):
        return jsonify(music_preferences)

    def post(self):
        body = request.get_json()
        new_pref = {
            "name": body["name"],
            "uid": body["uid"],
            "favorites": body["artist_pref"].split(", "),
            "music_platform": body["method"],
            "learn_preference": body["new_music"],
            "listening_frequency": body["how_often"],
            "favorite_era": body["era"],
            "important_aspect": body["favorite_aspect"]
        }
        music_preferences.append(new_pref)
        return jsonify(new_pref)
    </div>
    <p class="description"> Listens for requests from the website. This class handles GET and POST requests for retrieving and adding user data.</p>

    <h2>Fetching and Displaying Data</h2>
    <div class="code-container">
function fetchMusicPrefs() {
    fetch(apiUrl)
        .then(response => response.json())
        .then(data => {
            const tableBody = document.getElementById('preferencesTable').getElementsByTagName('tbody')[0];
            tableBody.innerHTML = ""; 
            data.forEach(pref => {
                const row = tableBody.insertRow();
                row.innerHTML = `
                    <td>${pref.name}</td>
                    <td>${pref.uid}</td>
                    <td>${pref.favorites.join(', ')}</td>
                    <td>${pref.music_platform}</td>
                    <td>${pref.learn_preference}</td>
                    <td>${pref.listening_frequency}</td>
                    <td>${pref.favorite_era}</td>
                    <td>${pref.important_aspect}</td>
                    <td class="actions">
                        <button onclick="editMusicPref('${pref.uid}')">Edit</button>
                        <button onclick="deleteMusicPref(${pref.id}, this)">Delete</button>
                    </td>
                `;
            });
        })
        .catch(error => console.error("Error fetching data:", error));
}
    </div>
    <p class="description">This function retrieves stored music preferences from the backend and displays them in a table.</p>

    <h2>Editing a User's Name</h2>
    <div class="code-container">
function editMusicPref(uid) {
    editingUID = uid;
    const modal = document.getElementById('editModal');
    modal.style.display = 'flex';
}
    </div>
    <p class="description">This function opens a modal for editing a user’s name.</p>

    <div class="code-container">
document.getElementById('saveNameButton').addEventListener('click', () => {
    const newName = document.getElementById('editName').value;
    fetch(`${apiUrl}`, {
        method: 'PUT',
        headers: { 'Content-Type': 'application/json' },
        body: JSON.stringify({ uid: editingUID, name: newName })
    })
    .then(response => response.json())
    .then(() => {
        alert('Name updated!');
        fetchMusicPrefs();
        document.getElementById('editName').value = ''; 
        document.getElementById('editModal').style.display = 'none';
    })
    .catch(error => console.error('Error updating name:', error));
});
    </div>
    <p class="description">This function sends a PUT request to update a user’s name in the backend.</p>

    <h2>Deleting a Music Preference</h2>
    <div class="code-container">
function deleteMusicPref(id, buttonElement) {
    if (confirm('Are you sure you want to delete this entry?')) {
        fetch(apiUrl, {
            method: 'DELETE',
            headers: { 'Content-Type': 'application/json' },
            body: JSON.stringify({ id: id })
        })
        .then(response => {
            if (response.ok) {
                alert('Music preference deleted!');
                const row = buttonElement.closest('tr');
                row.remove();
            } else {
                alert('Error deleting music preference');
            }
        })
        .catch(error => console.error('Error deleting data:', error));
    }
}
    </div>
    <p class="description">This function handles deleting a user’s music preference from the database.</p>

</body>
</html>


<!-- Lists -->
<h2>Lists</h2>
<p>The <code>favorites</code> field in the <code>MusicPref</code> model is an example of a list. It allows a user to store multiple favorite artists.</p>

<textarea readonly rows="10" cols="80">
music_pref = MusicPref(
    name=name,
    uid=uid,
    favorites=[artist_pref],  # List storing favorite artists
    music_platform=method,
    learn_preference=new_music,
    listening_frequency=how_often,
    favorite_era=era,
    important_aspect=favorite_aspect
)
</textarea>



<!-- Algorithms in Code -->
<h2>Algorithms</h2>
<p>Example of an algorithm that <strong>fetches a user’s music preference</strong> based on their name:</p>

<textarea readonly rows="10" cols="80">
@staticmethod
def get_user(name):
    users = {
        "Hannah": { "ArtistPref": "Taylor Swift", "Method": "Spotify" },
        "Rhea": { "ArtistPref": "SZA", "Method": "Spotify" },
        "Carson": { "ArtistPref": "Frank Ocean", "Method": "Spotify" }
    }
    return users.get(name)  # Algorithm that looks up a user by name
</textarea>

<p>This algorithm takes a <strong>name</strong> as input, searches for it in a <strong>dictionary</strong>, and returns the matching data. If the name isn’t found, it returns nothing.</p>
