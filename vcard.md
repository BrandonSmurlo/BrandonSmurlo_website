---
layout: base 
title: vCard
search_exclude: true
comments: True
---

<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Brandon Smurlo - vCard</title>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@600&display=swap" rel="stylesheet" />
  <style>
    body {
      background-color: #e0f7fa;
      font-family: 'Segoe UI', sans-serif;
      margin: 0;
      padding: 2rem;
    }
    .container {
      display: flex;
      gap: 2rem;
      background-color: transparent;
      max-width: 1100px;
      width: 100%;
      margin: 0 auto;
    }
    .card {
      background: #fff;
      border: 2px solid #ea6d6d;
      border-radius: 12px;
      padding: 2rem;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
    }
    .left-card {
      width: 600px;
      align-items: flex-start;
      word-wrap: break-word;
      overflow-wrap: break-word;
    }
    .left-card h1 {
      font-family: 'Orbitron', sans-serif;
      color: #ea6d6d;
      font-size: 1.8rem;
      margin-bottom: 1rem;
    }
    .links {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 0.75rem;
      width: 100%;
    }
    .links a {
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      color: #1a0dab;
      text-decoration: underline;
      font-weight: 500;
      white-space: nowrap;
      overflow: hidden;
      text-overflow: ellipsis;
      max-width: 100%;
      transition: color 0.3s ease, text-decoration-thickness 0.3s ease;
      text-decoration-thickness: 1px;
    }
    .links a:hover,
    .links a:focus {
      color: #0b0080;
      text-decoration-thickness: 2px;
      cursor: pointer;
    }
    .download {
      margin-top: 1.5rem;
      padding: 0.75rem 1.5rem;
      background-color: #ea6d6d;
      color: white;
      font-weight: bold;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      text-decoration: none;
      align-self: center;
    }
    .qr-code {
      width: 240px;
      height: auto;
      margin-top: 1rem;
    }
  </style>
</head>
<body>
  <div class="container">
    <!-- Left Card -->
    <div class="card left-card">
      <h1>Brandon Smurlo</h1>
      <div class="links">
        <a href="mailto:brandonsmurlo11@gmail.com" target="_blank" rel="noopener noreferrer">
          <img src="https://upload.wikimedia.org/wikipedia/commons/4/4e/Gmail_Icon.png" width="20" alt="Email Icon" />
          brandonsmurlo11@gmail.com
        </a>
        <a href="https://tvick22.github.io/ShotSpot/" target="_blank" rel="noopener noreferrer">
          <img src="https://cdn-icons-png.flaticon.com/512/54/54481.png" width="20" alt="Website Icon" />
          Project Website
        </a>
        <a href="https://www.linkedin.com/in/brandon-smurlo-550679365/" target="_blank" rel="noopener noreferrer">
          <img src="https://cdn-icons-png.flaticon.com/512/174/174857.png" width="20" alt="LinkedIn Icon" />
          LinkedIn
        </a>
        <a href="https://github.com/BrandonSmurlo/BrandonSmurlo_website" target="_blank" rel="noopener noreferrer">
          <img src="https://cdn-icons-png.flaticon.com/512/25/25231.png" width="20" alt="GitHub Icon" />
          GitHub
        </a>
      </div>
      <a class="download" href="ocs.vcf" download>Download vCard</a>
    </div>

    <!-- Right Card -->
    <div class="card">
      <img class="qr-code" src="images/frame.png" alt="QR Code" />
    </div>
  </div>
</body>
</html>
