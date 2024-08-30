# Using Git

Depending on your preferences, you can either use [Git on the command line](https://gitforwindows.org/) or via [GitHub Desktop](https://desktop.github.com/). Either way you'll need to use your Local Admin credentials to install it. The Desktop app is much easier, especially if you are new to using Git, however it does have limitations and Git on the command line is significantly more powerful and flexible. Generally you won't need that flexibility, but occassionally it's handy or even necessary to get out of a mess.

## Git documentation

The [official documentation](https://git-scm.com/) can be useful, though it's sometimes so obtuse that it has spawned [a parody site](https://git-man-page-generator.lokaltog.net/).

The [Atlassian Bit Bucket](https://www.atlassian.com/git) guides are pretty good. Of course there is also [GitHub's docs](https://docs.github.com/en/get-started/using-git/about-git).

# Creating new repositories

Generally you should start by cloning the [LTU example repository](https://github.com/La-Trobe-University-Library/example).

You can do this from GitHub Desktop by going to `File - clone repository...` or via the command line via `git clone`. See [GitHub's instructions on cloning](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository?tool=desktop)

Once you have a clone on your local machine, add a new **empty** La Trobe repository on GitHub. Do not initiate it with any files (e.g. LICENSE, README) when asked. Your new repository should have an address like `https://github.com/La-Trobe-University-Library/myawesomeproject.git`.

Now go back to GitHub Desktop and go to `Repository > Repository settings...`. Change the **Remote** address to the address of the empty repository you just created.

Make your changes locally to turn the example template into a real repository. Once you have committed your changes, you can **publish** up to GitHub. This will push your changes to the new remote you created.

# Working with existing repositories

We use the process described in [GitHub flow](https://docs.github.com/en/get-started/quickstart/github-flow), except to keep things simple you don't necessarily need a new branch if you are working from a fork:

1. Create a fork
2. Make changes in a new branch or the `main`/`master` branch
    1. make sure all the changes in a single branch are related - if there are two different bugs you are fixing, you should have a branch for each of them respectively.
    2. generally you should add each self-contained change in your work as a single commit, with a descriptive name. Judging how big a commit should be is more art than science, but err on the side of more rather than fewer commits (i.e. smaller changes per commit).
3. Create a pull request - you can do this from the GitHub Desktop interface by pushing to the remote and creating a PR in one action
4. Invite reviewers: Usually at least one other relevant team member should review your changes before they are merged.
5. Address review comments
6. Merge your pull request: Once your PR is complete, another team member should merge your PR to ensure that a second person always reviews every PR as above.
7. If you created a fresh branch: Delete the branch on the remote (GitHub) repository to keep thing clean, and also on your local machine.
