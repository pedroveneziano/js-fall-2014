
- Create a folder (directory) on your Desktop, called `command-line`
- Open it in Finder and resize it so it takes up the right half of your screen.
- Open Terminal.app and resize it so it takes up the left half of your screen.

It should look like this.

- Type `cd ~/Desktop/command-line`

Commands have a few parts. Here `cd` is the command name. The second part is its 'argument.' With this command you're telling the terminal to _c_hange _d_irectory to the directory you just made.

In order to __print__ your __working directory__ is, type the command `pwd`. 

- In order to __list__ what's in the current directory, type the command `ls`. Since there are no files in this directory, the command won't print anything. Let's change that.
- To create new empty file, we can use the command `touch`. Touch creates a file with whatever name you supply it. Try entering `touch my-new-file.txt` into the terminal. You should notice a new file appear in your Finder.
- Try typing `ls` now. You should see the name of your new file.
- In Finder, open this file using a text editor such as Sublime or Text Wrangler. Enter a sentence or two of text and save it.
- Back in terminal, type `cat my-new-file.txt`. You should see the text you entered printed on the screen. The `cat` command prints out the contents of a file.
- Press the up arrow in your terminal, you should see the command you just entered. Play with the up and down arrows and you'll notice you can move backwards and forwards through the commands you've entered. Press down until you have an empty terminal again.
- Type `clear` in the terminal. It clears all of the text that's been printed so far. Use it whenever you want a fresh slate.
- Create another by typing `touch another-file.txt` and then another by typing `touch yet-another.txt`.
- You can also create a __copy__ of a file. Try entering `cp another-file.txt another-file-2.txt`. 

Notice that this command takes two arguments. The first argument is the name of the file to copy, the second argument is the name of the new file.

- Type `ls` again to see your new files. So you can create a file, now let's __remove__ one. Type `rm my-` and then hit the tab key. You'll notice that terminal completes the name of the file. Hit enter. You should notice your file disappear. It's gone forever. It's not in the trash. It's just gone.
- Now let's delete all the files you've created. All the files you've created have the ending `.txt`. It would be nice if we could use this fact to avoid typing each filename. The terminal lets us use wildcards for this. Try typing `rm *.txt`. You'll notice all the files are gone.

Lets say you want to move to the Desktop. There are a few ways to do this. Remember when you typed `pwd`. It printed out the complete path to your directory. You could grab the first part of this (everything up to and including Desktop) type `cd /home/<yourname>/Desktop`. Or you can use the special directory name `..` which means __the parent directory__. Let's use that.

- Type `cd ..`. Then type `pwd`. You've moved up a directory to the desktop.

There are many more things you can do with the terminal and we'll see some more things throughout the class. But for now you know the basics. Feel free to play around, but be careful with commands like `rm`. 


This is your first assignment, and its very important.
It's the basis for all the other assignments. Each week, you'll be submitting work
by uploading it to a website called Github.com. Github is a popular site used by programmers to 
colloborate on code. It's based on Git, a piece of __version control software__. 

If you don't know what that is, that's ok. You know when you're working on a Photoshop file and you want to make a new copy, but you
think you might still want to keep around your old changes, so you save as and name it something like _final-project-new-2-jan-11th.psd_? Programmers don't like to that.
It gets to confusing to figure out what the actual new version is. So we use a version control tool to keep around all the old versions. They're tucked away, out of site, but available. Git is one of these tools.

Git can be pretty daunting even to seasoned professionals. But our use will be pretty basic. Before you get started, here are some terms:

#### Glossary

##### Repository (Repo):
A single git project. Can have multiple folders and files. Can exist on many computer. There is a copy of the repo for this class at https://github.com/miniatureape/js-fall-2014. I also have a local copy on my computer. You can clone it yourself and have your own copy. when you do, you have the complete project history.

##### Adding:
In order for git to track a project, you have to 'add' it to the repo. Otherwise it will ignore it.

##### Commit:
A change or set of changes you've made to one or more files.

##### Pushing:
To move the code from your computer where you're working to a central repo to share with others, you 'push' your code.

#### Example workflow.

You have a new project you're about to start. First you create a git repo to track files. Then you create a file, _index.html_. You're ready to save this work, so you add this file to the repo and commit file. You also want to share it with the world, so you push it to your remote repo. 

You decide there are a few changes you'd like to make so you edit your file. When you have completed the edits, you commit again. Then you decide you need a new file _main.css_ so you create it and add it to the repo. Now you want to share this new file and all your changes so you push again.


Your assignment for this week:

1. Create an account on github.com (a free one is just fine).
2. Download a client for your [Mac](https://mac.github.com/) or [PC](https://windows.github.com/).
3. Complete steps 1-6 in the getting started guide for [Mac](https://mac.github.com/help.html) or 1-4 in the guide for [PC](https://help.github.com/articles/getting-started-with-github-for-windows) 
4. Create a local repository with a single file and push it github.com.

Note: the window instructions are much worse. I suggest you follow the Mac instructions even if you're on a windows machine, but understand you'll have to do a bit of translation, because the user interfaces are not identical. If you're having trouble see also:

- https://help.github.com/articles/creating-a-new-repository
- https://help.github.com/articles/adding-repositories-with-github-for-windows

If you're not afraid of your computer's terminal, skipping the github GUI is fine. You can work on the command line if you wish.

I know this is a lot to take in without any instruction, but remember, you have two weeks to complete this because we don't meet the first two Mondays. If you're having trouble, reach out to your fellow students, the internet at large or me. You will have completed this assignment if:

- You have a github account
- You have a local repository (doesn't matter what's in it).
- You have pushed the local repository to github.
