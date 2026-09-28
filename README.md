# A02

## Part 1: How to use VS Code

- VS Code is the code editor that most programmers use and some may say is the industry standard.
- Luckily its easy to get started with it. VS Code prides itself on is its beginner friendliness and ease of use.

### Download VS Code

1. Download VS Code with the following website and click the big download button in the middle. Download link: https://code.visualstudio.com/

2. Run the .exe file you installed and follow the installation prompts

3. You should have VS Code downloaded! Open VS Code but searching it up on your machine and open the application.

### How to get started with using VS Code

- VS Code is a code editor with a ton of features so it can be little overwhelming at the start. Luckily, VS Code provides a step by step onboarding feature that walks you through all of the main features you will most likely use. It is really recommended to complete these walkthroughs!

- If you are one that prefers to read about how to do things, I recommend reading the following website on how to get started with VS Code which is written by VS Code themselves. Link: https://code.visualstudio.com/docs/editing/getting-started/editor-tutorial

- If you are one that preferes watching videos, I recommend this video by VS Code themselves that walks you through VS Code and its features! Link: https://youtu.be/f8_uF_IDV50?si=Asuoxh37FXGf_Ld5

## How to use Git and Github

- **Git** and **Github** are one of the most important tools any software developer should know. Git is a tool that allows you to have verison control on your files. You can think of it like the history feature on google docs. If you break something, you can go back to an older version. GitHub is a website where you can store your Git projects online. It lets you back up your work, share it, and team up with other people.

- Now there is more to Git and Github than just that. In fact, Git and Github are one of the more confusing tools to use and it troubles a lot of begineer programmers. Luckily, since they are both so widely used and considered industry standard for the most part, there are a ton of resources online to help you!

- I recommend using this website which is a tutorial that walks you through how to use Git and Github that is made by Github themselves. Link: https://docs.github.com/en/get-started/git-basics/set-up-git

### Install Git

- Install git from the following website. Link: https://git-scm.com/install/windows

- Run the .exe file you downloaded and go through the installation prompts

- Check if it works by search for the git bash application and running the following command to see what version of git you have. Command: git --version

### Configure Github

- Git needs to know who you are so it can label your changes.

- Run the following commands in git bash. Change "your name" to your actual name and "your email" to the same email you plan to use for GitHub. 

- Command: git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"

### Get Started with Github

- Make a Github account on https://github.com

- Create your **remote** **repository** which just a project folder that Git keeps track of.
    - Log in and click the + in the top right corner.
    - Click New repository. 
    - Give it a name and then click Create repository.

- **Cloning** the repo which means just downloading a copy of the repo to your machine.
    - before this you have to setup your ssh keys which is its own thing. Please use the following link to set them up and them come back. Link: https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent
    - On your repo's GitHub page, click the green Code button and copy the SSH link.
    - In git bash, go to the folder where you want the project using the cd command and run the following command. Command: git clone "copied ssh link"
    - you should see a new folder with the same name as your repo.

- In your code editor of your choice, Open the folder and start making changes like edit or create a file.

- Next, you have to stage your changes which means you're picking which changes you want to save. Use the following command
    - Command: git add filename of file you want to save
    - To add everything at once, use the following command. Command: git add .

- Next, you have to **commit** your changes. This is where you are doing the actual saving part. You always have to add a short message explaining what you did. Use the following command. Command: git commit -m "message"

- Next, you want to upload the local changes to Github. In order to do this, you have to **push** your commits to Github using the following command. Command: git push
    - If you refresh your Github repo you should see your new changes.

- If someone else changed the project, you need to download those changes. In order to do this, you have to **pull** the changes from the Github repo to your local machine using the following command. Command: git pull
    - Note that git pull automatically merges any new changes to your local files (merging talked about later). If you don't want that but still want to be up to date, then you have **fetch** the changes from the Github repo using the following command. Command: git fetch

- If you want to play around with your project but don't want to change the main version, use **branches**.
    - To create a new branch and switch to it, use the following command. Command: git checkout -b branchname

- If you want to combine a branch you were working on with your main branch you have to do what we call a **merge**. Now Git automatically combines the code from the two branches but sometimes it can't. We call that a **merge conflict**. 
    - To merge a new branch to your main branch, run the following command from your main branch and then push it. Command: git merge newBranch

## Part 2: Glossary:

- Branch: Branches are like a separate workspace where you can make changes and try new ideas without affecting the main version of a project.
- Clone: Command used to download a copy of a specific repository or branch within a repository on your local machine.
- Commit: Command that acts like a save option on a document. Rememeber that it always needs a message.
- Fetch: Command that retrieves the latest commits from the remote repository, but it does not affect the local working directory.
- GIT: A version control system for files.
- Github: A platform that builds on Git by hosting your Git projects, called repositories, in the cloud, as well as adding other tools that make it easier for teams to work together.
- Merge: Command that combines changes from different branches into a single branch.
- Merge Conflict: An event that occurs when Git is unable to automatically combine code changes from two different branches.
- Push: Command used to upload your local repository commits to a remote repository
- Pull: Command used to download changes from a remote repository, like Github and immediately integrate them into your local working branch.
- Remote: A version of your project that is hosted on the internet or a server instead of your local computer.
- Repository: A place where you can store your code, your files, and each file's revision history.