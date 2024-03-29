---
title: "Using git in VSCode"
---

&nbsp;

This is a short guide on how to use **git** in **Visual Studio Code** (VSCode). The purpose of git is to allow you to easily share your code with collaborators and track the changes each of you make.

**Note:** We assume you have already signed up for GitHub and installed git on your computer. Otherwise, see step 3 in this [guide](/guides/python-setup/).

&nbsp;
<!-- 
<img src="https://github.com/NumEconCopenhagen/NumEconCopenhagen.netlify.com-v2/raw/master/content/guides/vscode-git/create-repo.gif" alt="create-repo" width="80%"/>
<br />
<br />
 -->
### Cloning a repostiory

<br /><kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>P</kbd> + run `git: clone` + write link to repository (from e.g. step 1)

&nbsp;

### Working with a repostiory

&nbsp;

1. Open folder with repository (e.g. the one you just cloned in step 2)
2. Download existing changes: <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>P</kbd> + run `git: sync`
3. Make some changes, add/remove files, etc. (it does not matter whether it is done in VSCode, JypterLab or from your OS)
4. Upload new changes: 
  
    1. <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>P</kbd> + run `git: commit all` (choose "Always" if there is a pop-up)
    2. Write commit message
    3. <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>P</kbd> + run `git: sync` (choose "OK, don't show again" if there is a pop-up)
    
&nbsp;

<p style="font-size: 20px;"><strong>IMPORTANT NOTE</strong>: To avoid merge conflicts always download existing changes, before you make new ones. This reduces the risk of merge conflicts, where you and your collaborators have changed the same lines of code</p>
<!-- 
<img src="https://github.com/NumEconCopenhagen/NumEconCopenhagen.netlify.com-v2/raw/master/content/guides/vscode-git/git-clone-commit.gif" alt="git-clone-commit" width="80%"/>
<br />
<br /> -->

&nbsp;

### 4. Video guides for working with Git
1. Victor and Christian create a repository and **push their project** to it [here](https://youtu.be/nWFeHsCAtpE).
2. A short explanation of **important concepts and commands** in Git, also found in L05, can be seen [here](https://youtu.be/XqxcvWcpEtI).
3. In [this video](https://youtu.be/Aa-qQwNwak0), you'll see some examples of how to make **additional commits** across members to the project that Victor and Christian had uploaded. Also, solving **merge conflicts**. 

&nbsp;

### 5. Merge conflicts

<br />*Skip this if you are a first time user of git*

If you get a **merge conflict**:

1. Resolve conflicts by point-and-click (don't save the file)
2. <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>P</kbd> + run `git: stage all changes`
3. <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>P</kbd> + run `git: commit all`
4. <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>P</kbd> + run `git: sync`
5. Save the file
6. <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>P</kbd> + run `git: commit all`
7. <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>P</kbd> + run `git: sync`

&nbsp;

**Problems?** You can undo last commit with `git: undo last commit`

**Worst case:** Make a new clone of the repository and redo the changes file-by-file.