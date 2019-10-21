|<a name="start"></a>Introduction to Interactive Media (IGME-110), Fall 2019 | [Syllabus](https://lawleyfall2019.github.io/110-fall2019/) | [Schedule](https://lawleyfall2019.github.io/110-fall2019/schedule.html#week10) |
|----|----|----|


# Git Basics Exercise (Week 10, Tuesday 10/29) 

In today's exercise you'll create a GitHub account, add a new repository, clone it to your computer using Visual Studio Code, and get some practice with creating, editing, staging, committing, and syncing files. 

## Part 1: Creating a GitHub Account and Repository 

If you don't already have a GitHub account, go to https://github.com to create an account. (You can use whatever userid you'd like, it doesn't have to be your RIT ID if you don't want it to be.) 

Once your account has been created and validated, you'll be asked if you want to create a new repository. Create one called 110exercise. Make it public, and initialize it with a README. 

![Screenshot of new repo page](newRepo.png) 

You'll be taken to the main page of your new repository. Leave it open in the browser while you complete the next steps. 

## Part 2: Setting Up Git & GitHub on Your Computer

Open the GitBash program. 

Set a Git username. This is not your git login name; it's used to identify who made commits to a repository. I generally use my first and last name, but that's not necessary. (Don't type the $; that's the system prompt!)

    $ git config --global user.name "Your Name"

Check to be sure that you have set the Git username correctly:

    $ git config --global user.name
    > Mona Lisa

Repeat the process for your email address, using:

    $ git config --global user.email "your@email.com"

Close the GitBash program. 

## Part 3: Cloning the Repository to Your Computer

In the top right corner of your repository page, there's a green button that says "Clone or Download". Click that button, and you'll see a URL that you can use to clone the repository to your machine. Copy that URL. 

(Cloning creates a copy of the repository that's linked to the master version on GitHub; downloading retrieves copies of the files but doesn't link them to the original repository.) 

Launch VS Code, and from the file menu, choose View --> Command Palette. 

Type in `git:clone`. You should see that command appear below the entry box; select it, and VS Code will prompt you for the URL that you just copied from GitHub. Paste that in and press Enter. 

VS Code will prompt you for a location for your files. Once you've selected a location, VS Code will create a directory for the repository files using the name of the repository, and will retrieve copies of any files in the repository (which right now should just be the README.md file). When it's done, it will ask if you want to open the new repository (either in the current window, or in a new window). 

Here's a video showing the cloning process: https://youtu.be/hNMkIF0klow 

## Part 4: Editing Files in Your Repository

In VS Code, select the README.md file in your repository directory. This file is in a format called "[Markdown](https://guides.github.com/features/mastering-markdown/)", which allows you to do limited formatting of text documents with a much simpler syntax than HTML. (This exercise page is actually a Markdown file!)

By default, the page should have a title of 110exercise. If you added a description when you created the repository, that should appear below the title. Mine looks like this:

    1  # 110exercise
    2  Test directory for 110 GitHub exercise

Edit the file so that it has a more meaningful title, and some additional text. For example:

    1  # IGME-110 GitHub Practice
    2  This is a repository that I created in class to practice with Git and GitHub. 

Save the changes to the file. In the left sidebar of VS Code, you should now see a notification on the middle icon; VS Code knows that this is a repository, and is letting you know that your file changes haven't yet been added to the repository tracking system. Click on that icon, and you'll see the README.md file, with an M next to it. The M means the file has been modified. 

To add the changed file to your repository you need to first stage it (to tell VS Code that you want to include the changes in your next commit to the repository), and then commit it. 

To stage the file, put your cursor over its name, and click on the + next to it. The file will move from "Changes" to "Staged Changes". Add a commit message in the box at the top (e.g. 'Added new title to README'), and click on the checkmark to commit it to your repository. The changes have now been recorded. (Why the extra step of staging? Several reasons. Sometimes you might be editing a lot of files, but only a few are complete enough to be added to the repository. By staging them before you commit, you don't have to add the changed files to the repository until you're ready. Other times you may have updated a lot of files, and want different commit messages for specific groups of files.) 

While Git is now tracking the changes to the file, the changes have only been made in your local copy of the repository. Since Git is a distributed source control system, you'll need to take another step to synchronize the changes in your copy of the repository changes to the copy on GitHub. 

In the "..." menu at the top of the sidebar, choose "Sync".

Because you have to be logged in to make changes to a repository on GitHub, you should now get a GitHub login prompt. Once you've provided your GitHub login credentials, the changes you committed to your local copy of the repository will be sent to the GitHub version. In your browser, reload your repository page. You should see the modified README.md file, and next to its name in the file list you should see the commit message that you used. 

Click on the commit message, and you'll be shown the changes that were made in the file; green is content that's been added, red is content that's been deleted. It's possible to browse through all past committed versions of a file using GitHub. It's also possible to "roll back" a file to a previous commit, but that gets a bit more complicated!

## Part 5: Adding a File to the Repository

In VS Code, create a new file in the repository directory. It can be an HTML file, a Markdown (.md) file, or a text (.txt) file. Add whatever content you'd like, and then save it. 

In the Git sidebar, the new file will appear with a U next to its name (for "untracked", because it hasn't yet been committed to the repository). Stage, commit, and sync this file, too.  Reload your repository in the browser to make sure the file is visible.

## Part 6: Deliverable
Go to https://links.lawley.net/githubinfo and enter your name, your RIT user ID, your GitHub username, and the URL to the repository you just created. This should be submitted before the start of class on Thursday. 

## Note: You Can Clone to Multiple Machines!
Once you have the repository set up on GitHub, you can create clones of it on as many computers as you'd like. I usually clone the repositories I'm actively working on to my Mac, my Windows computer, and my iPad. Changes I make on one can then be retrieved from GitHub on the other devices. If you do that, it's a good idea to always start your editing session by syncing with GitHub, so you get all the changes that have been made. (And make sure to commit and sync your changes with GitHub at the end of every editing session!)


