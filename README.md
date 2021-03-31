# Open Coding Hour GitHub Workshop

Welcome to the Open Coding Hour GitHub workshop! 
Rachael Cox and Alex Lukasiewicz will be guiding you through the basics of using github. We will start by covering some common terms used in the git world and then walking through the process of intializing your own repository. 
We will also cover how to work on collaborative projects and demonstrate what happens when things go wrong.

## Demo: Branching and Merging with Conflicts 

1. As a collaborator on this repository, I've made a branch called "test" that we are going to merge with Alex's "main" branch. The "test" branch contains an R script not present in the "main" branch.
    * [R script, merge 1](https://htmlpreview.github.io/?https://github.com/rachaelcox/OCH_git_workshop/blob/main/output1.html)
2. To do this, I'll click "pull requests." **Important: merge order matters.** I want to prioritize changes in Alex's branch by pulling from "main" to "test" first. The "test" branch contains this text, not present in the README of Alex's "main" branch--this will create a merge conflict, which we will resolve manually.
4. After the file looks the way I want it to, I'll mark the conflict as resolved, and complete the merge.
5. Finally, I'll merge my test branch upstream. There should be no conflicts since we resolved those in the previous step, and the merge will complete automatically.

## Demo: Forking, Cloning, Pushing, Merging Upstream

1. Now we're going to pretend I'm not a collaborator, and instead I am a stranger that sees this repository and wants to suggests changes to this R script. To do this, I'm going to create a fork. A copy of this repository will then appear on my account.
2. To make changes to the R script, I will make a local clone of the repository. I'll do this on the command line, but it can also be down via GitHub Desktop application or the "Download zip" button.
3. Next, I'll open the script I want to edit in a development environment of choice. If it were a Python script, I might open it in Spyder or Sublime Text. Since it is an R script, I'm going to open it in RStudio to make and save changes.
4. Once I've made changes on the local version of this repository, I need to push those changes back up to the GitHub server. I'll do this on the CLI with the following commands:
    * `git add .`
    * `git commit -m "made changes to script"`
    * `git push`
5. Now that my fork is now up-to-date with the changes I want to contribute, I will open a pull request as in the previous example. GitHub automatically detects my fork is downstream of Alex's repo, and sends her a request to merge my fork with the main branch of her repo.
