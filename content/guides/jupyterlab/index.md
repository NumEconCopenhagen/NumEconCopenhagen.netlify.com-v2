---
title: "Running Python in JupyterLab"
---


&nbsp;

JupyterLab is an awesome way of combining text and code in the same framework. This is a short guide on how to use JupyterLab. If you haven't seen JupyterLab before it looks like this: 

<img src="https://github.com/NumEconCopenhagen/NumEconCopenhagen.netlify.com-v2/raw/master/content/guides/jupyterlab/jupyterlab.gif" alt="jupyterlab" width="80%"/><br /><br />

### 1. Starting JupyterLab

<br /> *For installation of JupyterLab see step 1b [here](/guides/python-setup/)*

1. Open the program **Anaconda Prompt** (Windows) or **Terminal** (Mac)
2. Paste in `jupyter lab` + <kbd>Enter</kbd>

<br />Hopefully, you will experience that you browser automatically opens a new tab looking something like this:

<img src="https://github.com/NumEconCopenhagen/NumEconCopenhagen.netlify.com-v2/raw/master/content/guides/jupyterlab/jupyterlab-open.gif" alt="jupyterlab-open" width="80%"/><br /><br />

> **Note:** Despite JupyterLab is running in a browser, it is running offline (the path is something like *localhos:8888/lab*).

&nbsp;

### 2. Creating a notebook

<br />In the *Launcher* tab you create a new Jupyter notebook by pressing the *Python 3* bottom under *Notebook*. Notebooks consists of two types of cells:

1. Code cells with Python code
2. Markdown cells with text (see the guide [Writing markdown](/guides/markdown))

<br />When inside a cell you are in `edit mode`, when not you are in `command mode`.

The most important notebook commands are:

* Movements: Arrows and scrolling
* Run cell and advance: <kbd>Shift</kbd>+<kbd>Enter</kbd>
* Run cell: <kbd>Ctrl</kbd>+<kbd>Enter</kbd>
* Enter edit mode: <kbd>Enter</kbd>
* Enter command mode: <kbd>Ctrl</kbd>+<kbd>M</kbd>
* Change to markdown cell: <kbd>M</kbd> (only in command mode)
* Change to code cell: <kbd>Y</kbd> (only in command mode)

<br />In the left-panel on JupyterLab you can e.g. access:

1. File Browser: To open existing notebooks anywhere on your computer.
2. Running Terminals and Kernels: To shutdown terminals and kernels.
3. Command Palette: To see a list of possible commands.
4. Table of Contents: To see links to sections based on headings (#, ##, ###).

<br />The **interface of JupyterLab** is explained in detail [here](https://jupyterlab.readthedocs.io/en/stable/user/interface.html).

The use of **Jupyter notebooks** in JupyterLab is explained in detail [here](https://jupyterlab.readthedocs.io/en/stable/user/notebook.html).

&nbsp;

### 3. Variable inspector

<br />A very nice feature of JupyterLab is that it has a variable inspector that visualize vectors, DataFrames and matrices. You can open it by right-clicking in a notebook and choose "Open Variable Inspector". It looks like this:

<img src="https://github.com/NumEconCopenhagen/NumEconCopenhagen.netlify.com-v2/raw/master/content/guides/jupyterlab/jupyterlab-variable-inspector.gif" alt="jupyterlab-variable-inspector" width="80%"/><br /><br />

### 4. Shortcuts

<br />Other good-to-know standard short-cuts are:

* Only in command mode:
   * Create new cell above: <kbd>A</kbd>
   * Create new cell below: <kbd>B</kbd>
   * Cut cell: <kbd>X</kbd>
   * Copy cell: <kbd>C</kbd>
   * Paste cell: <kbd>V</kbd>
   * Delete cell: <kbd>D</kbd>+<kbd>D</kbd>
   * Toggle sidebar: <kbd>Ctrl</kbd>+<kbd>B</kbd>
   * Restart kernel: <kbd>0</kbd>+<kbd>0</kbd>
* Single-document mode: <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>D</kbd>
* Autocomplete (when writing code): <kbd>Tab</kbd>
* Show tooltip: <kbd>Shift</kbd>+<kbd>Tab</kbd> (used when inside function)
  
<br />**Advanced:** Additionally, you can create customized short-cuts. Open settings with <kbd>Ctrl</kbd>+<kbd>,</kbd>. 

1. Open 'Settings: Advanced Settings Editor
2. Open 'Keyboard Shortcuts'
3. In the `User Preferences` tab paste in the followng:

```python
{
    "shortcuts": [
        {
            "command": "runmenu:restart-and-run-all",
            "keys": [
                "Ctrl Space"
            ],
            "selector": "[data-jp-code-runner]"
        },
        {
            "command": "notebook:move-cell-up",
            "keys": [
                "Ctrl ArrowUp"
            ],
            "selector": ".jp-Notebook:focus"
        },
        {
            "command": "notebook:move-cell-down",
            "keys": [
                "Ctrl ArrowDown"
            ],
            "selector": ".jp-Notebook:focus"
        },
        {
            "command": "application:toggle-presentation-mode",
            "keys": [
                "Ctrl Shift P"
            ],
            "selector": "body"
        },
        {
            "command": "viewmenu:line-numbering",
            "keys": [
                "Ctrl Shift K"
            ],
            "selector": ".jp-Notebook.jp-mod-commandMode"
        }
    ]
}
```

<br />You now have access to the following short-cuts:

1. Restart kernal and run all cells: <kbd>Ctrl</kbd>+<kbd>Space</kbd>
2. Toggle presentation mode: <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>P</kbd>
3. Toggle line numbers: <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>K</kbd>
4. Move cell up: <kbd>Ctrl</kbd>+<kbd>&uparrow;</kbd> (only in command mode)
5. Move cell down: <kbd>Ctrl</kbd>+<kbd>&downarrow;</kbd> (only in command mode)

&nbsp;

### Next guide

<br />[Running Python in VSCode](/guides/vscode-basics)
