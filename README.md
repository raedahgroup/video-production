# Raedah Group Video Production

The purpose of this repository is to conduct and archive our video production efforts in an open and collaborative manner.
 
## What we do
We create informational videos explaining technical concepts relating to blockchain technology for the average techie.

To see what is currently being working on, check out the open issues and project-board.

### Pre-production
All pre-production materials are written in markdown. This includes scripts (paragraph format or two-column format) and storyboards.

Creating storyboards and two column scripts in markdown is necessary to allow for easy viewing directly on github, but tedious. To help with the creation and editing of two column scripts an storyboards in markdown format, mdh can be used.

#### mdh
mdh is a command line program included in this repo designed to allow quick creation and editing of two column format scripts and storyboards as markdown files. mdh is designed with a specific pre-production workflow and script/storyboard format in mind:

First, a voice over script is written in paragraph format and is named `/videoName/videoName_vo.md`  Next, a two-column script or storyboard can be genrated by mdh using the _vo.md as input. The generated markdown table representing the two column script or storyboard can then be edited by mdh.

With mdh you can easily split, add, and remove rows all without having to manually update the index column, or index specific links and filenames.