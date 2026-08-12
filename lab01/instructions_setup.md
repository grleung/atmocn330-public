Welcome to your first lab workbook for ATM OCN 330! Today we are setting up our computing workflow for the rest of the semester.

# Goals
1. Access AOS JupyterHub server
2. Practice pulling empty lab workbooks from `atmocn330-public` repository
3. Practice exporting your lab workbook as PDF and submitting to Canvas

# Overview
We will always use the AOS JupyterHub for executing code in this course. This makes our lives easier by ensuring we're all using the same code environments.

All the empty lab workbooks for this course will be on `atmocn330-public`. You won't need to set up a GitHub account for this course since the repository is public!

# Part 1: Download lab workbooks
1. Log into the AOS JupyterHub. Go to `https://jupyterhub.aos.wisc.edu:1225` in your browser, and use log-in details from Pete.
2. Open the Launcher, scroll to the bottom, and open a new Terminal.
3. Clone the lab repository:

    ```git clone https://github.com/grleung/atmocn330-public.git```
   
     If this worked properly, you should now see a directory called `atmocn330-public` on the left-hand side file browser.
4. Check the file directory is there:
   ```ls atmocn330-public```

   There should be a directory named `lab01`. 

*Note: You should ideally reach this point within 15-20 minutes. If you run into an error or get stuck for more than 5 minutes on one step, raise your hand so Bee or Kiran can help you debug!*

# Part 2: Complete `lab01_setup.ipynb`
In your JupyterHub file browser (left hand side), double click on the `atmocn330-public` folder, then the `lab01` folder, and click on `lab01_setup.ipynb` to complete today's assignment.