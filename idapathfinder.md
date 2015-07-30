# Installation #

You may either copy the _idapthfinder.py_ and _pathfinder.py_ files into IDA's _plugins_ and _python_ directories respectively, or use the included installer script:

```
$ ./install.py /path/to/ida/install/directory
```

# Usage #

Run the IDAPathFinder plugin to generate a call graph from the current function:

<img src='https://idapathfinder.googlecode.com/svn/wiki/images/run_plugin.png' />

<br />
When prompted, enter the name of the target function you wish to find paths to:

<img src='https://idapathfinder.googlecode.com/svn/wiki/images/strcpy.png' />

<br />
Nodes with direct calls to the target function will be highlighted. Double clicking on any node will take you to that function in the disassembly:

<img src='https://idapathfinder.googlecode.com/svn/wiki/images/call_graph.png' />
<br />


# Filters #

Nodes can be dynamically included or excluded using the right-click menu:

<img src='https://idapathfinder.googlecode.com/svn/wiki/images/right_click_menu.png' />

<br />
To show only paths that traverse a certain node, select the **Include node** option and click on the desired node.

To exclude all paths that traverse a certain node, select the **Exclude node** option and click on the undesired node.

Include and exclude actions can be undone (but there is no re-do). Optionally, the graph can also be reset to its original state.