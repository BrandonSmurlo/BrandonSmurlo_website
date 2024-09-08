---
layout: blogs 
title: Journey
search_exclude: true
permalink: /blogs/
---

tools and setup

# TERMINAL & FILE MANAGEMENT
I used the Linux terminal to navigate and manage files. Commands like `cd` (change directory), `mkdir` (create folder), and `ls` (list files) were crutial for moving through and organizing my project files.

# INSTALLING DEVELOPER TOOLS WITH UBUNTU LINUX
Ubuntu’s `apt` package manager was used to install tools like Python and Ruby. Key commands used:  
- `sudo apt update` – to update the package list  
- `sudo apt install <package_name>` – to install necessary packages  

# SETTING UP PYTHON ENVIRONMENT
After setting up Python, I created a virtual environment for my project using:  
- `python3 -m venv venv` – sets up an isolated environment  
- `source venv/bin/activate` – activates it  
This keeps project dependencies organized and separate from global packages.

![Ubuntu Image](https://ubuntu.com/wp-content/uploads/a9c1/Screenshot-from-2022-04-18-13-05-17-min.png)

# INSTALLING PYTHON PACKAGES
With the virtual environment active, I used `pip` to install required packages:  
- `pip install -r requirements.txt` – installs everything from my project’s requirements file.

# RUBY AND JEKYLL SETUP
To run Jekyll (for GitHub Pages), I installed Ruby gems:  
- `bundle install` – grabs the necessary Ruby packages.  
This sets up my local Jekyll environment for creating the website.

# LAUNCHING THE LOCAL SERVER
I ran the local server with the command `make`. This let me view my website at `http://127.0.0.1:4000`, making it easy to check updates before pushing them live.

# SYNCING WITH GITHUB
After changes are made, I saved and committed them to Git:  
- `git commit -m "insert message"`  
I pushed my commits with `git push` to update the remote repository. GitHub Pages will automatically rebuild the site with my changes.