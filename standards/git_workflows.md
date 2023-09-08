# Using Git

Depending on your preferences, you can either use [Git on the command line](https://gitforwindows.org/) or via [GitHub Desktop](https://desktop.github.com/). Either way you'll need to use your Local Admin credentials to install it. The Desktop app is much easier, especially if you are new to using Git, however it does have limitations and Git on the command line is significantly more powerful and flexible. Generally you won't need that flexibility, but occassionally it's handy or even necessary to get out of a mess.

## Git documentation

The [official documentation](https://git-scm.com/) can be useful, though it's sometimes so obtuse that it has spawned [a parody site](https://git-man-page-generator.lokaltog.net/).

The [Atlassian Bit Bucket](https://www.atlassian.com/git) guides are pretty good. Of course there is also [GitHub's docs](https://docs.github.com/en/get-started/using-git/about-git).

# Creating new repositories

Generally you should start by cloning the [LTU example repository](https://github.com/La-Trobe-University-Library/example).

You can do this from GitHub Desktop by going to `File - clone repository...` or via the command line via `git clone`.

# Working with existing repositories

We use the process described in [GitHub flow](https://docs.github.com/en/get-started/quickstart/github-flow):

1. Create a branch
2. Make changes
    1. make sure all the changes in a single branch are related - if there are two different bugs you are fixing, you should have a branch for each of them respectively.
    2. generally you should add each self-contained change in your work as a single commit, with a descriptive name. Judging how big a commit should be is more art than science, but err on the side of more rather than fewer commits.
3. Create a pull request
4. Invite reviewers
    Usually at least one other relevant team member should review your changes before they are merged.
5. Address review comments
6. Merge your pull request
    If you are confident you have addressed all review comments, merge the PR. You can also ask your reviewer or another team member to do this.
7. Delete your branch
    Delete the branch on the remote (GitHub) repository to keep thing clean, and also on your local machine.

TODO:

- do we use Issues, or is that doubling up on tickets elsewhere? Or can we automate it in Powerapps? Should we?
