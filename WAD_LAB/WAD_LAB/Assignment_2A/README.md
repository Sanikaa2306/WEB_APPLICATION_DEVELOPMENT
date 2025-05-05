Step-by-Step Procedure:

1. Create a GitHub Account
   Go to https://github.com
   Click on Sign Up and fill in the required details.
   Verify your email and set up your profile.

2. Install Git (if not already installed)
   For Windows: Download from https://git-scm.com
   For Linux: Use the command : sudo apt install git

3. Configure Git for the First Time
   git config --global user.name "Your Name"
   git config --global user.email "your.email@example.com"

4. Create a New Repository on GitHub
   Log in to GitHub.
   Click on New Repository.
   Provide a repository name, choose visibility (Public/Private), and click Create Repository.

5. Initialize a Local Git Repository
   mkdir my-project
   cd my-project
   git init

6. Add Files and Commit Changes
   touch index.html (add basic code in it, can insert given index.html in created folder)
   git add .
   git commit -m "Initial commit"

7. Link Local Repository to GitHub
   git remote add origin https://github.com/yourusername/your-repository.git

8. Push Code to GitHub
   git push origin main
