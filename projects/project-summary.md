# Project Summary
This is a surface level overview of the most relevant information related to the eye tracking project. This should provide a general but non-technical understanding of what the team is trying to do. Technical documentation can be found in each projects specific README page.

## What is the project?
Our team has various research goals. First and foremost is developing eye movement data extraction tools. In short, this means that information about where a subject's eye is looking could be gathered with a simple commerical grade webcam. This would bring with it the potential for various applications such as developing new [brain-vision coordination](##Brain-Vision-Coordination) routines. And other applications could include studying UI/UX design, and [image-based studies](##Image-Based-Eye-Tracking).

## Brain-Vision Coordination
The brain-vision coordination project seeks to benefit the medical field. Notably, neuro-opthamologists can use eye tracking technology to aid in diagnosis of various neurological, visual, and motor conditions, as well as physical disorders affecting the eye. This project can be broken down into three distinct parts listed below.

Repos and documentation [here](https://github.com/TylerEgloff/temp-readme/blob/main/projects/vision-brain-coordination.md)

### Data Aquisition
To acquire eye gaze data, this project will use MediaPipe, a framework that has many uses including exporting 3-D spatial data (X,Y,Z) for landmarks around the face (click left image). We also must develop stimulus routines for subjects to be presented with, such as this revolving circle stimulus (click right image).

<div align="center">
  <a href="face-mesh.gif">
    <img src="/assets/project-summary/face-mesh-still.png" width="300"/>
  </a>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <a href="circle-stimulus.gif">
    <img src="/assets/project-summary/circle-stimulus-still.png" width="300"/>
  </a>
</div>

### Data Processing
The raw spatial geometry requires some processing to fit our needs. In short, the MediaPipe coordinates are not the only aspects of data we need, and we must extract or derive other data based on the coordinates (such as the angle of the users face relative to the camera). Some data filtering is also likely needed, for example, we may want to remove frames where subjects are blinking from our data.

### Data Visualization
After collecting data, it will need to be visualized in correspondence with what sort of stimulus was presented. To the right is a sketch of what the visualiztion for the above stimulus may look like, where the red is the path that the user's eye followed.

<div align="center">
  <img src="/assets/project-summary/circle-stimulus-visualized.png" width="300"/>
</div>

## Image-Based Eye Tracking
The image-based eye tracking project has many broad applications. One instance can be found in our medieval manuscript study, in which we studied which parts of the pages that subjects viewed during short experiments.

Repos and documentation [here](https://github.com/TylerEgloff/temp-readme/blob/main/projects/2024-medieval-manuscripts.md)

### Data Aquisition
To acquire eye gaze data, this project used a Tobii eye tracker, which ouputs X and Y coordinates that represent the viewers gaze location upon the screen. 

### Data Processing
The Tobii data we gathered was not properly calibrated, meaning that the points did not accurately reflect the viewers eye gaze location. To fix this, we developed a script to manually adjust the datapoints and also remove outliers. 

### Data Visualization
Many components were made for the visualization piece. Below are the four types of visualization we made: heatmaps, scanpaths, area-of-interest(AOI) maps, and scanpath timelines, respectively. Heatmaps are a very readable way to view the intensity of gaze in different ways. Scanpaths show the direction and time that the subjects gaze followed. AOI maps have particular regions tagged, with percentages showing how much of the time the viewers gaze fell into each tagged region. Scanpath timelines also represent where and how long gaze fell into the tagged regions, but it is an aggregation of all subjects data for each page of manuscript, where each row represents one subject.

<div align="center" style="white-space: nowrap;">
  <img src="/assets/project-summary/visualizations.jpg">
</div>

## How Can I Contribute?
This project requires a wide variety of tasks in to be successful with many different role available. Some ways that you can make a contribution to the project are by helping to review previous literature, prepare presentations, write conference papers, and develop software,  
### Reviewing Literature
In many cases, it is necessary for members of the team to familiarize ourselves with the existing literature about a subject that we are going to study to ensure that we have a solid background to base our research on and that we can contribute to the existing body of literature in a meaningful way. We also need to include the findings of previous studies in our research papers to provide some context to how our findings fit into the work that others have done and to show that we have adequate knowledge about our topic to be able to participant in the conversation surrounding it. To do this, we need members of the team to conduct in depth searches of all literature related to our study and to present relevant finding the group to use as reference for better understanding the topic, and for including in conference papers
### Preparing Presentation
After completing a study, it is likely that we will write a paper that covers the results of our research to submit at a conference. If the paper is accepted, then we must present the key findings at whatever conference we submitted to. We also might present our research in other places, like at classes or conference that take place at NKU. We need team members to create presentation slides and posters about our study to be presented at these various events.
### Writing Papers
To share our research work with others, we need to write a paper that covers all relevant information that is needed to be able the purpose, methods, and findings of our study. Papers will include background literature that is necessary to give context to where are study fits into existing research and how it can fill gap in the research, the main purpose of our research, how we conducted our study/investigated our question, what are results were, and how these results are relevant to our topic. There will need to be team members responsible for ensuring that papers have all of the necessary pieces to explain our study and its importance to others.
### Adapting/Developing Software
As the primary focus of this project is eye tracking, there are many piece of software that our team has to apply to the satisfy the needs of our research or build from scratch. There are many different types of software used in the project, but the main ones are data acquisition, data processing, and data visualization. Contributions can be made to any one or combinations of these categories.








