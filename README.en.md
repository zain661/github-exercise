# Learning how to use git commands
1. Go to the `index.js` file and type this: `console.log("Hello, World!");` then save it.
2. Open the terminal and click on the debug console as you see in the picture below:

![image](https://user-images.githubusercontent.com/47659847/83018829-9495b380-a02e-11ea-9979-4d9b3735af61.png)

3. Press F5 to run the file and see what you wrote inside the console.log get immediately printed inside the terminal. 


## Sharing your code on Github
The changes you have just made are only on your local machine. If you go to Github and open up the repo we cloned, you’ll notice that nothing has really changed there.

To see the changes on Github, write these commands on the terminal:
- git add index.js then hit Enter.
- git commit -m “Wrote my first JS code” then hit Enter.
- Pushing your code has 2 options:
  - If the repo you're pushing to is your own, use git push origin master then hit Enter.
  - If the repo you're pushing to is a forked repo, follow these steps:
    - First, you need to set the remote repo to the repo you forked from, so you can pull the latest changes from them. Use this command to do so: git remote add upstream (original repo link).
    - Second, make sure you did the first step correctly using git remote -v. You should see 4 links; 2 of them are the original rep link and the other 2 are the forked repo links which have your username in.
    - Lastly, use git push origin master to push to your forked repo.

## The basic git commands you’ll use in every project
- **git status:** This command shows the names of the files to which you made a change.
- **git diff:** Use this command when you can’t remember the changes you made to the files. This command will show you what the original code was and how you changed it.
- **git add:** This allows you to choose the files you want to put on Github and share them.
- **git commit -m “ ”:** The -m stands for message. You’ll use it to connect your commits to a message explaining what you just committed to git. This is like saying ‘I really want these changes’. Then, you write a message between the quotes to explain what are the changes you made and why you did them so that you and your teammates can track what you did.


  **Note:**

  When you use the git add command, you will be preparing or staging the files you added for a commit. You will have the files in something called the staging area which allows you to easily remove files. If you put any file there by mistake or you just don’t want the changes you made, you can just remove them all at once.

- **git push [remote name] [branch name]:** we use this command to push or move all the changes you just added and committed to Github so it can be online for everyone to see.

~ To actually push you have to specify the remote location that you are pushing to. Here we’re pushing to master which is the place where all the final changes are going to be in. So use this command **git push origin master**.


## Some notes about the command git push origin ...
Origin is the default short name of your online repo. You can clearly see this if you run this command : **git remote**.

Use this command **git remote -v** and you’ll get a short name of the repo, which is **origin**, and its URL, which is the URL you see in the browser tab of your Github account just without the **.git** part.

You can see next to one of the URLs the word **push**. This tells you that you can use this URL to push to.


# Lecture Practice set
- Change the string inside the `console.log` to say **"Hello"** then **your name**.
- Press `F5` to run the file and make sure you solved the first step right.
- Use **git's basic commands** to `add` and `commit` your changes.
- Use the commands we learned in order to get the URL of the remote repo and push to it.
- Change the string again to say **"Goodbye"** then **your name**.
- Use **git's basic commands** to `add` and `commit` your changes then push again but this time use the word origin instead of the URL. Do you notice any differences or are they the same?
