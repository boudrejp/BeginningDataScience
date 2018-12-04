# __Learning Git__
There's a lot of good resources out there to learn git. You'll want to learn git after you know your way around the command line. There are many ways to interface with git functionality, but I believe the best way to learn and have solid fundamentals is to use the command prompt.

## Step 0: Download Git
* Download git for your system here: `https://git-scm.com/downloads`

Go ahead and open up `Git Bash` when you have it all installed. You'll notice that Git looks like a standard command prompt or powershell window. It will use __bash__ commands rather than windows shell commands, so if you run into issues with the commands taught to you in the command prompt lesson that's why. Most commands are the same but just a few are different.

From here, I will turn it over to external resources since there are lots of good resources out there to learn why you'd want to use git and how to use it effectively. No sense in recreating the wheel...

## Git Context
Why use git in the first place? What is it?

* [A nice article on Medium](https://medium.com/swlh/git-as-the-newbies-learning-steroid-963a2146220b)
* [The Atlassian Git tutorial is VERY good](https://www.atlassian.com/git/tutorials/what-is-version-control)
* [A nice, short video of why you want it and broadly how it works](https://www.youtube.com/watch?v=DqtZUvmPmo4)

## Using Git
How can I use git?

I would recommend the [Atlassian Git tutorial](https://www.atlassian.com/git/tutorials/setting-up-a-repository) sections `Getting Started` and `Collaborating`. These give you all the commands that you'll need to use on a regular basis.

In general, a git workflow is the following:
  1. Someone sets up a central git repository in Bitbucket, Github, Gitlab, or by some other means
  2. The developers clone the repository
    a. In git bash, first `cd ./directory/to_lone repo/` then `git clone repo_url.git`
  3. Each individual developer creates branches for the features that he/she works on. Commits are made locally for small blocks of code.
  a. In git bash, `git branch my_new_branch`, then `git checkout my_new_branch`
  b. Begin doing work, making changes, additions, etc...
  c. Upon a good "checkpoint", `git add file_to_be_added`, `git commit -m "message about changes"`, `git push origin my_new_branch`
  4. Once a feature is completed, the developer merges the feature branch into the master branch of the repository in the central repository. Other editors will review to make sure things look good, and work together to resolve merge conflicts.
  5. Developers will merge/rebase their current feature branches to reflect the new changes in the master branch in the central repository.

By doing this, all the developers can work efficiently on their own parts of the project while not stepping on the toes of anyone else as they work. It allows for easier collaboration and more productivity!

You'll notice that this is a git repository in its own right- so you could clone this to your local machine and make changes to it and I would never know. However, if you had a fix or a suggestion that you'd like to make, you could make the edit, commit, and then submit it to the central repository as a pull request. That's how a lot of open source software projects work- people develop useful features for their own purposes and then will create pull requests so other people can use them as well.

Happy Git-ing!
