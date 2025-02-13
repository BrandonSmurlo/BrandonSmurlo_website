---
layout: base
title: Student Home 
description: Home Page
hide: true
---

<div class="header" style="text-align: center; padding: 20px; background-color: #f0f8ff; border-radius: 12px;">
   <h1 style="color: #4B0082; font-family: 'Poppins', sans-serif; font-size: 48px; letter-spacing: 2px; text-shadow: 2px 2px #8A2BE2;">
      Brandon Smurlo
   </h1>
   <h2 style="color: #8A2BE2; font-family: 'Poppins', sans-serif; font-size: 32px; letter-spacing: 1.5px; text-shadow: 1px 1px #4B0082;">
      Home Page
   </h2>
</div>



<div style="display: flex; justify-content: center; gap: 20px; padding: 20px;">
   <div style="text-align: center;">
      <a href="notebook1" style="text-decoration: none;">
         <button class="animated-button" style="background-color: #4CAF50; color: white; border: none; padding: 15px 30px; font-size: 16px; border-radius: 8px; cursor: pointer;">
            notebook 1
         </button>
      </a>
   </div>

   <div style="text-align: center;">
      <a href="notebook2" style="text-decoration: none;">
         <button class="animated-button" style="background-color: #2196F3; color: white; border: none; padding: 15px 30px; font-size: 16px; border-radius: 8px; cursor: pointer;">
            notebook 2
         </button>
      </a>
   </div>

   <div style="text-align: center;">
      <a href="notebook3" style="text-decoration: none;">
         <button class="animated-button" style="background-color: #f44336; color: white; border: none; padding: 15px 30px; font-size: 16px; border-radius: 8px; cursor: pointer;">
            notebook 3
         </button>
      </a>
   </div>
</div>

<style>
   .animated-button {
      transition: transform 0.3s ease, box-shadow 0.3s ease;
   }

   .animated-button:hover {
      transform: translateY(-5px);
      box-shadow: 0px 8px 15px rgba(0, 0, 0, 0.3);
   }
</style>




<style>
  img {
    position: fixed;
    bottom: 0;
    left: 0;
    width: 100px;
    height: 150px;
    animation: walk 10s linear infinite;
  }
  @keyframes walk {
    from { transform: translateX(-100%); }
    to { transform: translateX(100vw); }
  }
</style>

<div class="section">
    <p>MCQ Blog + Sprint 3 Reflection</p>
    <button class="custom-button" onclick="location.href='mcq_blog.html'">MCQ Blog + Sprint 3 Reflection</button>
</div>

<!-- Placeholder link for creating the mcq_blog.html file -->
<a href="mcq_blog.md" style="display:none;">Create mcq_blog.html</a>

<style>
    .custom-button {
        padding: 10px 20px;
        font-size: 16px;
        color: white;
        background-color: #007BFF; /* Button color */
        border: none;
        border-radius: 5px;
        cursor: pointer;
        transition: background-color 0.3s ease;
    }

    .custom-button:hover {
        background-color: #0056b3; /* Hover color */
    }
</style>






<style>
  img {
    position: fixed;
    bottom: 0;
    left: 0;
    width: 100px;
    height: 150px;
    animation: walk 10s linear infinite;
  }
  @keyframes walk {
    from { transform: translateX(-100%); }
    to { transform: translateX(100vw); }
  }
</style>

<div class="section">
    <p>Sprint 5 Review Blog</p>
    <button class="custom-button" onclick="location.href='review_blog.html'">Sprint 5 Review Blog</button>
</div>

<!-- Placeholder link for creating the mcq_blog.html file -->
<a href="review_blog.md" style="display:none;">Create review_blog.html</a>

<style>
    .custom-button {
        padding: 10px 20px;
        font-size: 16px;
        color: white;
        background-color: #007BFF; /* Button color */
        border: none;
        border-radius: 5px;
        cursor: pointer;
        transition: background-color 0.3s ease;
    }

    .custom-button:hover {
        background-color: #0056b3; /* Hover color */
    }
</style>



<style>
  img {
    position: fixed;
    bottom: 0;
    left: 0;
    width: 100px;
    height: 150px;
    animation: walk 10s linear infinite;
  }
  @keyframes walk {
    from { transform: translateX(-100%); }
    to { transform: translateX(100vw); }
  }
</style>

<div class="section">
    <p>Deployment Blog</p>
    <button class="custom-button" onclick="location.href='collegeboard_vids.html'">Deployment Blog</button>
</div>

<!-- Placeholder link for creating the mcq_blog.html file -->
<a href="collegeboard_vids.md" style="display:none;">Create collegeboard_vids.html</a>

<style>
    .custom-button {
        padding: 10px 20px;
        font-size: 16px;
        color: white;
        background-color: #007BFF; /* Button color */
        border: none;
        border-radius: 5px;
        cursor: pointer;
        transition: background-color 0.3s ease;
    }

    .custom-button:hover {
        background-color: #0056b3; /* Hover color */
    }
</style>



<div class="section">
   <p>Fun Button</p>
   <button class="custom-button">Fun Button</button>
</div>

<div class="section">
   <p>Fishing Sites:</p>
   <a href="https://www.basspro.com/shop/en#" style="text-decoration: none;">
      <button class="custom-button">BassPro</button>
   </a>
   <a href="https://www.basspro.com/l/casting-rods" style="text-decoration: none;">
      <button class="custom-button">Casting Rods</button>
   </a>
</div>

<style>
  .section {
    border: thin solid black;
    margin: 20px auto;
    padding: 20px;
    text-align: center;
    width: 60%; /* Adjust this value for desired width */
    background-color: #f9f9f9;
    border-radius: 8px;
  }

  .section p {
    margin-bottom: 10px;
    font-size: 18px;
    color: black;
  }

  .custom-button {
    padding: 12px 24px;
    font-size: 16px;
    border: 2px solid black;
    border-radius: 8px;
    background-color: white;
    color: black;
    cursor: pointer;
    transition: background-color 0.3s ease, color 0.3s ease;
  }

  .custom-button:hover {
    background-color: black;
    color: white;
  }

  a {
    margin-left: 10px;
  }
</style>


[![Mario walking](https://images-wixmp-ed30a86b8c4ca887773594c2.wixmp.com/f/4ddabef1-8390-424a-a828-f61e4df3d499/daraj8q-744f0563-d3f2-4a25-98a7-377abba7dc7b.gif?token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJ1cm46YXBwOjdlMGQxODg5ODIyNjQzNzNhNWYwZDQxNWVhMGQyNmUwIiwiaXNzIjoidXJuOmFwcDo3ZTBkMTg4OTgyMjY0MzczYTVmMGQ0MTVlYTBkMjZlMCIsIm9iaiI6W1t7InBhdGgiOiJcL2ZcLzRkZGFiZWYxLTgzOTAtNDI0YS1hODI4LWY2MWU0ZGYzZDQ5OVwvZGFyYWo4cS03NDRmMDU2My1kM2YyLTRhMjUtOThhNy0zNzdhYmJhN2RjN2IuZ2lmIn1dXSwiYXVkIjpbInVybjpzZXJ2aWNlOmZpbGUuZG93bmxvYWQiXX0.KpbFWvWcQbuGNwF9TtupLcDKwLRFW8DAZLx404K5bAU)](shhh.html)




<style>
 img {
   position: fixed;
   bottom: 0;
   left: 0;
   width: 120px;
   height: 120px;
   animation: walk 10s linear infinite;
 }
 @keyframes walk {
   from { transform: translateX(-100%); }
   to { transform: translateX(100vw); }
 }
</style>


<div style="display: flex; justify-content: center; gap: 20px; padding: 20px;">
   <a href="calculator" style="text-decoration: none;">
      <button class="animated-button" style="background-color: #000080; color: white; border: none; padding: 15px 30px; font-size: 16px; border-radius: 8px; cursor: pointer;">
         Calculator
      </button>
   </a>

   <a href="snake game" style="text-decoration: none;">
      <button class="animated-button" style="background-color: #800080; color: white; border: none; padding: 15px 30px; font-size: 16px; border-radius: 8px; cursor: pointer;">
         Snake Game
      </button>
   </a>

   <a href="cookie clicker" style="text-decoration: none;">
      <button class="animated-button" style="background-color: #964B00; color: white; border: none; padding: 15px 30px; font-size: 16px; border-radius: 8px; cursor: pointer;">
         Cookie Clicker
      </button>
   </a>
</div>

<div style="display: flex; justify-content: center; gap: 20px; padding: 20px;">
   <a href="emojis" style="text-decoration: none;">
      <button class="animated-button" style="background-color: #FFC0CB; color: white; border: none; padding: 15px 30px; font-size: 16px; border-radius: 8px; cursor: pointer;">
         Emojis
      </button>
   </a>

   <a href="Interactive Map" style="text-decoration: none;">
      <button class="animated-button" style="background-color: #FFA500; color: white; border: none; padding: 15px 30px; font-size: 16px; border-radius: 8px; cursor: pointer;">
         Interactive Map
      </button>
   </a>

   <a href="Recipe Maker" style="text-decoration: none;">
      <button class="animated-button" style="background-color: #3c9dd0; color: white; border: none; padding: 15px 30px; font-size: 16px; border-radius: 8px; cursor: pointer;">
         Recipe Maker
      </button>
   </a>
</div>
