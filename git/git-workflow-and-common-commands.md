---
description: 'My Actionable Insights: developers expected to use only Git Bash for workflow.'
---

# Git Workflow

## The GitHub workflow for My Application Insights.

The Git flow is a lightweight, branch-based workflow built around core Git commands.:

* **Clone Repository:** Create a local copy of a project that already exists remotely at preferred file location. 

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

* **Create a branch:** Before starting new task always create task specific branch from DEV branch. 

  Task specific branch created from DEV allows team to contribute parallel along with other team members. These short-lived branches, in particular, keep team members focused about particular task.

{% tabs %}
{% tab title="Git Branch" %}
```
$ git branch [BRANCH-NAME]
```
{% endtab %}

{% tab title="Links" %}
```

```
{% endtab %}
{% endtabs %}

{% hint style="info" %}
Instructions: BRANCH-NAME format =&gt; MAI_\(DeveloperName\)_\(TaskNumber\)
{% endhint %}

* **Checkout newly created branch :** The git checkout command lets you navigate between the branches created by git branch. Checking out a branch updates the files in the working directory to match the version stored in that branch, and it tells Git to record all new commits on that branch.

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

* **Commit Code into local Repository:** Save snapshots of development efforts within working branch and completes the change-tracking process. Working in Git and saving changes is two step process.
  * **Add Changes :** The `git add` command adds a change in the working repository to the staging area. It tells Git that include particular file in the next commit.
  * **Git Commit :** The `git commit` command captures a snapshot of project's currently staged changes. Committed snapshots can be thought of as “safe” versions of a project—Git will never change them unless you explicitly ask it to.

{% tabs %}
{% tab title="Git Add" %}
```
$ git add .
$ git add all
$ git add <fileNam>
$ git add <directory>
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
$ git commit -m ["commit message"]
```
{% endtab %}

{% tab title="Links" %}
```
https://www.atlassian.com/git/tutorials/saving-changes
```
{% endtab %}
{% endtabs %}

{% hint style="info" %}
BRANCH-NAME format =&gt; MAI_\(DeveloperName\)_\(TaskNumber\)\_\(CommitMessage\)
{% endhint %}

\*\*\*\*

\*\*\*\*

1. **Open a pull request:** Pull requests publish a project’s ongoing efforts and set the tone for a transparent development process.
2. **Discuss and review code:** Teams participate in code reviews by commenting, testing, and reviewing open pull requests. Code review is at the core of an open and participatory culture.
3. **Merge:** Upon clicking merge, GitHub automatically performs the equivalent of a local ‘git merge’ operation. GitHub also keeps the entire branch development history on the merged pull request.
4. **Deploy:** Teams can choose the best release cycles or incorporate continuous integration tools and operate with the assurance that code on the deployment branch has gone through a robust workflow.



sdfsf

If you are beginner with Git then first of all visit following links.

* [https://guides.github.com/](https://guides.github.com/).
* \*\*\*\*[**https://www.youtube.com/playlist?list=PLg7s6cbtAD17Gw5u8644bgKhgRLiJXdX4**](https://www.youtube.com/playlist?list=PLg7s6cbtAD17Gw5u8644bgKhgRLiJXdX4)\*\*\*\*
* \*\*\*\*[**https://www.atlassian.com/git/tutorials**](https://www.atlassian.com/git/tutorials)\*\*\*\*
* \*\*\*\*[**https://learngitbranching.js.org/**](https://learngitbranching.js.org/)\*\*\*\*
* \*\*\*\*[**http://git-school.github.io/visualizing-git/**](http://git-school.github.io/visualizing-git/)\*\*\*\*
* \*\*\*\*[**https://github.github.com/training-kit/downloads/github-git-cheat-sheet/**](https://github.github.com/training-kit/downloads/github-git-cheat-sheet/)\*\*\*\*

