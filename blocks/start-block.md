# Home block

## Home block overview
The Home block is the root of your project and cannot be deleted. The Home block houses both the Start step which is the first step that is opened once your project is launched, and Commands which are reusable flows.

<img src="https://i.imgur.com/J0YdL5T.png" alt="img" style="zoom:30%;" />

## Features of the Home block
- Starting projects
- Creating Command flows
- Cannot be deleted
- Every flow has a Home block

### Starting projects
Every Home block has a Start Step which is where a project will be launched. When a project is launched, it will happen from the Start Step's path within the Home block.

### Creating Command flows
Commands, also known as Command flows, can be created and housed within the Home block. Each Home block within a project, because there can be multiple on different flows, can create and house Commands.

### Cannot be deleted
The Home block cannot be deleted because it is the root of your project, and where it starts.

### Every flow has a Home block
Every flow has its own unique Home block and Start step. So, it is possible to have many Home blocks within your project if you have multiple flows. However, you can only have one Home block per flow.

### Common errors
- If the Start Step within the Home Block is not linked to another Step or Block, the project will not say anything and close on opening.
- If a Command is invoked but empty, the project will stall.

Last updated: May 27th, 2020 <br>
Written by: braden@voiceflow.com