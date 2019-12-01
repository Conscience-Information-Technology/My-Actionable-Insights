---
description: >-
  The Git workflow for My Application Insights, developers expected to use only
  Git Bash for workflow. We are using very lightweight, branch-based workflow
  built around core Git commands.
---

# Git Workflow

**Clone Repository:** Create a local copy of a project that already exists remotely at preferred file location. 

{% tabs %}
{% tab title="Git clone " %}
```
$ git clone https://ConscienceIT@dev.azure.com/ConscienceIT/MAI/_git/MAI
```
{% endtab %}

{% tab title="Links" %}
```
https://www.atlassian.com/git/tutorials/setting-up-a-repository/git-clone

```
{% endtab %}
{% endtabs %}

**Pull latest code from centralised repository:** Before starting any new task always get latest updates from ****centralised DEV repository to local DEV repository. 

{% tabs %}
{% tab title="$ git pull" %}
```text
$ git fetch origin DEV
$ git pull origin DEV
```
{% endtab %}

{% tab title="Links" %}
```
https://www.atlassian.com/git/tutorials/syncing/git-pull
```
{% endtab %}
{% endtabs %}

**Create a branch:** Before starting task always create _**task specific branch**_ from DEV branch. Task specific branch created from DEV allows team to contribute with other members. These short-lived branches, in particular, keep team members focused about particular task.

{% tabs %}
{% tab title="Git Branch" %}
```
$ git branch [BRANCH-NAME]
```
{% endtab %}

{% tab title="Instructions" %}
```
BRANCH-NAME format => MAI(DeveloperName)(TaskNumber)_(CommitMessage)
```
{% endtab %}

{% tab title="Links" %}
```

```
{% endtab %}
{% endtabs %}

**Checkout newly created branch :** The git checkout command lets you navigate between the branches created by git branch. Checking out a branch updates the files in the working directory to match the version stored in that branch, and it tells Git to record all new commits on that branch.

{% tabs %}
{% tab title="Git Checkout" %}
```
$ git checkout [BRANCH-NAME] 
```
{% endtab %}

{% tab title="Links" %}
```
https://www.atlassian.com/git/tutorials/using-branches/git-checkout
```
{% endtab %}
{% endtabs %}

**Commit Code into local Repository:** Save snapshots of development efforts within working branch and completes the change-tracking process. Working in Git and saving changes is two step process.

* **Add Changes :** The `git add` command adds a change in the working repository to the staging area. It tells Git that include particular file in the next commit.
* **Git Commit :** The `git commit` command captures a snapshot of project's currently staged changes. Committed snapshots can be thought of as “safe” versions of a project—Git will never change them unless you explicitly ask it to.

{% tabs %}
{% tab title="Git Add" %}
```
$ git add .
$ git add all
```
{% endtab %}

{% tab title="Links" %}
```
https://www.atlassian.com/git/tutorials/saving-changes
```
{% endtab %}
{% endtabs %}

{% tabs %}
{% tab title="Git Commit" %}
```
$ git commit -m "[commit message]"
```
{% endtab %}

{% tab title="Instructions" %}
```
BRANCH-NAME format => MAI(DeveloperName)(TaskNumber)_(CommitMessage)
```
{% endtab %}

{% tab title="Links" %}
```
https://www.atlassian.com/git/tutorials/saving-changes
```
{% endtab %}
{% endtabs %}

**Push all commits to remote repository:**  The `git push` command is used to upload local repository content to a remote repository. Following command creates local branch at remote origin.

{% tabs %}
{% tab title="Git Push" %}
```text
$ git push -u origin [BRANCH-NAME]
```
{% endtab %}
{% endtabs %}

**Open a Pull Request:** Newly uploaded will merged into DEV repository once code reviewed by responsible person, for that Developer need to create Pull request at GitHub/DevOps portal. Pull Requests initiate discussion about code, they're tightly integrated with underlying Git repository, anyone can see exactly what changes would be merged. Once code reviewer accept your changes then your code will be automatically merged with DEV branch.

**Creating New Branch:** Again create fresh new branch for new task from latest DEV repository so that your work will be collaborated and sync with other team members, So each task assigned to each team member will have new repository. \([https://guides.github.com/introduction/flow/](https://guides.github.com/introduction/flow/)\)

**Deleting Old/Unused Branches:** Developer suppose to delete local branches once TESTING Team approves your task. Remote branches automatically deleted once your code merged with DEV repository.

~~~~

* ~~**SQUASHING COMMITS**~~ **USING GIT REBASE**
* [http://gitready.com/advanced/2009/02/10/squashing-commits-with-rebase.html](http://gitready.com/advanced/2009/02/10/squashing-commits-with-rebase.html)
* [https://www.freecodecamp.org/news/an-introduction-to-git-merge-and-rebase-what-they-are-and-how-to-use-them-131b863785f/](https://www.freecodecamp.org/news/an-introduction-to-git-merge-and-rebase-what-they-are-and-how-to-use-them-131b863785f/)

If you are beginner with git then you can visit following links and understand how git or github works.

* [https://guides.github.com/](https://guides.github.com/).
* [https://www.youtube.com/playlist?list=PLg7s6cbtAD17Gw5u8644bgKhgRLiJXdX4](https://www.youtube.com/playlist?list=PLg7s6cbtAD17Gw5u8644bgKhgRLiJXdX4)
* [http://gitready.com/](http://gitready.com/)
* [https://www.atlassian.com/git/tutorials](https://www.atlassian.com/git/tutorials)
* [https://learngitbranching.js.org/](https://learngitbranching.js.org/)
* [http://git-school.github.io/visualizing-git/](http://git-school.github.io/visualizing-git/)
* [https://github.github.com/training-kit/downloads/github-git-cheat-sheet/](https://github.github.com/training-kit/downloads/github-git-cheat-sheet/)
* [https://dzone.com/articles/top-20-git-commands-with-examples](https://dzone.com/articles/top-20-git-commands-with-examples)

