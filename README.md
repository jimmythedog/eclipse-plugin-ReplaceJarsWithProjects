# eclipse-plugin-replacejarswithprojects

An eclipse plugin that replaces referenced jars with workspace projects

## Installation
Sorry, but manual instructions at the moment...

1. Import the project into eclipse
1. Right-click on project and select `"Export..."`
1. Navigate to `"Plug-in Development->Deployable plug-ins and fragments"`
1. Click on `"Next"`
1. You now have a couple of ways to install the plugin:
    1. Either:
        1. Use the `"Archive file"` option
        1. Once you've created the archive, unzip it into your `eclipse` directory and restart eclipse
    1. Or:
        1. Use the `"Install into hist: Repository"` option
        1. Accept the default path e.g. mine is `"/home/kevin/workspace/.metadata/.plugins/org.eclipse.pde.core/install/"`
        1. You'll probably get a dialog informing you that you are about to install unsigned code
        1. Then you should get a dialog asking you if wish to restart eclipse

## Uninstallation

1. Shutdown eclipse
1. Delete the plugin from the `eclipse/plugins` directory
1. Restart eclipse
1. If the plugin does not uninstall, restart eclipse - this time specifying the `-clean` command line argument to eclipse

## User Instructions
In the eclipse Package Explorer window:

1. Select the project(s) containing the jars you want replacing - Tip: I usually select all projects by entering `Ctrl-A`
1. Right-click to display the pop-up menu
1. Left-click on the `"Replace jars with workspace projects"` pop-up menu entry
1. Once the jars have been replaced (or not), a dialog window should appear to inform you what actions were taken. Note: the dialog title is incorrect (displays `"Problem Occurred"`) - [this issue has been logged](https://github.com/jimmythedog/eclipse-plugin-ReplaceJarsWithProjects/issues/1)
