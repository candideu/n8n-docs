# Navigating the editor user interface

In this lesson you will learn how to navigate the Editor UI. You'll walk through the canvas and see what each icon means and where to find things you'll need while building workflows in n8n. 



## Getting started

<!-- vale off -->
First of all, you need to get n8n. There are different [ways to set up n8n](/hosting/options/){:target="_blank" .external}, choose the option that best suits your skills and needs.
<!-- vale on -->

!!! warning "n8n version"

    This course was developed on n8n version 0.175.1. In other versions, the Editor UI might look different, but the core functionality of the workflows should not be impacted.

Once you have n8n running, open the Editor UI in a browser window. It should look like this:

<figure><img src="/_images/courses/level-one/chapter-one/Editor-UI.png" alt="Editor UI" style="width:100%"><figcaption align = "center"><i>Editor UI</i></figcaption></figure>

Next, you'll learn how to navigate the Editor UI.

## Editor settings

The [Editor UI](/editor-ui/){:target="_blank" .external} represents the web interface where you build [workflows](/workflows/workflows/){:target="_blank" .external}. Think of it as a canvas on which the artist in you designs automations. From the Editor UI you can access all your workflows and credentials, as well as support pages.

### Left-side panel

In the upper left corner, click on the round arrow icon to open the left-side menu. This contains the core functionalities and settings for managing workflows.

The panel contains the following sections:

- **Admin Panel**: Access the management Dashboard (for n8n.cloud users).
- **Workflows**: Contains operations for creating and editing workflows.
- **Credentials**: Contains operations for creating credentials.
- **Executions**: Contains information about your workflow executions.
- **Help**: Contains resources around n8n product and community.

<figure style="text-align: center;"><img src="/_images/courses/level-one/chapter-one/Left-side-menu.png" alt="Editor UI left-side menu" style="height: 600px;"><figcaption align = "center"><i>Editor UI left-side menu</i></figcaption></figure>

### Top bar

The top bar of the Editor UI contains the following information:

- **Name** of the current workflow. By default, n8n names new workflows **My Workflow**, but you can edit this name anytime.
- **Tag** of the current workflow. Tags help you organize your workflows by category, use case, or whatever is relevant for you. Tags are optional.
- **Save** button that saves the current workflow.
- **Toggle** button that activates or deactivates the current workflow. By default, workflows aren't active.

<figure><img src="/_images/courses/level-one/chapter-one/Editor-UI-top-bar.png" alt="Editor UI top bar" style="width:100%"><figcaption align = "center"><i>Editor UI top bar</i></figcaption></figure>

### Canvas

The canvas is the gray grid background in the Editor UI. On the canvas, there are several icons and a node with different functionalities:

- Buttons to zoom the canvas to fit the screen, zoom in or out of the canvas, and reset the canvas to the original resolution.
- A button to **Execute Workflow**. When you click on it, n8n executes all nodes on the canvas.
- A button with a **+** sign inside. This button opens the nodes panel.
- A button with a note icon inside. This button adds a [sticky note](/workflows/sticky-notes){:target="_blank" .external} to the canvas.
- A square with a green play icon inside. This is the Start node. You will learn more about nodes in the [next section](#nodes).

<figure><img src="/_images/courses/level-one/chapter-one/Workflow-canvas.png" alt="Workflow canvas" style="width:100%"><figcaption align = "center"><i>Workflow canvas</i></figcaption></figure>

!!! note "Moving the canvas"
    You can move the workflow canvas around in two ways:

    - Click **Ctrl + Left Mouse Button** on the canvas and move it around
    - Place two fingers on your touchpad and slide

Don't worry about workflow execution and activation for now, you'll learn about these concepts later on in the course.

## Nodes

Nodes are like building blocks. When you put them together, they create an automated workflow.

!!! note "What's a node?"
    A node is an individual step in your workflow: one that either (a) loads, (b) processes or (c) sends data.

<!-- vale off -->
There are two types of nodes:
<!-- vale on -->

- **Regular Nodes** add, remove, and edit data, as well as request and send external data.
- **Trigger Nodes** start a workflow and supply the initial data.

!!! note "Core nodes"
    Some nodes don't represent an app or service. Instead, they serve general functions like scheduling workflows or adding JavaScript. n8n refers to these as core nodes.


### Start node

The [Start node](/integrations/core-nodes/n8n-nodes-base.start/){:target="_blank" .external} is the default starting point in any workflow. Every new workflow includes a Start node by default.

You can't delete or duplicate the Start node. If you have a workflow in which you don't use the Start node, you can remove the connection, deactivate it, and move it away from the workflow. If you need more than one Start node, you probably need to use other trigger nodes or create separate workflows.

You've probably figured out already that the Start node is a core trigger node. Apart from it, there are over 290 other regular and trigger nodes for various functions, apps, and services.

### Finding nodes

You can find all available nodes in the nodes panel on the right side of the Editor UI. You can open the nodes panel in three ways:

- Click the **+** icon in the top right corner of the canvas.
- Click the gray dot on the right side of an existing node on the canvas (the node to which you want to add another one) and pull the connection line to the right.
- Click the Tab key on your keyboard.

<figure style="text-align: center;"><img src="/_images/courses/level-one/chapter-one/Nodes-panel.png" alt="Nodes panel" style="width:50%"><figcaption align = "center"><i>Nodes panel</i></figcaption></figure>

In the nodes panel, notice that n8n displays the nodes in three tabs: **All**, **Regular**, and **Trigger**. Nodes are also grouped by their functionality domain (like Analytics or Sales). This makes it easier to find the nodes you need.

If you want to get a specific node, type in the name of the node, app, or service in the search field and select the respective tab.


### Adding nodes

You can add nodes by:

- Clicking on the node you want in the nodes panel. 
- Dragging and dropping the node from the nodes panel to the canvas.

If you have a node selected, n8n automatically connects the new node to the selected node.



To review, here's a walkthrough of the Editor UI touching on all the settings you've learned so far:

<figure><img src="/_images/courses/level-one/chapter-one/Editor-UI-walkthrough.gif" alt="Editor UI walkthrough" style="width:100%"><figcaption align = "center"><i>Editor UI walkthrough</i></figcaption></figure>

### Node buttons

If you hover on a node, you'll notice that four icons appear on top:

- Delete the node
- Deactivate/Activate the node
- Duplicate the node
- Execute the node

<figure><img src="/_images/courses/level-one/chapter-one/Node-buttons.gif" alt="The four node buttons" style="width:100%"><figcaption align = "center"><i>The four node buttons</i></figcaption></figure>


!!! note "Moving a workflow"
    To move a workflow around a canvas:
        1. Select all nodes with your mouse, or by clicking **Ctrl + a**.
        2. Click and hold on one of the nodes in the group.
        3. Drag the group to where you want it on the canvas.


## Summary

In this lesson you learned how to:

* Navigate the Editor UI.
* Understand what the icons mean. 
* Access the left-side and node panels. 
* Add nodes to the canvas and interpret their execution results.

In the next lesson, you will build a mini-workflow to put into practice what you've learned so far.
