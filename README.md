## Welcome to FrameBlends Project 

This project is developed by Wenyue Xi (Suzie) for Google Summer of Code 2020 with Red Hen Lab

### Description 
- For the project idea "AI Recognizers of Frame Blends, Especially in Conversations About the Future," my proposal aims to create a semantic tagging system to classify different time frames in the conversation in the form of text or video record. Ideally, this system can classify the situation where human beings imagine a future by blending the present with incompatible frames. The project will be based on some of the existed algorithms, frameworks, and databases, and also choose and integrate them carefully to accomplish the goal. This system will also create an interactive system that allows humans to manually mark the false positive and true negative and keep re-training the data with such human manipulation. In each round of training, the system will consider the manual marks, and eventually reach the stage when the system is able to mark the desired portion as accurate as possible. When the source data is large enough, the tagging system of the blended frame also allows us to make the unnoticed connections between current and past social conditions to gain inspiration to solve the real-world problem, or provide more evidence to the anthropological and historical studies.

## Community Boning Period 
### Preparation Stage
- May 10: Finish general set-up process 
- May 13: Inital Meeting with Professor Turner 
- May 14: Inital onboarding meeting with other GSoC members 

### Blog Report #1 (May 11 ~ May 17)
(This report is not the most updated version by May 18 Monday. Still Editing) 

#### Part 1: Completed preparation tasks 
After the initial meeting and the group meeting, I gain a more specific sense of the plan, path, and the direction of this project, and also feel supported by a professional and welcoming community. After the meeting, I review both my notes and the video recording of my initial project meeting. I summarized the tasks and finished some part of it, while also setting a clear timeline of studying, planning, and coding. I reach out to the student who had worked on the FrameNet project last year(Yong) from LinkedIn and got his email address. Thus, I will email him to clarify some questions about FrameNet 1.7 and Semafor this week. I have reached out to Professor Whitehouse and Dr. Uhrig, who expressed interest in my project and proposal during the group meeting. Based on the rich amount of information I received, I list some small tasks before setting a timeline and a detailed plan. The following small tasks have been completed by May 18, Monday. 

- Understand Red Hen Techne Public Site in detail 
- Understand how to create Singularity and other information related to Singularity 
- Understand Red Hen Edge Search Engine and Edge2 Search Engine in detail
(e.g., How to search for linguistic patterns) 
- Explore the data from Gallina Home, be familiar with the different file extension, especially seg file 
- Be familiar with the existed frame detecting tools, such as Semafor and Open-Sesame packages (These are the packages to decide which is the best candidate for tagging) 
- Study the mechanism of Berkeley FrameNet, especially Full Text Annotation 
- Read about Semantics “Semantics Boot Camp” written by Elizabeth Coppock & Lucas Champollion 
- Read about MetaNet mentioned by Professor Torrent, especially the paper “Automatic metaphor detection using constructions and frames” (?) 
- Read about Global FrameNet mentioned by Professor Torrent, especially the paper “The Multilingual FrameNet Shared Annotation Task: a Preliminary Report” 
- Reflect about Xi Jing Ping’s speech video, which combined complicated visual and text to create FrameBlends, and as a great example of multimodal communication 
- Read some important presentation and publications about multimodality, including “Tutorial on Multimodal Machine Learning” from ACL 2017, “Multimodal Machine Learning: A Survey and Taxonomy”, “Multimodal Fusion for Multimedia Analysis: A Survey”, and“Deep Multimodal Learning: A survey on recent advances and trends” 


#### Part 2: Re-thinking about the goal of this project 
After the meeting, I reflect on Xi Jing Ping’s One Belt One Road speech as an example of multimodal communication. I have asked the question regarding different formats of data, such as visual and text, and their collaboration mechanism as the input of frame blends detection. I realize I asked a question about multimodal communication even before I know the definition of this concept, which is the essential part of Red Hen’s mission. Thus, I’m intensively reading important publications about multimodal communication besides semantics. Of course, I will focus more on semantics since I will begin with text right now. 

This project is challenging yet inspiring; it’s related to cognitive science and the general humanities, and aims to offer a useful tool for human analysts. For such a complicated and large-scale project, as Professor Turner mentioned in the initial project meeting with mentors, it’s better to starts with simple and small thing that works, and then build on top of it. From the initial meeting, I summarize and break down the three main goals of functionalities in a progressing manner.

- Work with existed tools to detect frame blend and identify the flaws and improve it 
- Build an interactive system to manually enter text and frame, allow human experts labeling 
- Detect the communication about future as frame blends 

Additionally, I have some preliminary ideas about the interactive system for manually input the text and frame in the further research steps, which need to plan a comprehensive system of rules for entering data with restriction for merging the data to the original dataset. This may also need me to gain more background knowledge about cognitive science and semantics. 

However, I’m not sure which steps I can eventually accomplish during this summer, so I decided to start from the first step, “Detect frame blends.” After having enough confidence in this part, I may then begin to think about the next steps. Thus, I write the third part of this blog post. 


#### Part 3: Next Step to accomplish “Detect FrameBlends”  
After studying and making the judgment of the complicated and massive information, I realize there are a lot of skills and knowledge I do not yet have, but need to have to accomplish this goal of the project. Those not-yet-have but have-to-gain tasks are: 

- Confirm proper dataset for training and testing from Red Hen data source 
- Understand and test the existed tools for detecting FrameBlends, including Semafor and Open Sesame   
- Try to test out the bias and flaws of the existed tools and explore the underlying reasons. 
- Try to improve the system based on the flaws of the existed tools, or create functional integration 
- Gain more background knowledge about semantics, syntax, and multimodality 


My plan for the following week(May 18 ~ May 24) shows as following: 

- Choose the proper dataset from The UCLA NewsScape data from the gallina directory ( /mnt/rds/redhen/gallina/tv ) on CWRU HPC
- Implement Semafor and Open Sesame
- Discuss the further research plan with mentors and others who may contribute helpful suggestions 
(Still updating) 

#### Part 4: Study Materials
My study materials and important website that may be helpful for other student who takes over this project: 

- Semantics 
http://eecoppock.info/bootcamp/semantics-boot-camp.pdf

- Syntax 
https://www.ling.upenn.edu/~beatrice/syntax-textbook/

- Semafor 
https://github.com/Noahs-ARK/semafor

- Open Sesame 
https://github.com/swabhs/open-sesame

- FrameNet Full Text Annotation 
https://framenet.icsi.berkeley.edu/fndrupal/fulltextIndex

- Tutorial on Multimodal Machine Learning
https://www.cs.cmu.edu/~morency/MMML-Tutorial-ACL2017.pdf

- Multimodal Machine Learning: A Survey and Taxonomy
https://arxiv.org/abs/1705.09406

- Multimodal Fusion for Multimedia Analysis: A Survey
https://link.springer.com/article/10.1007/s00530-010-0182-0

- Deep Multimodal Learning: A survey on recent advances and trends
https://ieeexplore.ieee.org/document/8103116



## Coding Period Before the First Evaluation 
- June 1: 
 
