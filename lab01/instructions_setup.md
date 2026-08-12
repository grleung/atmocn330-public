Welcome to your first lab workbook for ATM OCN 330! Today we are setting up our computing workflow for the rest of the semester.

# Goals
1. Set up your GitHub account and `atmocn330-[netid]` repository for lab submissions
2. Access AOS JupyterHub server
3. Practice pulling empty lab workbooks from `atmocn330-public` repository
4. Practice pushing your submission to `atmocn330-[netid]` and submitting to Canvas

# Overview
We will always use the AOS JupyterHub for executing code in this course. This makes our lives easier by ensuring we're all using the same code environments.

There are two GitHub repos that are relevant for this course. First, the public class repo is `atmocn330-public`, which contains the empty lab workbooks for each week. Second, each of you will set-up your own private repo called `atmocn330-[netid]`, which you will use to turn in your labs.

# Part 1: GitHub set-up
1. If you don't already have one, create a GitHub account.
2. From the GitHub website, make a new **private** repository. Name it `atmocn330-[netid]`, and replace `[netid]` with your NetID (e.g., `gleung3`). Select Visibility: Private. Don't check the "Add a README file". 
3. On the link for your new private repo, go to Settings > Collaborators > Add people. Add Bee (`@grleung`) and Kiran ([@username]) so we can check your submissions. 
4. Log into the AOS JupyterHub (go to `https://jupyterhub.aos.wisc.edu:1225` in your browser, and use log-in details from Pete) and open a new Terminal.
5. Set up your GitHub SSH key. This allows you to access files from your GitHub on our JupyterHub without typing your passcode every time. Generate a new key on the JupyterHub:

    ```ssh-keygen -t ed25519 -C "[your_email@wisc.edu]"```
    
    Press `Enter` three times to accept all the defaults without setting a password. Print your public key using:
    
    ```cat ~/.ssh/id_ed25519.pub```
    
    Copy the entire printed line (starting with `ssh-ed25519`) and paste it on your GitHub account under Settings > Access > SSH and GPG keys > Add new SSH Key. Call it something like `UW JupyterHub`.

6. Set up username, etc. for commit messages. I usually run:
    ~~~
    git config --global user.name "Your Name"
    git config --global user.email "your_email@wisc.edu"
    git config --global init.defaultBranch main 

7. On your JupyterHub terminal, clone your private repo

    ```git clone git@github.com:[your-gh-username]/atmocn330-[netid].git```

    You can find the relevant link by clicking on the green "<> Code" button on your GitHub repository, and going to Local > SSH. This will create a new directory that you should navigate into using ```cd atmocn330-[netid]```. 

8. Add the public lab repo as an upstream branch

    ```git remote add upstream git@github.com:grleung/atmocn330-public.git```

    This links your repo to Bee's public repo so you can download future labs.

9. Pull the starter files.

    ```git pull upstream main```
 
     If this worked properly, you should now see a sub-directory called `lab01` in your `atmocn330-[netid]` directory!

*Note: You should ideally reach this point within 30-35 minutes. If you run into an error or get stuck for more than 5 minutes on one step, raise your hand so Bee or Kiran can help you debug!*

# Part 2: Complete `lab01_setup.ipynb`
In your JupyterHub file browser, open the `lab01` folder and launch `lab01_setup.ipynb` to complete today's assignment.