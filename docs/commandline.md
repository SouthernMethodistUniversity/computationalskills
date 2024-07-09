# How do you interact with your computer?
* Most of us are used to a graphical user interface [GUI](https://en.wikipedia.org/wiki/Graphical_user_interface) but the command line allows you more control.

# Command Line

* What is the command line and why is it like this?

The command line is a text-based way of interacting with your computer. Working in command line helps you make a mental model of how you environment is layed out. This environment is the result of a series of choices, made by humans.  

You may hear it called different names, such as the terminal, the shell, or bash. In practice, you can use these terms interchangeably. If you're curious, though, you can read more about them [here.](https://askubuntu.com/questions/506510/what-is-the-difference-between-terminal-console-shell-and-command-line) The shell we use (whether terminal, shell, or bash) is a program that accepts commands as text input and converts commands into appropriate operating system functions.  

And yes, "the command line" is also laden with masculine and military metaphors, which is reflective of the history of computing and programming. 

* As Wendy Hui Kyong Chun discusses in ["On Software, or the Persistence of Visual Knowledge," (2004)](https://direct.mit.edu/grey/article/doi/10.1162/1526381043320741/10837/On-Software-or-the-Persistence-of-Visual-Knowledge) almost all computers (as in human comput-ers) in the US during World War II were young women. Human computers received commands from analysts &#8212; predominantly men with the military &#8212; that they then had to interpret and act upon the machine. As Chun argues, "computation depends on 'yes, sir' in response to short declarative sentences and imperatives that are in essence commands ... The command line is a mere operating system (OS) simulation" (page 34). The command line (of computers today) receives these commands as text that is typed in.  

These repositories we are using for our lessons additionally have a lot of racialized terms. [See 'Ditch These Racist Terms From Your Tech Vocabulary.'](https://lifehacker.com/ditch-these-racist-terms-from-your-tech-vocabulary-1844041452)


## Why is the command line useful?

Initially, for some of us, the command line can feel a bit unfamiliar. Why step away from a GUI point-and-click workflow? By using the command line, we move into an environment where we have more minute control over each task we'd like the computer to perform. Instead of ordering your food in a restaurant, you're stepping into the kitchen. It's more work, [but there are also more possibilities."](https://www.freecodecamp.org/news/command-line-for-beginners/#whyshouldievencareaboutusingtheterminal)

The command line allows you to...

* Easily automate tasks such as creating, copying, and converting files.
* Set up your programming environment.
* Run programs you create.
* Access the (many) programs and utilities that do not have graphical equivalents.
* Control other computers remotely.

In addition to being a useful tool in itself, the command line gives you access to a second set of programs and utilities and is a complement to learning programming.
  * Wring a script or program (programming!) allows you to automate a series of repetitive tasks.  

What if all these cool possibilities seem a bit abstract to you right now? That's all right! On a very basic level, most uses of the command line are about **showing information** that the computer has, or **modifying or making** things (files, programs, etc.) on the computer. 

## Introduction to the command line

By this point in our academic careers, most of us have figured out some ways we like to interact with computers. Whether that involves avoiding them as much as possible or constantly testing new software, we likely have some ideas about how we feel comfortable getting things done. How would you show a person who had never seen a computer, say [Kimmy Schmidt](https://youtu.be/LIdFa1qLgNQ) or [Brendan Fraser in *Blast from the Past*](https://youtu.be/Xq29uTtKW4M), how to *do* something on your computer? 

Many of us would explain what a screen and a cursor are, and then show how to point and click on icons. This approach relies on the  graphical user interface, or GUI (pronounced "gooey!"). 

Another way to make your computer do things: through the command line. Instead of pointing and clicking, we'll be typing in either Git bash (Windows) or terminal (OSX) to tell the computer directly what task we'd like it to perform. 

* Here is an external [command line tutorial](https://ryanstutorials.net/linuxtutorial/) if you wish to learn more. 


## Review of the Command Line (also command shell).
- For additional practice, you can look at this [The Unix Shell workshop](https://swcarpentry.github.io/shell-novice/index.html)

<!--- In addition to the command line, you may be using your text editor and your browser. Before continuing, its important that we clearly distinguish between these three different spaces or environments:
- Your plain text editor where you'll be writing your document is on your local computer.
- That document is initially saved in a git-enabled repository on your local computer.
- Your browser is where you'll be uploading your repository to GitHub, a cloud service.
- Your terminal is where you'll be communicating with GitHub to send the repository and project files back and forth between the cloud (which you can view through the GitHub website) and your hard drive. 

Because you'll be moving between these three spaces throughout the workshop, you may want to use (<kbd>command (⌘)</kbd> + <kbd>tab</kbd>) or (<kbd>control</kbd> + <kbd>tab</kbd>) to move quickly between the three windows on your desktop.-->

## Accessing the Terminal

### macOS

Hold the <kbd>command (⌘)</kbd> key and press the <kbd>space</kbd> bar at the same time to bring up the "Spotlight Search" window. Type `terminal`, followed by <kbd>enter</kbd> to quickly open the Terminal.

### Windows

Press the <kbd>windows</kbd> button on your keyboard. When the search menu pops up, type `git bash` and press <kbd>enter</kbd>.

## Practice Navigating the Command Line

- If you _do not have experience or prior knowledge of the command line, you may want to work through one of 
 the following workshops_: [Introduction to the Command Line](https://gc-dri.github.io/Dhrift-GC/workshops/command-line/) or [The Unix Shell](https://swcarpentry.github.io/shell-novice/)

You can create the folder anywhere on your hard drive by typing the following into your terminal and hitting <kbd>enter</kbd>.

```console
$ cd <directory-name>
```

Let's practice this command by using it to take us to our Desktop. Type the following command into your terminal and hit <kbd>enter</kbd>.

```console
$ cd Desktop
```

This will change your current working directory from `/Users/<your-name>` to `/Users/<your-name>/Desktop`.

#### *Note for staff or company computers* 

If your computer has multiple users you can choose your user profile in the C: drive or you type the following command in your terminal and and hit <kbd>enter</kbd>
```console
$ cd C:/Users/[put your username such as SMU ID here]/Desktop/
```



Check your current directory by typing the following command into your terminal and hit <kbd>enter</kbd>:

```console
$ pwd
```

Now, use the following command to go up one directory:

```console
$ cd ..
```

Check your current directory again using the following command. You should be back in your "home" directory:

```console
$ pwd
```

Practice going back and forth between your Desktop and your home directory.

When finished, go to your Desktop folder and check that you're there with `pwd`.

## Making a Projects Folder

In this session, we will be making a syllabus and using Git to keep track of our revisions. Let's create a Git project folder.

If you don't have a projects folder on your desktop, create one using the following command:

```console
$ mkdir projects
```

From `Desktop`, Navigate into your `projects` folder using the following command:

```console
$ cd projects
```

Then create a `git-practice` folder with the following command:

```console
$ mkdir git-practice
```

Navigate into the new `git-practice` folder using the following command:

```console
$ cd git-practice
```

At this point, when you type `pwd`, your folder structure should look like this:

```console
$ pwd
/home/<username>/Desktop/projects/git-practice
```

TO see what files are in a folder, `ls`, it will show what files are there. To see all files, including invisible, type `ls -a`

```console
$ ls

$ ls -a
```


## Evaluation

Which command do you use to make a new folder?
- `pwd`
- `cd`
- `mkdir`*

Which command do you use to enter into a folder?
- `pwd`
- `cd`*
- `mkdir`

Which command do you use to check where you are?
- `pwd`*
- `cd`
- `mkdir`


## Pro-tip for the Command Line: How to exit unknown screens

If you're ever stuck or "trapped" on the command line, try running through these common exit commands to return to the prompt:

- <kbd>control</kbd> + <kbd>c</kbd>
- <kbd>control</kbd> + <kbd>d</kbd>
- `q` followed by <kbd>enter</kbd>
- `:q` followed by <kbd>enter</kbd>

<kbd>control</kbd> + <kbd>c</kbd> attempts to abort the current task and restore user control. <kbd>control</kbd> + <kbd>d</kbd> escapes the current shell environment—if you use it at the normal `$` prompt, it will end the current command line session. `q` is often used as a command (followed by <kbd>enter</kbd>) to escape from specific programs like `less`. `:q` is the command used in `vi` that changes the mode of interaction (`:`), allowing you to enter the `q`, a one-letter command to quit, which must be followed by <kbd>enter</kbd>. Thus, it's a command specific to `vi`.


## Evaluation

Which best describes where you are working when you're writing in your plain text editor:
- on my local machine*
- on the internet

Which best describes where you are working when you're using your terminal to communicate with GitHub and share the files:
- on my local machine*
- on the internet

Which best describes where your files are when you are viewing them in GitHub:
- on my local machine
- on the internet*

Git-enabled repository means
- none of the files on my local machine are being tracked
- a specific file on my local machine is being tracked
- a specific folder on my local machine is being tracked*
- all the files on my local machine are being tracked

Which command do you use to make a new folder?
- `pwd`
- `cd`
- `mkdir`*

Which command do you use to enter into a folder?
- `pwd`
- `cd`*
- `mkdir`

Which command do you use to check where you are?
- `pwd`*
- `cd`
- `mkdir`
---
 ## Shell Cheat Sheets

[Summary of Basic Commands](https://swcarpentry.github.io/shell-novice/reference.html#summary-of-basic-commands)

| Action       | Files | Folders      | 
| ------------ | ----- | ------------ |
| Inspect      | ls    | ls           | 
| View content | cat   | ls           | 
| Navigate to  |       | cd           | 
| Move         | mv    | mv           | 
| Copy         | cp    | cp -r        | 
| Create       | nano  | mkdir        | 
| Delete       | rm    | rmdir, rm -r | 

- [Unix Shell Cheat Sheet](https://cambiotraining.github.io/hpc-intro/99-unix_cheatsheet.html)

## Glossary
- [Glossary](https://swcarpentry.github.io/shell-novice/reference.html#glossary)


-----
#### Attribution 

Session Leaders:  [Rafia Mirza](http://guides.smu.edu/prf.php?account_id=142826/) 
* Written by Rafia Mirza. 

[![Creative Commons License](https://i.creativecommons.org/l/by-sa/4.0/88x31.png)](http://creativecommons.org/licenses/by-sa/4.0/)
When sharing this material or derivative works, preserve this paragraph, changing only the title of the derivative work, or provide comparable attribution.


