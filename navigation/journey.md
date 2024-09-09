---
layout: blogs
title: Journey
search_exclude: true
permalink: /blogs/
---

# My Coding Journey

## Tools and Setup

---

### Terminal & File Management

Using the **Linux terminal** was essential for navigating and managing my project files. Some of the key commands I used were:  
- `cd` – change directory  
- `mkdir` – create a folder  
- `ls` – list files  

These commands were crucial for keeping my project organized and efficient.

---

### Installing Developer Tools with Ubuntu Linux

I installed necessary developer tools using Ubuntu's **apt** package manager. Key commands I used include:  
- `sudo apt update` – updates the package list  
- `sudo apt install <package_name>` – installs specific tools like Python and Ruby

---

### Setting Up Python Environment

To keep my project dependencies organized, I set up a **virtual environment** for Python:  
- `python3 -m venv venv` – creates an isolated environment  
- `source venv/bin/activate` – activates the environment

This helped me keep my project dependencies separate from the system's global packages.

---

![Ubuntu Image](https://ubuntu.com/wp-content/uploads/a9c1/Screenshot-from-2022-04-18-13-05-17-min.png)

---

### Installing Python Packages

With the virtual environment active, I used `pip` to install the necessary packages for my project:  
- `pip install -r requirements.txt` – installs everything listed in the requirements file

---

### Ruby and Jekyll Setup

To run **Jekyll** for GitHub Pages, I installed the required **Ruby gems** using:  
- `bundle install` – installs the necessary Ruby packages  
This set up my local environment for creating and testing the website.

---

### Launching the Local Server

I used the command `make` to run the local server, allowing me to preview my website at `http://127.0.0.1:4000`. This was crucial for testing changes before pushing them live.

---

### Syncing with GitHub

After making updates, I saved my changes using Git:  
- `git commit -m "insert message"` – commits my changes  
- `git push` – pushes the changes to the remote repository

GitHub Pages then automatically rebuilds the site with the new changes.

---

This journey has helped me understand the importance of organization and attention to detail in coding projects.
