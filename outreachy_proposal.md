# Outreachy Proposal: Crowdsourcing Translation for CHAOSS Diversity & Inclusion Badging

> Ore-Aruwaji Oloruntola
>
> Landmark University Omu-aran
>
> Kwara, Nigeria
>
> [GitHub](https://github.com/thecraftman) | [LinkedIn](https://www.linkedin.com/in/oloruntola-ore-aruwaji-5a332314a/)

## Synopsis

This project aims to make the process for obtaining badges for events & projects multilingual. 
Based on CHAOSS D&I standards, integration of multiple languages will help streamline the Badging process to be more simplified and flexible thereby making the process quick and easy-to-follow. 

The repositories for the CHAOSS Badging can be found on github [here](https://github.com/badging).

The mentors for my project are [Matt snell](https://github.com/Nebrethar), [Matt Germonprez](https://github.com/germonprez), [Saleh Abdel Motaal](https://github.com/smotaal). 

## Benefits to the community 

A lot of texts, documentation are written in languages which people don't understand. They find it difficult to communicate the problem they are having because they don't understand the native language in which it was implemented. This project will "automate source content updates for translation" into different languages (https://crowdin.com/features). This would afford applicants translated documentation to better assist them navigate the process. It would also make it possible to render viewer-based localizations for badges.

## Current status of the project 

The CHAOSS Badging project is made up of five repositories, a submission template for badging, Documentation about the Badging project, issues based on D&I badging, source texts `.md` about the event and project guidelines (https://github.com/badging).

## Goal 
Build a Collaborative translation process

This process will handle both the projects and events documentation translation based on the applicants choice from different regions, who are interested in obtaining D&I Badging. This process will validate "the synchronization of source text and translated content to ensure" flexibility with integrated tools (https://crowdin.com/teams/engineering).

## Deliverables 

### Deliverable 1: Bring all content together

Identify and localize contents for translation written in the markdown format in a single repository on Github, this will enable an ideal structure that will be implemented. This model will give the maintainers, reviewers and applicants a way to discuss which contents, documentation needs to be translated, ask questions about the D&I badging translation, and also request more content. 

### Deliverable 2:  Integrate the workflow using Crowdin

After the first deliverable, the workflow needs to be automated using Crowdin. Crowdin is a translation and localization management platform that will integrate the development processes of badging from the repository  into deployable translations on github that will be ready for publication (https://crowdin.com/features).

This automation keeps the source content "up to date for translating […], and previously-translated content is returned automatically" (https://crowdin.com/teams/engineering).

### Deliverable 3: Document/Scale more repositories 

After deliverable two, it is important to scale more repositories that will have multilingual documentation for a seamless user experience, this helps applicants to get their project/event badge in several languages at once especially in their own specified language. 

The documentation will have a summary of the guidelines and methods involved for applicants and reviewers.

## Expected results 

After the integration of the workflow; 

1.  Translation status and project activity 
The implementation of this will enable translators,reviewers, maintainers and proofreaders to become more efficient in providing better translations.  
Also, through voting, the best translation is chosen collaboratively. 

2.  Comments and Issues
Maintainers, reviewers will be able to ask questions, this will be in the form of a Pull request template. comments on the file/repository will be made on  CHAOSS Badging. They will also get feedback based on each activity, and request for more context if need be.

3.  Multilingual source texts
Accessibility of the badging source texts will be made available in different languages.


## Approach

Workflow Automation using Crowdin & Github 
(https://support.crowdin.com/github-integration/#connecting-github-with-crowdin)

The platform that is currently used for CHAOSS Badging is github. Integration with GitHub makes source and translation files synchronized with the GitHub repository and Crowdin translation project, where "translated and approved files will be automatically pushed as a pull request" back to GitHub (https://support.crowdin.com/github-integration/).

### Github integration with Crowdin is divided into four parts 

1. Connecting GitHub with Crowdin
Github accounts will be linked with Crowdin, your accounts can be a personal account or an Enterprise account for integration.
The integration process setup will be linked with the repositories and branches that should be translated. 
 Crowdin sends the pull requests from the branches that have been translated to the version system.

For every branch that is under localization, Crowdin creates additional service branches with translations. Commits will not go directly to the master branch, so that we can verify if it’s the right translation that happened.


Branches to Sync Automatically
 - Features will be added from branches  to Crowdin automatically, creating a pattern for the branch names. The branch name will follow a certain pattern that  will be automatically added to Crowdin.
 
- For example, you add a pattern *feature in the GitHub integration. 
In this case, the future branches that contain this word at the end of the title will be added to the repo. 
(“https://support.crowdin.com/github-integration/#connecting-github-with-crowdin”)

2. Selecting Content for Synchronization
Specification of source files needs to be translated before the integration can work. Crowdin will provide a framework for translated files in the repository. 

I will create a configuration file using the yaml format, this would be stored in the Github repository with each separate branch that needs to be translated. 
Through this synchronization, Crowdin will be able to know what files exactly that should be sent for translations.

3. Synchronization Schedule
After synchronizing the content, all related source texts are stored in the same place in the github section; a time interval is needed so that the synchronization can be done instantly. 

4. Checking the Status of Synchronization
Once the integration is set up, all the related source texts are stored in the same place – Projects, Integrations, GitHub section. 



Technologies 
- Languages: YAML 
- Framework: Crowdin
- Platform: Github
- Markup: Markdown for writing documentation 
     


| Period                | Task                                                                                 |
| --------------------- | ------------------------------------------------------------------------------------ |
| April 7 - May 8       | More contributions to CHAOSS Badging                                                 |
|                       | Gather more contents about Badging                                                   |
| May 8 - May 31        | Discuss with mentors on any changes or feedback                                      |
|                       | Gather more content about Crowdin workflow                                           |
|                       | Create framework for guidelines                                                      |
| June 1 - June 14      | Meet mentors for feedback and act accordingly                                        |
|                       | Gather repositories for translation                                                  |
|                       | Get more content, guidelines and procedures that needs to be translated              |
| June 15 - June 30     | Meet mentors for feedback and make changes                                           |
|                       | Gather more knowledge about multilingual languages that will be implemented          |
| July 1 - July 5       | Phase one Evaluation                                                                 |
| July 6 - July 28      | Automate workflow on Github                                                          |
|                       | Implement translators                                                                |
|                       | Integrate the Crowdin workflow on github processes                                   |
|                       | Synchronize schedule configuration -Gather feedback from mentors and act accordingly |
| July 29 - July 31     | Phase two evaluation                                                                 |
| August 1 - August 16  | Start Documenting the workflow                                                       |
|                       | Add/scale more repositories                                                          |
|                       | Fix any issues that might come up                                                    |
| August 17 - August 25 | Wrap up Documentation                                                                |
|                       | Ask mentors for feedback                                                             |
| August 26 - August 31 | Submit final work report                                                             |


## About me

I am Ore-aruwaji Tola currently in my final year studying Electrical & Information Engineering.  I am a  staunch advocate of Open source technologies. I have been contributing to the CHAOSS D&I Badging project for over 2 months. I have experience in AWS, Devops, python and Linux. 

### Contributions to the CHAOSS D&I Badging program

- https://github.com/badging/diversity-and-inclusion/pull/2
- https://github.com/badging/meta/issues/6
- https://github.com/thecraftman/CHAOSS-microtasks/blob/master/Microtasks_solution.md
- https://github.com/thecraftman/CHAOSS-microtasks
- https://github.com/thecraftman/CHAOSS-microtasks/blob/master/Draft_PR_Event_Badge.md

### Contributions to Open Source

- https://github.com/thecraftman/NAT-Gateway
- https://github.com/thecraftman/Python-REST-APIs
- https://github.com/thecraftman/Tic-Tac-Toe---Python-

### Why CHAOSS?
I am very much interested in CHAOSS because i really want to make an impact with an open source community and CHAOSS was my best choice. I want to use my skills to develop methodologies, guidelines about how Badging can be accessible to all participants for their projects and events.  CHAOSS D&I mentors have really been helpful making me understand how badging works and the methods involved. It is an honour to work with them.

### Availability 
I will be available full time, 40 hours a week. I will be in contact with the mentors if there are any changes that will take place.  I plan to communicate with the mentors through Zoom calls and Emails.  

For more information, please email temitopetola@gmail.com.
