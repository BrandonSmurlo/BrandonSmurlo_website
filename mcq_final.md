---
layout: base 
title: CSP Final Blog
search_exclude: true

---


<div class="accomplishments-section" style="background-color: #fff3e0; padding: 25px; border-left: 8px solid #ff6f00; border-radius: 10px;">
    <h2 style="text-align: center; color: #ff6f00; font-size: 2.2em; text-transform: uppercase; font-weight: bold; margin-bottom: 15px;">
        My Top 5 Accomplishments This Trimester
    </h2>

    <div style="margin-top: 20px; text-align: center;">
        <a href="https://github.com/gaheerab/sprint4_frontend/issues/16" target="_blank" style="display: inline-block; padding: 10px 20px; background-color: #ff7043; color: white; text-decoration: none; font-weight: bold; border-radius: 5px;">
            View My Accomplishments on GitHub Issues
        </a>
    </div>

</div>


<hr style="border: 3px solid black;">

<div class="question-box" style="background-color: #f8f9fa; padding: 20px; border-left: 8px solid #117a8b;">
    <h2 style="text-align: center; color: #117a8b; font-size: 2em; text-transform: uppercase; font-weight: bold; margin-bottom: 15px;">
        CPT Requirement Highlights/Application
    </h2>

    <p class="analysis" style="font-size: 1.2em; text-align: center; margin-bottom: 20px;">
        My profile-building feature in MelodyMates allows users to input their music preferences, which are dynamically stored in a database. This feature incorporates several key computing principles required in the CPT project.
    </p>

    <table style="width: 100%; border-collapse: collapse; margin-top: 20px;">
        <tr style="background-color: #117a8b; color: white;">
            <th style="padding: 15px; text-align: left; font-size: 1.3em;">CPT Requirement</th>
            <th style="padding: 15px; text-align: left; font-size: 1.3em;">Application in MelodyMates</th>
        </tr>

        <tr style="background-color: #e3f2fd;">
            <td style="padding: 15px; font-weight: bold;">✅ Lists</td>
            <td style="padding: 15px;">
                The backend database maintains a list of user preferences, tracking favorite artists dynamically.  
                <br><br>
                <img src="images/Screenshot 2025-03-03 at 1.02.13 PM.png" alt="Database List Example" style="width: 100%; border-radius: 5px;">
            </td>
        </tr>

        <tr style="background-color: #fff3e0;">
            <td style="padding: 15px; font-weight: bold;">✅ Dictionary</td>
            <td style="padding: 15px;">
                The system uses **dictionaries** to store artist details, allowing for efficient retrieval and personalized recommendations.
            </td>
        </tr>

        <tr style="background-color: #e8f5e9;">
            <td style="padding: 15px; font-weight: bold;">✅ Sequencing, Selection, & Iteration</td>
            <td style="padding: 15px;">
                <strong>Sequencing:</strong> The recommendation process follows a logical order, retrieving user data, applying filters, and returning results.
                <br><br>
                <strong>Selection:</strong> Conditional statements determine if an artist matches user preferences before adding them to recommendations.
                <br>
                <img src="images/Screenshot 2025-03-03 at 1.05.48 PM.png" alt="Selection Example" style="width: 100%; border-radius: 5px;">
                <br><br>
                <strong>Iteration:</strong> A **for-loop** iterates through the list of user preferences to generate personalized suggestions.
                <br>
                <img src="images/Screenshot 2025-03-03 at 1.09.23 PM.png" alt="Iteration Example" style="width: 100%; border-radius: 5px;">
            </td>
        </tr>

    </table>

    <p class="analysis" style="margin-top: 20px; font-size: 1.1em; text-align: center;">
        By integrating these CPT requirements, my feature effectively processes user data, maintains structured lists, applies algorithmic logic, and delivers a dynamic, interactive experience.
    </p>
</div>


<hr style="border: 3px solid black;">

<h1>MelodyMates Project Feature</h1>

<h2 style="color: #a3c4f3; font-family: 'Comic Sans MS', cursive, sans-serif; text-shadow: 2px 2px 5px rgba(163, 196, 243, 0.6); font-size: 1.5em;">
    Music Preference Survey
</h2>

<ul>
    <li><strong>User Input:</strong> The program receives structured user-generated data through an interactive interface, allowing users to enter values such as their favorite artist and genre.</li>
    <li><strong>Data Storage:</strong> The system implements persistent data storage using a structured data abstraction, such as a database or data table, to retain user preferences across sessions.</li>
    <li><strong>Data Modification:</strong> Users can update or delete stored data dynamically, demonstrating procedural abstraction through functions that modify database entries.</li>
    <li><strong>Data Accessibility:</strong> The program displays stored user preferences using data visualization techniques, allowing other users to retrieve and explore different music tastes.</li>
    <li><strong>Data Persistence:</strong> The application ensures persistent data management by maintaining user information even after execution ends, using a cloud-based or local storage solution.</li>
</ul>

<h2>How It Works</h2>
<ol>
    <li>The user interacts with the user interface (UI) by navigating to the Music Preference Survey section on the MelodyMates website.</li>
    <li>Through input validation, the system accepts structured user input, including favorite artist, genre, and other musical preferences.</li>
    <li>Upon submission, the program executes a procedure to store the data in a relational database, making use of tables.</li>
    <li>Users can later call predefined functions to modify or remove existing data entries dynamically.</li>
    <li>Other users retrieve stored data through database queries to view and analyze the music preferences of different users.</li>
</ol>

<div style="display: flex; justify-content: center; gap: 20px; margin-top: 20px;">
    <img src="images/Screenshot 2025-02-28 at 7.51.05 PM.png" alt="Music Profile Screenshot 1" style="width: 45%; max-width: 500px;">
    <img src="images/Screenshot 2025-02-28 at 8.14.15 PM.png" alt="Music Profile Screenshot 2" style="width: 45%; max-width: 500px;">
</div>



<hr style="border: 3px solid black;">

<div class="frq-section" style="background-color: #eef7ff; padding: 25px; border-radius: 12px; box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.1);">
    <h2 style="text-align: center; color: #0d47a1; font-size: 2.2em; font-weight: bold; margin-bottom: 15px;">
        Understanding FRQ Language in MelodyMates
    </h2>
    
    <p style="font-size: 1.2em; text-align: center; margin-bottom: 20px;">
        The format requires precise, structured responses to programming problems. My website, MelodyMates, reflects these concepts through well-defined <b>algorithms</b>, efficient data structures like <b>lists</b> and other <b>collections</b>, and logical program behavior with clear <b>parameters</b> for functions.
    </p>
    
    <div style="display: flex; flex-wrap: wrap; gap: 20px; justify-content: center;">
        <div class="frq-card" style="background: white; padding: 20px; border-radius: 10px; width: 45%; box-shadow: 0px 3px 8px rgba(0, 0, 0, 0.1);">
            <h3 style="color: #0d47a1;">Calling Functions</h3>
            <p>MelodyMates follows the concept of <b>calling functions</b> by organizing functionalities into reusable methods with clear <b>parameters</b>, ensuring modular and maintainable code.</p>
        </div>
        
        <div class="frq-card" style="background: white; padding: 20px; border-radius: 10px; width: 45%; box-shadow: 0px 3px 8px rgba(0, 0, 0, 0.1);">
            <h3 style="color: #0d47a1;">Program Complexity</h3>
            <p>Data retrieval and processing in MelodyMates is structured to minimize redundant operations, following <b>efficiency principles</b> in <b>algorithms</b> and <b>program complexity</b>.</p>
        </div>
        
        <div class="frq-card" style="background: white; padding: 20px; border-radius: 10px; width: 45%; box-shadow: 0px 3px 8px rgba(0, 0, 0, 0.1);">
            <h3 style="color: #0d47a1;">State & Behavior</h3>
            <p>MelodyMates maintains user preferences using structured <b>lists</b> and other <b>collections</b>, ensuring that the <b>state</b> of each session aligns with expected user interactions, including <b>input from the user</b>.</p>
        </div>
        
        <div class="frq-card" style="background: white; padding: 20px; border-radius: 10px; width: 45%; box-shadow: 0px 3px 8px rgba(0, 0, 0, 0.1);">
            <h3 style="color: #0d47a1;">Preconditions & Postconditions</h3>
            <p>Each function in MelodyMates is written with clear <b>preconditions</b> and <b>postconditions</b>, ensuring data integrity and predictable outputs when <b>input from a device</b>, <b>online data stream</b>, or <b>file</b> is processed.</p>
        </div>
    </div>
    
    <p style="margin-top: 20px; font-size: 1.1em; text-align: center;">
        Understanding the <b>language</b> is essential for structured programming. MelodyMates integrates these principles to maintain clarity, efficiency, and logical flow throughout its codebase, following best practices for <b>algorithms</b> and program design.
    </p>
    
    <div style="margin-top: 40px; font-size: 1.1em; text-align: left;">
        <h3 style="color: #0d47a1;">Definitions of Terms Used:</h3>
        <ul>
            <li><b>Calling Functions:</b> Using a function in your program to perform a task. Functions are written to be reusable to avoid repeating code.</li>
            <li><b>Parameters:</b> Values you provide to a function to customize what it does or how it works.</li>
            <li><b>List:</b> A collection of items that can be ordered and accessed by position, often used for storing and managing data.</li>
            <li><b>Other Types of Collection:</b> Other data structures used to store multiple items, such as arrays, sets, or maps, which help organize and manipulate data efficiently.</li>
            <li><b>Program Complexity:</b> How complicated or efficient a program is, based on factors like how much time or memory it uses.</li>
            <li><b>Input from One of the Following:</b> The data that your program receives from different sources like the user, a device, an online data stream, or a file.</li>
            <li><b>Algorithms:</b> Step-by-step instructions for solving a problem or performing a task, which is central to how a program works.</li>
        </ul>
    </div>
</div>

<hr style="border: 3px solid black;">

<div class="ap-exam-application" style="background-color: #f0f4f8; padding: 30px; border-radius: 15px; box-shadow: 0px 5px 15px rgba(0, 0, 0, 0.1);">
    <h2 style="text-align: center; color: #0b3d91; font-size: 2.5em; font-weight: bold; margin-bottom: 20px;">
        AP Exam Application
    </h2>

    <div class="concepts-container" style="display: flex; flex-wrap: wrap; gap: 30px; justify-content: center;">
        <!-- Concept 1 -->
        <div class="concept-card" style="background: #fff; padding: 25px; border-radius: 12px; width: 45%; box-shadow: 0px 4px 12px rgba(0, 0, 0, 0.15);">
            <h3 style="color: #117a8b; font-size: 1.8em;"> Algorithm Design</h3>
            <ul style="font-size: 1.2em; list-style-type: square; padding-left: 20px;">
                <li><strong>Efficiency:</strong> Apply time and space complexity principles to choose the optimal algorithm.</li>
                <li><strong>Modularization:</strong> Break down large problems into smaller reusable functions for better clarity and maintainability.</li>
                <li><strong>Recursion:</strong> Use recursive solutions where applicable, as they are a common topic on the AP exam.</li>
            </ul>
        </div>

        <!-- Concept 2 -->
        <div class="concept-card" style="background: #fff; padding: 25px; border-radius: 12px; width: 45%; box-shadow: 0px 4px 12px rgba(0, 0, 0, 0.15);">
            <h3 style="color: #117a8b; font-size: 1.8em;"> Data Structures</h3>
            <ul style="font-size: 1.2em; list-style-type: square; padding-left: 20px;">
                <li><strong>Lists & Arrays:</strong> Store and manipulate ordered collections of data with efficient indexing.</li>
                <li><strong>Dictionaries:</strong> Use hashmaps for fast lookup and retrieval of data based on unique keys.</li>
                <li><strong>Iterators:</strong> Efficiently traverse through lists and arrays with loops for dynamic data processing.</li>
            </ul>
        </div>

        <!-- Concept 3 -->
        <div class="concept-card" style="background: #fff; padding: 25px; border-radius: 12px; width: 45%; box-shadow: 0px 4px 12px rgba(0, 0, 0, 0.15);">
            <h3 style="color: #117a8b; font-size: 1.8em;"> Object-Oriented Programming</h3>
            <ul style="font-size: 1.2em; list-style-type: square; padding-left: 20px;">
                <li><strong>Classes & Objects:</strong> Organize code using classes for better structure, encapsulation, and reusability.</li>
                <li><strong>Inheritance:</strong> Create hierarchical relationships between classes for code reuse and better design.</li>
                <li><strong>Polymorphism:</strong> Use method overriding to create flexible and extensible programs.</li>
            </ul>
        </div>

        <!-- Concept 4 -->
        <div class="concept-card" style="background: #fff; padding: 25px; border-radius: 12px; width: 45%; box-shadow: 0px 4px 12px rgba(0, 0, 0, 0.15);">
            <h3 style="color: #117a8b; font-size: 1.8em;"> Problem Solving Techniques</h3>
            <ul style="font-size: 1.2em; list-style-type: square; padding-left: 20px;">
                <li><strong>Selection:</strong> Use conditional statements to control the flow based on decision-making criteria.</li>
                <li><strong>Iteration:</strong> Loop through data structures to apply logic repeatedly for dynamic solutions.</li>
                <li><strong>Preconditions & Postconditions:</strong> Establish clear expectations for functions to maintain program correctness.</li>
            </ul>
        </div>

    </div>
</div>


<hr style="border: 3px solid black;">

<!-- Blog Section: Feedback from Ms. Pataki -->
<div style="margin: 40px auto; width: 80%; background-color: #fff3cd; padding: 20px; border-radius: 15px; box-shadow: 4px 4px 10px rgba(0, 0, 0, 0.1); text-align: center;">
    
    <h2 style="color: #856404; font-size: 2em; text-shadow: 1px 1px 4px rgba(0, 0, 0, 0.1);">Feedback & Improvements</h2>
    
    <p style="color: #333; font-size: 1.2em; margin-bottom: 20px;">
        During our website review with <strong>Ms. Pataki</strong>, we presented a brief rundown of our website’s features, showcasing the different functionalities we implemented.
    </p>
    
    <div style="display: flex; justify-content: space-around; flex-wrap: wrap; gap: 20px;">

        <!-- Feedback Received -->
        <div style="width: 45%; background-color: #f8d7da; padding: 15px; border-radius: 12px; box-shadow: 3px 3px 8px rgba(0, 0, 0, 0.1);">
            <h3 style="color: #721c24;">Feedback Given</h3>
            <p style="color: #721c24; font-size: 1.1em;">
                Ms. Pataki suggested an improvement for our <strong>Artist Recommendation</strong> feature—allowing users to edit their favorite artists after making a submission.
            </p>
        </div>

        <!-- Action Taken -->
        <div style="width: 45%; background-color: #d4edda; padding: 15px; border-radius: 12px; box-shadow: 3px 3px 8px rgba(0, 0, 0, 0.1);">
            <h3 style="color: #155724;"> Action Taken</h3>
            <p style="color: #155724; font-size: 1.1em;">
                Based on her feedback, we <strong>updated the feature</strong> to allow users to modify their favorite artists, improving usability and user experience.
            </p>
        </div>

    </div>

    <p style="margin-top: 20px; color: #333; font-size: 1.2em;">
        This change ensures that users have more control over their preferences, making the feature more dynamic and useful!
    </p>

</div>

<hr style="border: 3px solid black;">

<h1>Night at the Museum</h1>


<h2>Book Site</h2>
<ul>
    <li>A feature allows users to input books along with the author, storing them for others as recommendations.</li>
    <li>Users can rate books, and others can see their ratings.</li>
    <li>The feature shown in the photo allows users to add book reviews, which I thought was cool and interesting.</li>
</ul>
<img src="images/Screenshot 2025-02-28 at 1.42.33 PM.png" alt="Book Website Screenshot" width="500">


<h2>Cantella</h2>
<ul>
    <li>A website designed for high school students to help manage their grades.</li>
    <li>A key feature allows students to interact with others in the same class to study together.</li>
    <li>Includes grade logs for each class to track academic progress.</li>
</ul>
<img src="images/Screenshot 2025-02-28 at 1.41.48 PM.png" alt="Cantella Website Screenshot" width="500">

<h2>Travel Plan Site</h2>
<ul>
    <li>Users can look at reviews from others for different hotels worldwide by typing in a location.</li>
    <li>A key feature allows users to rate hotels, and a dynamic bar fills based on the average rating.</li>
    <li>Includes a map displaying various travel locations around the world, as shown in the image.</li>
</ul>
<img src="images/Screenshot 2025-02-28 at 1.43.24 PM.png" alt="Travel Plan Website Screenshot" width="500">



<hr style="border: 3px solid black;">

<h1 style="text-align: center; font-size: 2em;">Night at the Museum: Website Feedback & Reflection</h1>

<div style="display: flex; justify-content: space-around; flex-wrap: wrap; gap: 20px; padding: 20px;">

    <!-- Positive Feedback Section -->
    <div style="width: 45%; background-color: #d8f3dc; padding: 15px; border-radius: 15px; box-shadow: 3px 3px 10px rgba(0, 0, 0, 0.1);">
        <h2 style="color: #1b4332; text-align: center;">Positive Feedback</h2>
        <ul>
            <li>"The website frontend CSS styling looks really nice."</li>
            <li>"The features are functioning well and are interconnected smoothly."</li>
            <li>"The UI is aesthetically pleasing, and the profile picture was really cute." - <em>Arshia (CSP)</em></li>
            <li>"I'm obsessed with the color scheme and the overall moral of the website. The censorship feature is great, making it accessible to all ages."</li>
            <li>"Very nice UI! The colors and CSS styling were very good! Good job guys!"</li>
        </ul>
    </div>

    <!-- Constructive Feedback Section -->
    <div style="width: 45%; background-color: #ffddd2; padding: 15px; border-radius: 15px; box-shadow: 3px 3px 10px rgba(0, 0, 0, 0.1);">
        <h2 style="color: #9b2226; text-align: center;">Constructive Feedback</h2>
        <ul>
            <li>"The navigation bar could be more intuitive—consider adding dropdowns or hover effects."</li>
            <li>"Some text was a bit hard to read against certain backgrounds. Increasing contrast might help readability."</li>
        </ul>
    </div>

</div>

<!-- Reflection Section -->
<div style="margin-top: 30px; padding: 20px; text-align: center; background-color: #f8edeb; border-radius: 15px;">
    <h2 style="color: #6d6875;">Reflection</h2>
    <p>We received a lot of positive feedback on the website's design, functionality, and color scheme. Many people enjoyed the aesthetic appeal and user-friendly interface. However, there are a few areas we can improve:</p>
    <ul style="display: inline-block; text-align: left;">
        <li>Enhancing the navigation bar to make it more user-friendly.</li>
        <li>Improving text visibility by adjusting color contrast.</li>
    </ul>
    <p>Overall, the event was a great success, and we appreciate all the feedback we received!</p>
</div>

<hr style="border: 3px solid black;">


<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MCQ Quiz Reflection</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f9;
            margin: 20px;
            text-align: center;
        }
        h1 {
            color: #2c3e50;
            font-size: 2.5em;
            margin-bottom: 10px;
        }
        p {
            font-size: 1.2em;
            color: #555;
        }
        .summary-box {
            background-color: #d1ecf1;
            padding: 15px;
            margin: 20px auto;
            width: 80%;
            border-radius: 15px;
            box-shadow: 3px 3px 10px rgba(0, 0, 0, 0.1);
        }
        .question-box {
            width: 80%;
            margin: 20px auto;
            background-color: #fff;
            padding: 15px;
            border-radius: 12px;
            box-shadow: 3px 3px 10px rgba(0, 0, 0, 0.1);
            text-align: left;
        }
        .question-header {
            font-size: 1.5em;
            color: #6c757d;
            margin-bottom: 10px;
        }
        .analysis {
            color: #333;
            font-size: 1.1em;
            margin: 10px 0;
        }
        .right-answer {
            color: #155724;
            font-weight: bold;
            font-size: 1.2em;
        }
        .skills {
            color: #721c24;
            font-weight: bold;
            font-size: 1.1em;
        }
    </style>
</head>
<body>

    <h1>MCQ Quiz Reflection</h1>
    <p>Review of my recent quiz performance, areas of improvement, and key takeaways.</p>

    <div class="summary-box">
        <h2 style="color: #117a8b;">Performance Summary</h2>
        <p><strong>Topic 1.4 (Identifying & Correcting Errors):</strong> 57% Correct</p>
        <p><strong>Topic 2.1 (Binary Numbers):</strong> 60% Correct</p>
        <p><strong>Topic 3.12 (Calling Procedures):</strong> 60% Correct</p>
        <p><strong>Topic 3.13 (Developing Procedures):</strong> 0% Correct</p>
        <p><strong>Topic 3.15 (Random Values):</strong> 50% Correct</p>
        <p><strong>Topic 3.17 (Algorithmic Efficiency):</strong> 50% Correct</p>
        <p><strong>Topic 4.1 (The Internet):</strong> 50% Correct</p>
        <p><strong>Topic 5.2 (Digital Divide):</strong> 0% Correct</p>
        <p><strong>Topic 5.6 (Safe Computing):</strong> 67% Correct</p>
        <p>All other topics not listed here were either <strong>100% correct</strong> or <strong>N/A.</strong></p>
    </div>

    <h2 style="margin-top: 30px;">Incorrect Answers & Analysis</h2>
   
    <!-- Question Analysis -->
    <div class="question-box">
        <div class="question-header">Question 12 (Topic 2.B)</div>
        <p class="analysis">I chose the wrong answer because I may have misunderstood binary representation concepts. The question likely required an understanding of bitwise operations or conversions.</p>
        <p class="right-answer">Correct Answer: C</p>
        <p class="skills">Skill to Improve: Binary representation and manipulation.</p>
    </div>

    <div class="question-box">
        <div class="question-header">Question 17 (Topic 3.C)</div>
        <p class="analysis">This question involved procedural abstraction. I may have misinterpreted how functions or procedures should be structured in a program.</p>
        <p class="right-answer">Correct Answer: D</p>
        <p class="skills">Skill to Improve: Understanding and writing reusable procedures.</p>
    </div>

    <div class="question-box">
        <div class="question-header">Question 22 (Topic 2.B)</div>
        <p class="analysis">This question tested binary number manipulation. I may have overlooked how binary addition or logic gates operate.</p>
        <p class="right-answer">Correct Answer: D</p>
        <p class="skills">Skill to Improve: Binary number operations.</p>
    </div>

    <div class="question-box">
        <div class="question-header">Question 23 (Topic 1.D)</div>
        <p class="analysis">I may have misunderstood debugging techniques or the identification of logical errors in a program.</p>
        <p class="right-answer">Correct Answer: B</p>
        <p class="skills">Skill to Improve: Debugging and troubleshooting strategies.</p>
    </div>

    <div class="question-box">
        <div class="question-header">Question 25 (Topic 5.A)</div>
        <p class="analysis">This question was likely about computing innovations and ethical considerations. My misunderstanding may have been in evaluating the impact of digital technologies.</p>
        <p class="right-answer">Correct Answer: C</p>
        <p class="skills">Skill to Improve: Understanding ethical implications of computing.</p>
    </div>

    <div class="question-box">
        <div class="question-header">Question 32 (Topic 3.B)</div>
        <p class="analysis">This question involved algorithm development and procedural thinking. I may have struggled with structuring algorithms efficiently.</p>
        <p class="right-answer">Correct Answer: D</p>
        <p class="skills">Skill to Improve: Algorithm structuring and efficiency.</p>
    </div>

    <div class="question-box">
        <div class="question-header">Question 35 (Topic 3.C)</div>
        <p class="analysis">This question involved abstraction within programming. I may have struggled with recognizing when and how to use functions effectively.</p>
        <p class="right-answer">Correct Answer: B</p>
        <p class="skills">Skill to Improve: Using abstraction in programming.</p>
    </div>

    <div class="question-box">
        <div class="question-header">Question 38 (Topic 5.A)</div>
        <p class="analysis">The question tested computing ethics and digital rights. I might have misunderstood how certain technologies impact user privacy.</p>
        <p class="right-answer">Correct Answer: B</p>
        <p class="skills">Skill to Improve: Digital ethics and privacy concerns.</p>
    </div>

    <div class="question-box">
        <div class="question-header">Question 48 (Topic 5.D)</div>
        <p class="analysis">This question was about cybersecurity. I may have misunderstood how to protect sensitive data online.</p>
        <p class="right-answer">Correct Answer: C</p>
        <p class="skills">Skill to Improve: Safe computing practices.</p>
    </div>

<div class="question-box">
    <div class="question-header">Question 54 (Topic 4.B)</div>
    <p class="analysis">I did not correctly interpret the impact of data compression on storage and transmission efficiency. I need to review lossless vs. lossy compression and understand when each is appropriate.</p>
    <p class="right-answer">Correct Answer: B</p>
    <p class="skills">Skill to Improve: Data compression and its effects on file size and quality.</p>
</div>

<div class="question-box">
    <div class="question-header">Question 56 (Topic 3.D)</div>
    <p class="analysis">I failed to recognize how algorithm efficiency is affected by different data structures. I need to practice analyzing the time complexity of algorithms and understanding how data structures impact performance.</p>
    <p class="right-answer">Correct Answer: D</p>
    <p class="skills">Skill to Improve: Algorithm efficiency and data structure selection.</p>
</div>

<div class="question-box">
    <div class="question-header">Question 60 (Topic 2.C)</div>
    <p class="analysis">I misinterpreted the behavior of logical operations in conditional statements. I need to work on applying De Morgan’s laws and understanding how Boolean expressions function in programming.</p>
    <p class="right-answer">Correct Answer: A</p>
    <p class="skills">Skill to Improve: Boolean logic and conditional reasoning.</p>
</div>

<div class="question-box">
    <div class="question-header">Question 61 (Topic 1.E)</div>
    <p class="analysis">I struggled to recognize an off-by-one error in a loop structure. I need to improve my debugging skills by carefully tracing loop iterations and verifying index values.</p>
    <p class="right-answer">Correct Answer: C</p>
    <p class="skills">Skill to Improve: Debugging loops and preventing off-by-one errors.</p>
</div>

<div class="question-box">
    <div class="question-header">Question 66 (Topic 5.B)</div>
    <p class="analysis">I underestimated the impact of computing innovations on accessibility and the digital divide. I need to study real-world examples of how technology can both bridge and widen societal gaps.</p>
    <p class="right-answer">Correct Answer: B</p>
    <p class="skills">Skill to Improve: Understanding the societal impact of computing innovations.</p>
</div>

<div class="question-box">
    <div class="question-header">Question 67 (Topic 3.F)</div>
    <p class="analysis">I misunderstood the role of recursion in algorithm design. I need to practice tracing recursive function calls and understanding base cases and recursive steps.</p>
    <p class="right-answer">Correct Answer: D</p>
    <p class="skills">Skill to Improve: Recursion and its application in problem-solving.</p>
</div>


    <h2 style="color: #e74c3c; margin-top: 30px;">Applying These Learnings to the AP Exam</h2>
    <p>Reflecting on this quiz, I realize that I need to focus more on procedural abstraction, algorithm development, and ethical considerations in computing. These are all essential skills for the AP Exam.</p>
    <p>To improve, I will review practice problems related to these topics, study explanations of correct answers, and ensure I understand the underlying concepts. Strengthening these areas will help me be better prepared for the AP Exam and similar assessments in the future.</p>

</body>
</html>


<hr style="border: 3px solid black;">

<h1>Strengths & Weaknesses</h1>

<table border="1" style="width: 100%; border-collapse: collapse; text-align: left;">
    <tr style="background-color: #000; color: #fff;">
        <th style="padding: 10px;">Strengths</th>
        <th style="padding: 10px;">Weaknesses</th>
    </tr>
    <tr>
        <td style="padding: 10px;"><strong>Leadership:</strong> I am able to guide a team effectively, ensuring tasks are completed efficiently.</td>
        <td style="padding: 10px;">Occasionally take extra time to fully organize tasks before starting, which can slow down workflow at times.</td>
    </tr>
    <tr style="background-color: #f2f2f2;">
        <td style="padding: 10px;"><strong>Communication:</strong> I Ccearly express ideas and listen actively to team members’ input.</td>
        <td style="padding: 10px;">Can sometimes focus too much on ambitious goals, which might take time away from the true objective.</td>
    </tr>
    <tr>
        <td style="padding: 10px;"><strong>Collaboration:</strong> Work well in the team environment, valuing different perspectives and contributing to group success.</td>
        <td style="padding: 10px;">At times, rely on last-minute efforts to finalize work, which could be improved with better time management.</td>
    </tr>
    <tr style="background-color: #f2f2f2;">
        <td style="padding: 10px;"><strong>Problem-Solving:</strong> I am able to quickly analyze challenges and find effective solutions in a structured manner.</td>
        <td style="padding: 10px;">Prefer to work independently at times after school, which may limit opportunities to seek help or delegate tasks efficiently.</td>
    </tr>
    <tr>
        <td style="padding: 10px;"><strong>Adaptability:</strong> Can adjust to new tools, workflows, or unexpected obstacles with a flexible mindset.</td>
        <td style="padding: 10px;">Occasionally take longer than necessary to transition between tasks, especially when switching focus.</td>
    </tr>
</table>

<hr style="border: 3px solid black;">


<h1 style="text-align: center; font-size: 2.5em; color: #264653;">Future Pathways in Computer Science & Beyond</h1>

<div style="display: flex; justify-content: space-around; flex-wrap: wrap; gap: 20px; padding: 20px;">

    <!-- Interests Section -->
    <div style="width: 45%; background-color: #e9c46a; padding: 15px; border-radius: 15px; box-shadow: 3px 3px 10px rgba(0, 0, 0, 0.1);">
        <h2 style="color: #533e2d; text-align: center;">Interests in Computer Science</h2>
        <p>While I may not pursue a strict Computer Science career, I’ve found aspects of this field that genuinely interest me:</p>
        <ul>
            <li><strong>Collaboration:</strong> Working in a team setting, brainstorming, and problem-solving together was engaging.</li>
            <li><strong>Logical Thinking:</strong> Breaking down complex problems and finding structured solutions was satisfying.</li>
            <li><strong>Creativity in Tech:</strong> The ability to build and design interactive projects showed how technology can be both functional and expressive.</li>
        </ul>
    </div>

    <!-- Applying CS to Other Areas -->
    <div style="width: 45%; background-color: #f4a261; padding: 15px; border-radius: 15px; box-shadow: 3px 3px 10px rgba(0, 0, 0, 0.1);">
        <h2 style="color: #533e2d; text-align: center;">Applying CS to Other Fields</h2>
        <p>Even if I don’t follow a Computer Science career, the skills learned here are widely applicable:</p>
        <ul>
            <li><strong>Problem-Solving:</strong> The ability to think critically and solve challenges applies to nearly every career field.</li>
            <li><strong>Data Organization:</strong> Understanding how data is structured helps in business, finance, and research roles.</li>
            <li><strong>Automation & Efficiency:</strong> Learning how to optimize workflows and automate tasks is useful in many industries.</li>
        </ul>
    </div>

</div>

<!-- Exploring Other Classes -->
<div style="margin-top: 30px; padding: 20px; text-align: center; background-color: #90be6d; border-radius: 15px;">
    <h2 style="color: #2d6a4f;">Exploring Other Courses</h2>
    <p>Looking ahead, I might take courses that incorporate similar problem-solving and logical thinking principles from CSP. Some possible options include:</p>
    <ul style="display: inline-block; text-align: left;">
        <li><strong>Engineering & Design:</strong> Uses computational thinking to create innovative solutions.</li>
        <li><strong>Business Analytics:</strong> Applies data structures and logic to real-world decision-making.</li>
        <li><strong>Psychology & AI:</strong> Explores how machine learning models human thought processes.</li>
    </ul>
</div>

<!-- College & Internships -->
<div style="margin-top: 30px; padding: 20px; text-align: center; background-color: #577590; color: white; border-radius: 15px;">
    <h2>College & Internship Considerations</h2>
    <p>While I may not major in CS, it remains a valuable skill set. College programs with interdisciplinary tech applications or internships in tech-adjacent fields could still be useful in broadening my career options.</p>
</div>



<hr style="border: 3px solid black;">

<h1 style="text-align: center; font-size: 2.2em; font-weight: bold; margin-bottom: 10px;">Next Steps & Reflection on MelodyMates</h1>

<div style="display: flex; justify-content: center; gap: 20px; flex-wrap: wrap; margin-top: 20px;">

    <!-- Next Steps -->
    <div style="background-color: #f0f8ff; padding: 20px; border-radius: 12px; box-shadow: 3px 3px 10px rgba(0, 0, 0, 0.1); width: 30%; min-width: 300px;">
        <h2 style="color: #0047ab; text-align: center;">Next Steps</h2>
        <ul style="line-height: 1.6;">
            <li>Enhancing <strong>feature interconnectivity</strong> to make user experiences more seamless.</li>
            <li>Improving <strong>login functionality</strong> by adding different permissions for normal users and admin users, like <strong>Thomas Edison</strong>.</li>
            <li>Refining the <strong>frontend designs</strong> to ensure a more cohesive and visually appealing interface.</li>
            <li>Expanding <strong>practicality</strong> by adding features that enhance usability for the average person.</li>
        </ul>
    </div>

    <!-- Weaknesses -->
    <div style="background-color: #fff0f5; padding: 20px; border-radius: 12px; box-shadow: 3px 3px 10px rgba(0, 0, 0, 0.1); width: 30%; min-width: 300px;">
        <h2 style="color: #a52a2a; text-align: center;">Weaknesses</h2>
        <ul style="line-height: 1.6;">
            <li>Currently, <strong>some features feel isolated</strong>, lacking a smooth connection between them.</li>
            <li>Our <strong>login system lacks admin-user differentiation</strong>, which limits access control.</li>
            <li>The <strong>design styles vary</strong> across different pages, making it less visually unified.</li>
            <li>Some features, while interesting, could be adjusted to better <strong>fit practical, everyday use</strong>.</li>
        </ul>
    </div>

</div>

<!-- Strengths (Placed Below but Horizontally Spanning) -->
<div style="display: flex; justify-content: center; margin-top: 20px;">
    <div style="background-color: #e6ffe6; padding: 20px; border-radius: 12px; box-shadow: 3px 3px 10px rgba(0, 0, 0, 0.1); width: 65%; min-width: 600px;">
        <h2 style="color: #006400; text-align: center;">Strengths</h2>
        <ul style="line-height: 1.6;">
            <li>Encourages <strong>communication and collaboration</strong> through music-sharing features.</li>
            <li>Music is a <strong>widely relevant</strong> aspect of modern culture, making the site appealing.</li>
            <li>Features <strong>dynamically update</strong> to ensure real-time interactions.</li>
            <li>The platform offers a <strong>unique and engaging</strong> way to connect over shared music interests.</li>
        </ul>
    </div>
</div>

<hr style="border: 3px solid black;">

<div class="exam-prep-section" style="background-color: #f5f5f5; padding: 25px; border-left: 8px solid #00796b; border-radius: 10px;">
    <h2 style="text-align: center; color: #00796b; font-size: 2.2em; text-transform: uppercase; font-weight: bold; margin-bottom: 15px;">
        Helping Each Other Get Final Exam Ready
    </h2>

    <p class="exam-intro" style="font-size: 1.2em; text-align: center; margin-bottom: 20px;">
        Arush Shah and I have been working together to prepare for the final exam by reviewing each other's websites and giving feedback. We did a <b>mock presentation</b> to ensure we are both ready.
    </p>

    <div style="display: flex; flex-wrap: wrap; gap: 20px; align-items: center; justify-content: center;">
        
        <!-- Left side: Arush's feedback -->
        <div style="width: 45%; background-color: #e3f2fd; padding: 20px; border-radius: 10px;">
            <h3 style="color: #0d47a1;">Arush’s Feedback on My Website</h3>
            <ul style="font-size: 1.1em; line-height: 1.6;">
                <li><b>“The blog is very streamlined and clear.”</b></li>
                <li>Creative layout makes information easy to follow.</li>
                <li>Feature meets <b>all the criteria</b> for the final review.</li>
                <li>Consider improving <b>UX (User Experience):</b></li>
                <ul>
                    <li>Use <b>fav icons</b> for edit and delete buttons.</li>
                    <li>Enable <b>in-place editing</b> instead of pop-ups.</li>
                </ul>
                <li>Overall, great feature execution and solid blog content.</li>
            </ul>
        </div>

        <!-- Right side: Studying Image -->
        <div style="width: 45%; text-align: center;">
            <img src="images/Screenshot 2025-03-02 at 7.09.17 PM.png" alt="Studying Together" style="width: 100%; border-radius: 10px; box-shadow: 3px 3px 10px rgba(0, 0, 0, 0.2);">
            <p style="font-size: 1em; color: #555; margin-top: 10px;">
                Arush and I reviewing together for the final.
            </p>
        </div>
    </div>

    <p class="exam-conclusion" style="margin-top: 20px; font-size: 1.1em; text-align: center;">
        Thanks to this feedback, I plan to refine my website’s <b>user experience</b> before the final review. Meanwhile, I also gave Arush feedback on his site to help him prepare.
    </p>
</div>


<hr style="border: 3px solid black;">


<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Self-Grade Evaluation</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f9;
            margin: 40px;
            text-align: center;
        }
        h1 {
            color: #333;
        }
        table {
            width: 90%;
            margin: 20px auto;
            border-collapse: collapse;
            background: white;
            box-shadow: 2px 2px 10px rgba(0, 0, 0, 0.1);
        }
        th, td {
            border: 1px solid #ccc;
            padding: 12px;
            text-align: left;
        }
        th {
            background-color: #4a90e2;
            color: white;
        }
        tr:nth-child(even) {
            background-color: #f9f9f9;
        }
    </style>
</head>
<body>

    <h1 style="color: #d9534f; font-size: 2.5em; font-weight: bold; text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.2);">Self-Grade Evaluation</h1>

    
    <h2>Project Execution (9/10)</h2>
    <table>
        <tr>
            <th>Component</th>
            <th>Score</th>
            <th>Analysis</th>
        </tr>
        <tr>
            <td>5 things done over 12 weeks, Issues, Burndown, Presentation</td>
            <td>4.5/5</td>
            <td>Strong execution, but scale of accomplishments and burndown tracking could have been slightly more detailed.</td>
        </tr>
        <tr>
            <td>Full Stack Project Demo (CPT requirements, N@tM feedback)</td>
            <td>1.5/2</td>
            <td>Functionality demonstrated well, but some backend elements (deployed frontend corresponding with backend data table) could be optimized.</td>
        </tr>
        <tr>
            <td>Project Feature Blog Write-up (CPT/FRQ language)</td>
            <td>1/1</td>
            <td>Effectively used AP CSP terminology and structured explanations clearly.</td>
        </tr>
        <tr>
            <td>MCQ</td>
            <td>1/1</td>
            <td>Completed correctly and demonstrated strong understanding in completion and corrections.</td>
        </tr>
    </table>

    <h2>Reflection & Engagement (1/1)</h2>
    <table>
        <tr>
            <th>Component</th>
            <th>Score</th>
            <th>Analysis</th>
        </tr>
        <tr>
            <td>Reflection on project (Next Steps, Strengths, Weaknesses)</td>
            <td>✔</td>
            <td>Clearly outlined improvements and strengths, though refining interconnectivity of features would be beneficial.</td>
        </tr>
        <tr>
            <td>Thinking about next steps in CompSci (Interests, Classes, Career, Internships, College)</td>
            <td>✔</td>
            <td>Well-explored future plans and connections between CSP and other fields.</td>
        </tr>
        <tr>
            <td>N@tM Reviews, Engagement in Other Projects</td>
            <td>✔</td>
            <td>Engaged well with other projects, providing constructive feedback and learning from peers.</td>
        </tr>
        <tr>
            <td>Helping Someone with Final Exam Prep</td>
            <td>✔</td>
            <td>Helped Arush Shah with organization and review materials.</td>
        </tr>
        <tr>
            <td>Preliminary Live Review Practice</td>
            <td>✔</td>
            <td>Practiced live review with group, improving delivery and planning.</td>
        </tr>
        <tr>
            <td>Sending Summary 24 Hours Before Live Review</td>
            <td>✔</td>
            <td>Prepared and sent a detailed summary in advance.</td>
        </tr>
        <tr>
          
            
            
        </tr>
    </table>

  <h2 style="color: #d9534f; font-size: 24px; font-weight: bold;">Final Score: ~9/10</h2>

   
</body>
</html>


<hr style="border: 3px solid black;">

