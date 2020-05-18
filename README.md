## Welcome to FrameBlends Project 

This project is developed by Wenyue Xi (Suzie) for Google Summer of Code 2020 with Red Hen Lab

### Project Description 
- For the project idea "AI Recognizers of Frame Blends, Especially in Conversations About the Future," my proposal aims to build a semantic tagging system to detect different time frames in the conversation in the form of text or video record. Ideally, this system can classify the situation where human beings imagine a future by blending the present with incompatible frames. The project will be based on some of the existed algorithms, frameworks, and databases, and also choose and integrate them carefully to accomplish the goal. If possible, this project also aims to create an interactive system that allows humans to manually mark the false positive and true negative and keep re-training the data with such manipulation by human experts. In each round of training, the system will consider the manual marks, and eventually reach the stage when the system is able to mark the desired portion as accurate as possible. When the source data is large enough, the tagging system of the blended frame also allows us to make the unnoticed connections between current and past social conditions to gain inspiration to solve the real-world problem, or provide more evidence to the anthropological and historical studies.

## Community Boning Period 
### Preparation Stage
- May 10: Finish general set-up process of CWRU HPC and gallina home 
- May 13: Inital project meeting with Professor Turner and other mentors 
- May 14: Inital onboarding group meeting with other 2020 GSoC members 

### Blog Report #1 (May 11 ~ May 17)

#### Part 1: Completed preparation tasks 
After the initial meeting and the group meeting, I gain a more specific sense of the plan, path, and the direction of this project, and also feel supported by a professional and welcoming community. After the meeting, I review both my notes and the video recording of my initial project meeting. I summarized the tasks and finished some part of it, while setting a clear timeline of studying, planning, and coding. 

I also reach out to the student who had worked on the FrameNet project last year(Yong Zheng Xin) from LinkedIn and got his email address. Thus, I can further email him to clarify some questions about FrameNet 1.7, Semafor and Open-Sesame in the following week. I have reached out to Professor Whitehouse and Professor Uhrig, who expressed interest in my project and proposal during the group meeting. Based on the large amount of information I have received, I list and finish some small tasks before setting a detailed plan and the general project timeline. 

The following small tasks have been completed by May 18, Monday. 

- Understand Red Hen Techne Public Site in detail 
- Understand how to create Singularity and other information related to Singularity 
- Understand Red Hen Edge Search Engine and Edge2 Search Engine in detail
(e.g., How to search for linguistic patterns) 
- Explore the data from Gallina Home, be familiar with the different file extension, especially seg file 
- Be familiar with the existed frame detecting tools, such as Semafor and Open-Sesame packages (These are the packages to decide which is the best candidate for tagging) 
- Study Berkeley FrameNet website, especially Full Text Annotation
- Begin to study the book FrameNet II: Extended Theory and Practice  
- Follow the [Semafor instruction by Dipanjan Das](https://github.com/Noahs-ARK/semafor/blob/master/training/README.md) to train FrameNet 1.5 full text annotations data 
- Read about Semantics “Semantics Boot Camp” written by Elizabeth Coppock & Lucas Champollion 
- Read about MetaNet mentioned by Professor Torrent, especially the paper “Automatic metaphor detection using constructions and frames” 
- Read about Global FrameNet mentioned by Professor Torrent, especially the paper “The Multilingual FrameNet Shared Annotation Task: a Preliminary Report” 
- Reflect on Xi Jing Ping’s One Belt One Road speech video, which combined complicated visual and text to create FrameBlends, and as a great example of multimodal communication 
- Read some important presentation and publications about multimodality, including “Tutorial on Multimodal Machine Learning” from ACL 2017, “Multimodal Machine Learning: A Survey and Taxonomy”, “Multimodal Fusion for Multimedia Analysis: A Survey”, and“Deep Multimodal Learning: A survey on recent advances and trends” 


#### Part 2: Rethinking about the goal 
After the project meeting, I reflect on Xi Jing Ping’s One Belt One Road speech as an example of multimodal communication, which requires multimodal machine learning to analyze it. I have asked the question regarding different formats of data, such as visual and text, and their collaboration mechanism as the input data of frame blends detection. I realize I asked a question about multimodal communication even before I know the definition of this concept, which is the essential part of Red Hen’s mission. Thus, I’m intensively reading important publications about multimodal communication besides semantics. Of course, I will focus more on semantics since I will begin with text right now. 

This project is challenging yet inspiring; it’s related to cognitive science and the general disciplines of humanities, and aims to offer a useful tool for human analysts. For such a complicated and large-scale project, as Professor Turner mentioned in the initial project meeting with mentors, it’s better to starts with simple and small thing that works, and then build on top of it. From the initial meeting, I summarize and break down the three main goals of functionalities in a progressing manner.

- Work with existed tools to detect frame blends, identify the flaws or the biased parts, integrate or improve them
- Build an interactive system to manually enter text and frame, allow human experts labeling 
- Detect the communication about future based on detection of frame blends 

Additionally, I have some preliminary ideas about the interactive system for manually input the text and frame in the further research steps, which need to plan a comprehensive system of rules for entering data with restriction for merging the data to the original dataset. This may also need me to gain more background knowledge about cognitive science and linguistics, especially semantics. 

However, I’m not sure which steps I can eventually accomplish during this summer, so I decide to start from the first step, “Detect frame blends.” After having enough confidence in this part, I may then begin to think about the next steps. Thus, I write the third part of this blog post to begin work on “Detect frame blends.”


#### Part 3: Next step to accomplish “Detect FrameBlends”  
After studying and making the judgment from the complicated and massive information, I realize there are a lot of skills and knowledge I do not have yet, but need to have in order to accomplish the goal of this project. Those not-yet-have but have-to-gain tasks are: 

- Confirm proper dataset for training and testing from Red Hen data source 
- Deeply understand and are able to test the existed tools for detecting FrameBlends, mainly including Semafor and Open-Sesame   
- Try to test out the bias and flaws of the existed tools and explore the underlying reasons  
- Try to improve the system based on the flaws of the existed tools, or create functional integration 
- Gain more linguistics background knowledge about Semantics and Syntax  
- Gain a solid understanding about multimodal communication and multimodal machine learning 


My tentative plan for the following week(May 18 ~ May 24) shows as following(Still updating): 

- Choose the proper dataset from The UCLA NewsScape data from the gallina directory ( /mnt/rds/redhen/gallina/tv ) on CWRU HPC
- Implement and test Semafor and Open-Sesame to the chosen dataset 
- Discuss the updated research plan and questions with mentors and others who may contribute helpful suggestions 


#### Part 4: Study materials
My study materials and important websites that may be helpful for other student who takes over this project: 

- [Semafor github page](https://github.com/Noahs-ARK/semafor)

- [SEMAFOR 1.0: A Probabilistic Frame-Semantic Parser](https://www.cs.cmu.edu/~nschneid/dscs-tr.pdf)

- [Open-Sesame github page](https://github.com/swabhs/open-sesame)

- [Frame-Semantic Parsing with Softmax-Margin Segmental RNNs
and a Syntactic Scaffold](https://arxiv.org/pdf/1706.09528.pdf)

- [FrameNet Full Text Annotation](https://framenet.icsi.berkeley.edu/fndrupal/fulltextIndex) 

- [FrameNet II: Extended Theory and Practice](https://framenet2.icsi.berkeley.edu/docs/r1.5/book.pdf)

- [Invitation to Formal Semantics(Formerly known as Semantics Boot Camp)](http://eecoppock.info/bootcamp/semantics-boot-camp.pdf)

- [The syntax of natural language:An online introduction using the Trees program](https://www.ling.upenn.edu/~beatrice/syntax-textbook/)

- [Treebanks: Building and Using Parsed Corpora](https://link.springer.com/content/pdf/10.1007%2F978-94-010-0201-1.pdf)

- [Tutorial on Multimodal Machine Learning](https://www.cs.cmu.edu/~morency/MMML-Tutorial-ACL2017.pdf)

- [Multimodal Machine Learning: A Survey and Taxonomy](https://arxiv.org/abs/1705.09406)

- [Multimodal Fusion for Multimedia Analysis: A Survey](https://link.springer.com/article/10.1007/s00530-010-0182-0)

- [Deep Multimodal Learning: A survey on recent advances and trends](https://ieeexplore.ieee.org/document/8103116)



## Coding Period Before the First Evaluation 
- June 1: 
 
