|<a name="start"></a>Introduction to Interactive Media (IGME-110), Fall 2019 | [Syllabus](https://lawleyfall2019.github.io/110-fall2019/) | [Schedule](https://lawleyfall2019.github.io/110-fall2019/schedule.html#week10) |
|----|----|----|

# GitHub Pages Exercise (Week 10, Thursday)

As discussed in the readings, and in lecture, GitHub provides the ability to publish a basic website from a repository. In this exercise, you’ll learn how to create a website associated with your GitHub username, as well as how to create one associated with a specific project/repository.</p>

***Do NOT start this exercise until you have successfully completed the exercise from Tuesday***

## Part 1: Creating a Personal GitHub Pages Site
(If you already have a personal GitHub Pages site, you can skip this.)

If you have a repository named *username*.github.io in your GitHub account, it will automatically be used to serve web pages from that address. You can see an example at https://github.com/mamamusings/mamamusings.github.io (the github directory) and http://mamamusings.github.io (the resulting website).

In your GitHub account, create a new (public) repository called *yourusername*.github.io. (This is the same process you used in Tuesday's exercise.) Give it a brief description, make sure the repository is public, and click the box to create a README.md file.You'll be taken to the web page for the new repository. 

In your browser, go to *yourusername*.github.io; you should see the readme page come up. ***If it doesn't work, ask for help before proceeding!!***

Now you need to clone the new repository to your computer, using the same process you used in Tuesday's exercise (copy the clone URL from the GitHub repository, and use the git:clone command in VS Code.
                
Once you've cloned the repo, and you have it open in VS Code, create an index.html file that includes your name and an image (you can use a pseudonym if you want, and it doesn't have to be a picture of you). Use CSS to make it look moderately professional. Commit the new file, and sync your files to GitHub. Then use a web browser to go to *username*.github.io. -- your files should show up there! (*Note*: GitHub can sometimes be slow in updating the website with changes; if you don't see your file appear right away, give it 30 seconds or so, and then try holding down the shift key while you reload the page. If it hasn't shown up after 60 seconds, ***ask for help***!)

(Note: Once this exercise has been graded, you can feel free to delete the files you created, or replace them with your own content.)

## Part 2: Creating a Project-Based GitHub Site
You're going to create a new repository to hold your web project files. 

While you could just create a subdirectory in your personal site directory, a better approach is to create a separate repository for your work in this class, and using the personal directory you created above for your own non-class-related personal page(s). There are a number of advantages to creating a separate repository for each project you work on, including being able to make the repository private before you want it "go live", giving editing access to specific users, and cloning only the repository that you want to work on.  

Create a new repository for your web project, called igme110. Follow the steps from Tuesday's exercise to create the repository on GitHub, and clone it to your computer. 

Using VS Code, create a subdirectory in the igme110 directory called "images", and another subdirectory called "more". 

In the igme110 directory, create an index.html file and a style.css file. In the "more" subdirectory create another index.html file. In the images directory put two images; one for each of the two HTML files. 

Before continuing, remember these rules for creating relative links to files:
- If you're linking to a file in the same directory, you just use the file name. (e.g. `href="style.css"`)
- If you're linking to a file in a subdirectory below the file, you start with the subdirectory name(s), followed by the file name. (e.g. `href="more/index.html`, `src="images/cat.jpg"`)
- If you're linking to a file in a directory above the current file, you use .. to mean "one level up" (e.g. `href="../styles.css` , `href="../images/dog.jpg`)

Add a heading, some text, and one of the images to each of the index.html files, along with a link from each page to the other page. Both pages should link to the same style.css file, and at a minimum you should use it to change the default font in the document.   

Here are my example files: https://github.com/mamamusings/igme110
And the resulting website: https://mamamusings.github.io/igme110


Stage, commit, and sync your files. 

On the GitHub site, go to the page for your new repository (github.com/*yourusername*/igme110), select “Settings” from the menu at the top of the page, and scroll down to the GitHub Pages settings. Choose the master branch as your source, and save. (Do *not* try to install a "theme"; these do not use standard HTML, but instead use a templating language based on the Ruby programming language. If you want to explore using GitHub Jekyll themes, you should create a separate repository for that.) After you save your new settings, the files in your igme110 directory should be visible at *yourusername*.github.io/igme110; try clinking on the link provided in the settings page to test it.

Here's an example of what I'm asking for: http://mamamusings.github.io/igme110


## Deliverables
Your project repository--with the two HTML files, two subdirectories, and two images--should be available at github.com/*yourusername*/igme110 no later than 9am on Friday morning. Once you've received a grade for this exercise, you can begin replacing the files with your web project files. 
