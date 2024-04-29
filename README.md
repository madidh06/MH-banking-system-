# MH-banking-system-elite 102 

# Step 1: Initial Setup

# This code sets up the initial environment on Replit and initializes a new GitHub repository.

# Import necessary libraries
import os
import subprocess

# Function to initialize GitHub repository
def initialize_github_repo():
    # Change directory to the project folder
    os.chdir("/home/runner/your-repl-name")  # Replace "your-repl-name" with your Repl name
    
    # Initialize a new GitHub repository
    subprocess.run(["git", "init"])
    subprocess.run(["git", "add", "."])
    subprocess.run(["git", "commit", "-m", "Initial commit"])
    
    # Add your GitHub repository URL here
    github_repo_url = "https://github.com/your-username/your-repo-name.git"  # Replace with your GitHub repo URL
    
    # Add the remote origin
    subprocess.run(["git", "remote", "add", "origin", github_repo_url])
    
    print("GitHub repository initialized successfully.")

# Call the function to initialize GitHub repository
initialize_github_repo()
