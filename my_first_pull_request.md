# Completing Your First Pull Request (PR)

## Introduction
For each assessment we will follow different commit strategies.

### Individual Assessments
For individual work a direct commit to the `main` or trunk of the repository will be done to secure your progress. This means every time you make a change to your code and commit and push the changes it will modify the main code base. The benefit of this for this course it that it will simplify your development process. You should endeavour to make commit comments meaningful, as good comments will get additional marks. When marking I will use a pull-request to give feedback.

### Group Assessments
When working on group assessments your team should follow [trunk-based development](https://www.atlassian.com/continuous-delivery/continuous-integration/trunk-based-development). This means that you will create a branch for the work you are doing and then create a merge or pull request when done with the changes for one of your other team members to review. They will give feedback and if happy with the changes you will merge these to main. This is current industry best practice for [continuous integration / continuous deployment (CI/CD)](https://about.gitlab.com/topics/ci-cd/). The previous best practice was [Git WorkFlows](https://nvie.com/posts/a-successful-git-branching-model/) which involved working off feature branch from trunk and merging changes back to trunk after the change was complete. Then create release and maintenance branches for supporting production. In organisations with many developers working on the same codebase this can result in merge hell where trunk has changed 1 or more times since your branch was made and you need to deal with merge conflicts.

### Additional Info
- [DevOps CI/CD Explained in 100 seconds](https://www.youtube.com/watch?v=scEDHsr3APg)
- [A guide to Git with Trunk Based Development](https://hackernoon.com/a-guide-to-git-with-trunk-based-development-93a350c)

## Prerequisites
- Laptop or PC. Using a tablet or iPad will severely limit your ability to work on code
- A fully functional IDE. Recommendation is VSCode or VSCodium. 
    - Visual Studio, JetBrain products (Rider, PyCharm, IntelliJ) will work
    - Avoid IDLE, Vim or other text based solutions as they will limit your ability to work quickly and are missing many modern features like syntax highlighting, code suggestions, built in debugging.
    - Anything else please ask before using.

# Making Changes in GitHub
## Step 1
Read though the documentation about using [git and github](./git_github.md).

## Step 2
1. Add a markdown file to the repository using github. `Add File -> Create new file`

![](images/Screenshot%202024-06-08%20160352.png)

2. The file should be called `hello.md` and should include at least:
    - first and second level headings
    - some icons like a :smile:
    - bullet points of what you have learnt from the reading
    - Any coding languages you have used before. (Blockly, Python, C, C++ Java, C#, ...)
    - What you would like to get from this subject

If you have forgotten what markdown is refer to the [section on markdown](./git_github.md#using-markdown-on-github)

3. Create a Pull request through `Contribute -> Open Pull Request -> Create pull request`
    - you would add a description if this was true code change PR but for now it can remain empty

![](images/Screenshot%202024-06-08%20154714.png?raw=true)

Your teacher will give you feedback in the PR (pull request) and close it.

# Making Changes on a Local Copy
You do not need to wait for the GitHub PR to be closed before starting this.

## Steps
1. Clone the repository to you local machine.
```console
foo@bar:~$ git clone https://github.com/<organisation>/<repository-name>.git
```

1. Create a branch and switch to it
```console
foo@bar:~$ git branch <branchname>
```
1. Add a new file called `local-branch.md` and include in the file:
    - which machine you are using (Laptop or PC)
    - which Operating system (Mac, Windows, Linux)
    - which IDE you are using

1. Add the file to the branch and commit it
1. Go back to github and create a pull request for you branch to be merged back into main
1. Approve your merge and then create a new merge for your teacher to review. The same as step 2.3 above

> [!NOTE]
> A pull request is not part of git. It is a feature of github, bitbucket and others online code repositories where as git is a revision control system. 

## Conclusion
You should now have a clear understanding of the basics for using git and github. In future lessons we will rely heavily on these tools for coding,  marking and feedback. If you still have concerns with using these tools or need more help, please check with others in the class first. If you are still not sure, please talk with your teacher.