---
layout: base
title: Planning Document
description: Planning
hide: true
---
## Planning Document

<div style="border: 2px solid #4CAF50; border-radius: 10px; padding: 15px; background-color: #f9f9f9;">
   <h2>Project Planning</h2>
   <p>Use this notebook to outline your project's objectives, tasks, and milestones.</p>
   
   <button onclick="document.getElementById('planning-info').style.display='block'" style="background-color: #4CAF50; color: white; border: none; padding: 10px 20px; font-size: 16px; border-radius: 5px; cursor: pointer;">
      Show More Info
   </button>
   
   <div id="planning-info" style="display: none; margin-top: 10px;">
      <p>Here you can detail the project phases and track progress.</p>
      <ul>
         <li>Define Objectives</li>
         <li>Plan Milestones</li>
         <li>Assign Tasks</li>
         <li>Monitor Progress</li>
      </ul>
   </div>
</div>

<script>
   // Example JS function to show/hide additional information
   function toggleInfo() {
      var info = document.getElementById('planning-info');
      info.style.display = (info.style.display === 'none' || info.style.display === '') ? 'block' : 'none';
   }
</script>
