# Renton Technical College CSI-244
<br />    

<div align="center">  
    <img src="logo.jpg" alt="Logo">
    <h3 align="center">Guided Activity 1</h3>
</div>

This repository is a part of CSI-244 at Renton Technical College.

## Part 1 Using the Command Line
We will complete the first Guided Activity together in class.

1. Clone the repository to your local machine.
2. Make note of the folder where you cloned the repository.
3. Launch powershell by hitting the windows key and typing `powershell` and then hit enter.
4. Once inside of powershell you can view your current directory with the `pwd` command. This stands for print working directory.
5. You can view the contents of the current directory with the `ls` command
6. In order to change to a different working directory you can use the `cd` command. This stands for change directory.
7. `cd` can be used to go to a specific folder, for example.

    ```powershell
    cd c:\RTC\CSI-244\Week1\
    ```
8. `cd` can also be used to back out of a folder. `cd ..` will take you up one folder. For example if you are currently in c:\Users\Jemery the `cd..` command will take you to c:\Users\

    ```powershell
    cd ..
    ```

9. `cd ~` will take you to what is referred to as the home folder. This is your windows users folder located at C:\Users\YourUserName\
10. `cd \` will take you to the root folder of your hard drive or C:\
11. When using cd to change folders you can use the `tab` key to auto complete a command. For Example let's say I wanted to navigate to C:\RTC\CSI-244\Week1\. I could start by typing `cd C:\R` and then hit `tab`. Powershell will try to find a Folder inside of C:\ that begins with the letter R. If none exists there will be no suggestion, if more than one exists than it will choose the first alphabetically. I can then repeat the processs for an folders within C:\RTC\
12. This will vary based on your file structure but my command could look something like this cd c:\R `tab to complete` Then type C `tab to complete` then W `tab to complete`
13. Getting used to this takes some time but it is a huge time saver and will cut down on typos.
14. After you have cloned this repository navigate to your local repository using the cd command.
15. Open the repository in Visual Studio Code by typing `code .`
16. Open the terminal in Visual Studio Code by hitting ctrl + \` or cmd + \` on mac.
17. This is powershell running inside of Visual Studio Code.
18. Create a new folder called myfiles with the `mkdir` command (make directory)

    ```powershell
    mkdir myfiles
    ```
19. Run the ls (list) command to see your newly created folder.
20. cd into the myfiles directory

    ```powershell
    cd myfiles
    ```
21. Create a new text file using the terminal. This command will create a new file named hello.txt

    ```powershell
    new-item hello.txt
    ```
22. To open the new text file inside of visual studio code type

    ```powershell
    code hello.txt
    ```

23. Inside of the file type your name and save the file.
24. Go back to the terminal and type `cat hello.txt`.
25. Notice that your name has been displayed in the console.
26. When making a github commit via the command line make sure to back out to the repository folder before creating the commit.

    ```powershell
    cd ..
    ```
27. You should now be back inside of the root folder of the repository. If you are not sure you can always check first by typing

    ```powershell
    pwd
    ```

## Part 2 Intro To GitHub

**Welcome to GitHub: A Beginner's Guide**

GitHub is a platform where you can store and collaborate on your coding projects. It's like a big shared folder where you and others can work together on code.

**Repository:**

Think of a repository (repo for short) as a folder for your project. It's where you store all your files and keep track of changes. Each project on GitHub has its own repository.

**Local Repository:**

Think of your local repository as the version of your project that exists on your own computer. When you're coding, making changes, and saving them, you're doing all of that within your local repository. It's like your own personal workspace.

**Remote Repository:**

The remote repository, on the other hand, is the version of your project that lives on GitHub's servers. It's the central hub where everyone on your team can collaborate and share their work. When you push your changes to GitHub, you're updating the remote repository with the latest version of your project.

**Commit:**

When you make changes to your files in the repository, you have to save those changes. This is called a commit. It's like taking a snapshot of your project at a certain point in time.

**Git add command:**

Before you make a commit, you have to tell Git which changes you want to include. This is where the `git add` command comes in. You use it to tell Git, "Hey, I want to include these changes in my next commit." It's like putting your files into a basket before you check out at the grocery store.

**Push:**

Once you've made some commits and you're happy with your changes, you can push them to GitHub. This means you're sending your changes from your computer to the GitHub server so others can see them.

**Pushing Changes:**

When you've made changes to your project in your local repository and you're ready to share those changes with your team or make them available to the public, you use the `git push` command. This command sends your committed changes from your local repository to the remote repository on GitHub.

- **Local Repository:** After you push your changes, your local repository remains unchanged. It still contains all the changes you've made, but now they're also reflected in the remote repository.

- **Remote Repository:** The remote repository gets updated with the changes you've pushed from your local repository. Once the push is successful, anyone with access to the remote repository on GitHub can see and access the latest version of your project.

So, in essence, pushing changes from your local repository to the remote repository is like updating the master copy of your project on GitHub, making your changes accessible to everyone collaborating on the project.

So, to sum up:
- **Repository**: Your project's folder on GitHub.
- **Commit**: Saving changes to your project.
- **Push**: Sending your commits to GitHub.
- **Pull**: Getting changes from GitHub to your computer.
- **Git add**: Putting changes into the commit basket.

1. First make sure that you are in the ROOT folder of your project.
2. Type `git add .` to stage all updated files.
3. Type `git status` to view all staged files.
    - You should see a list of files that you modified in part 1. These files are about to be pushed up to the remote repository.
5. Type `git commit -m "Part 1 Complete"`.
    - Now we have made a commit (a save) on our local repository. This has not been reflected on the remote repository yet.
7. Type `git push` to push the changes to GitHub.
    - This step will send our changes to the remote repository. Now if you go to your online repository at GitHub.com you will see your changes reflected.

## Part 3 Installing NVM and Node

1. Install NVM for your operating system. Windows users (https://github.com/coreybutler/nvm-windows/releases/download/1.1.11/nvm-setup.exe) Mac Users: https://dev.to/ajeetraina/how-to-install-and-configure-nvm-on-mac-os-5fgi
2. Once NVM is installed type nvm at your terminal. You should see a list of commands.
3. Type `nvm install latest` - This will install the latest version of NodeJS on your machine.
4. Type `nvm use latest`, take a screenshot of the output and add to the screenshots folder. 
5. With the latest version of NodeJS added you should now be able to run Nodel commands from the terminal.
6. Type `node --version` - A version of node should be printed to the terminal.

7. With node installed, lets try it out. For Windows, type `new-item helloworld.js` to create a new file.  For Mac, type `touch hellworld.js` to create a new file.
8. Type `code helloworld.js` to open the new file in visual studio code.
9. Add the following code to hellworld.js and save the file

    ```javascript
    console.log("Hello from helloworld.js");
    ```

11. Now from the terminal run `node helloworld.js`
12. Notice that you have now run JavaScript code outside of the web browser. This is what NodeJS allows us to do.

13. Type `git add .` to stage all updated files. 
14. Type `git commit -m "Guided Activity 1 Complete"`.
15. Type `git push` to push the changes to GitHub.

If you have any questions about this assignment please reach out to myself or our TA for this course.
