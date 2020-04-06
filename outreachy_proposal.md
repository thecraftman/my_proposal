<hgroup>

# Outreachy Proposal:

## Crowdsourcing Translation for CHAOSS Diversity & Inclusion Badging

</hgroup>

> Ore-Aruwaji Oloruntola
> Landmark University Omu-aran
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

This process will handle both the projects and events documentation translation based on the applicants choice from different regions, who are interested in obtaining D&I Badging. This process will validate the synchronization of source text and translated content to ensure flexibility with integrated tools. 

## Deliverables 

Deliverable 1: Bring all content together 

Identify and localize contents for translation written in the markdown format in a single repository on Github, this will enable an ideal structure that will be implemented. This model will give the maintainers, reviewers and applicants a way to discuss which contents, documentation needs to be translated, ask questions about the D&I badging translation, and also request more content. 

Deliverable 2:  Integrate the workflow using Crowdin

After the first deliverable, the workflow needs to be automated using Crowdin. Crowdin is a translation and localization management platform that will integrate the development processes of badging from the repository  into deployable translations on github that will be ready for publication. (https://crowdin.com/features) 

This automation keeps the source content up to date for translating, and previously-translated content is returned automatically. (https://crowdin.com/teams/engineering)

Deliverable 3: Document/Scale more repositories 

After deliverable two, it is important to scale more repositories that will have multilingual documentation for a seamless user experience, this helps applicants to get their project/event badge in several languages at once especially in their own specified language. 
The documentation will have a summary of the guidelines and methods involved for applicants and reviewers.

## Expected results 

Part one

To achieve this workflow;

1. Crowdin pricing; The pricing for Crowdin can be classified into 
   - Personal plans (https://crowdin.com/pricing#annual)
![crowdin pricing 1](https://user-images.githubusercontent.com/24816990/78518885-958e2f80-77b9-11ea-8ae0-75e4e5cc9138.PNG)

- Organization Plans
  
  ![crowdin pricing 2](https://user-images.githubusercontent.com/24816990/78519105-2fee7300-77ba-11ea-9ce8-4953ba600922.PNG)
  
For applicants, the micro personal plan is feasible. 

2.  Translation status and project activity
This will enable translators,reviewers, maintainers and proofreaders to become more efficient in providing better translations.  
Also, through voting, the best translation is chosen collaboratively. 

3. Budget planning
This would enable applicants to manage resources effectively, they can also collaborate with other applicants to avoid excessive budgeting. 

4.  Comments and Issues
Maintainers, reviewers will be able to ask questions, this will be in form of a Pull request comment on the file/repository on CHAOSS Badging. They will also get feedback based on each activity and request for more context if need be.  

## Approach

### Workflow Automation using Crowdin & Github  (https://support.crowdin.com/github-integration/#connecting-github-with-crowdin)
The platform that is currently used for CHAOSS Badging is github, Integration with GitHub makes source and translation files synchronized with GitHub repository and Crowdin translation project. All translated and approved files will be automatically pushed as a pull request to the master branch in GitHub repository.

Github integration with Crowdin is divided into four parts 
1. Connecting GitHub with Crowdin
After signing up on Crowdin, open Project Settings, Integrations tab in Crowdin. Then you have two options. You can either use your GitHub Account or GitHub Enterprise Account integration.
![log in crowdin](https://user-images.githubusercontent.com/24816990/78521536-10f3df00-77c2-11ea-84c0-cc5067fa47fc.PNG)

![11](https://user-images.githubusercontent.com/24816990/78521605-4d273f80-77c2-11ea-988b-f0734f3de0dd.PNG)

To integrate via your GitHub Account you can click Set Up Integration and then authorize the connection with Crowdin on the GitHub side:

![12](https://user-images.githubusercontent.com/24816990/78521679-95def880-77c2-11ea-986f-d8975e9768e5.PNG)

Authorize Crowdin application on your Github account

![13](https://user-images.githubusercontent.com/24816990/78521943-99bf4a80-77c3-11ea-88aa-7ff8a146b09f.PNG)

After integration, a pop-up dialogue would appear on your Project Settings, Integrations tab in Crowdin. In the newly appeared pop-up, continue the process of integration setup selecting necessary repository and branches that should be translated.

It is recommended to switch the duplicated strings handling to the Show (Recommended for versions) setting, so equal strings will be hidden across the branches.

#### Service Branches

When translations are finished and your languages are ready to go live, Crowdin sends pull request with translations to your version control system. For every branch that is under localization, Crowdin creates additional service branch with translations. We do not commit directly to the master branch so you can verify translations first.

By default, l10n_ is added to the created service branch name. If necessary it can be easily changed.

#### Branches to Sync Automatically
When you set up the integration you select existing repository branches that should be added to the Crowdin project. To add future branches from GitHub to Crowdin automatically, create a pattern for the branch names. If a branch name follows a certain pattern, it will be automatically added to Crowdin.

For example, you add a pattern *feature in the GitHub integration settings. In this case, the future branches that contain this word at the end of the title will be added to the project.

To add a pattern for branch names, follow these steps:

- Click Edit in the GitHub integration section.
- In the pop-up dialogue click Show Advanced Settings in the bottom left corner.

![14](https://user-images.githubusercontent.com/24816990/78522194-806ace00-77c4-11ea-9a85-bb7c6c501e3c.PNG)

- In the Branches to Sync Automatically field, use wildcard selectors such as '*', '?', '[set]', '' and others to identify the necessary branches.
- Click Save.

  
![15](https://user-images.githubusercontent.com/24816990/78522251-ad1ee580-77c4-11ea-8f55-cc8a672a81b9.PNG)



Selecting Content for Synchronization
To get the integration working, you have to specify which source files should be translated and how Crowdin should structure translated files in your repository. In case, you see a red icon with an exclamatory mark next to the service branch name, this means that you didn't choose content for synchronization.

We will configure it manually by creating a configuration file 
Creating Configuration File
Configuration file crowdin.yaml should be stored in the GitHub repository along with each separate branch that you want to translate, so Crowdin knows what files exactly should be sent for translations.
It should have the same structure as required for Synchronization Tool

Synchronization Schedule
To configure the synchronization schedule – click Edit and choose the update interval.

![16](https://user-images.githubusercontent.com/24816990/78523008-451dce80-77c7-11ea-913b-0c1d990b41d9.PNG)

Checking the Status of Synchronization
Once the integration is set up, all the related information is stored in the same place – Project Settings, Integrations tab, GitHub section.
By default, synchronization is processed every 10 minutes automatically. If there's a need to launch it instantly – click Sync Now.

![17](https://user-images.githubusercontent.com/24816990/78523078-831af280-77c7-11ea-9b2e-6a039b3931ea.PNG)

Technologies 
- Languages: YAML 
- Framework: Crowdin
- Platform: Github
- Markup: Markdown for writing documentation 
     


|Period | Task  |
|-------| ------------------------------------|
|        After submission [ April 7 -  May 8]          |-  More contributions to CHAOSS Badging, - Gather more contents about Badging 
|       [MAY 8 - MAY 31]         | - Discuss with mentors on any changes or feedback -Gather more content about Crowdin workflow - Create framework for guidelines 
|       [JUNE 1 - JUNE 14]        | -Meet mentors for feedback and act accordingly -Gather repositories for translation -Get more content, guidelines and procedures that needs to be translated 
|      [ JUNE 15 - JUNE 30]       | -Meet mentors for feedback and make changes -Gather more knowledge about multilingual languages that will be implemented
|        [JULY 1 - JULY 5]       |  Phase one Evaluation
|        [JULY 6 - JULY 28]     | Automate workflow on Github -Implement translators -Integrate the Crowdin workflow on github processes -Synchronize schedule configuration -Gather feedback from mentors and act accordingly
|         [JULY 29 - JULY 31]       | - Phase two evaluation
|         [AUGUST 1 - AUGUST 16]        | - Start Documenting the workflow -Add/scale more repositories -Fix any issues that might come up 
|           [AUGUST 17 - AUGUST 25]     | Wrap up Documentation -Ask mentors for feedback
|           [ AUGUST 26 - AUGUST 31]     | Submit final work report


### About me
I am Ore-aruwaji Tola currently in my final year studying Electrical & Information Engineering.  I am a  staunch advocate of Open source technologies. I have been contributing to the CHAOSS D&I Badging project for over 2 months. I have experience in AWS, Devops, python and Linux. 

```
Contributions to CHAOSS D&I Badging
 https://github.com/badging/diversity-and-inclusion/pull/2
https://github.com/badging/meta/issues/6
https://github.com/thecraftman/CHAOSS-microtasks/blob/master/Microtasks_solution.md
https://github.com/thecraftman/CHAOSS-microtasks
https://github.com/thecraftman/CHAOSS-microtasks/blob/master/Draft_PR_Event_Badge.md

My other Open Source contributions

https://github.com/thecraftman/NAT-Gateway
https://github.com/thecraftman/Python-REST-APIs
https://github.com/thecraftman/Tic-Tac-Toe---Python-
```

### Why CHAOSS?
I am very much interested in CHAOSS because i really want to make an impact with an open source community and CHAOSS was my best choice. I want to use my skills to develop methodologies, guidelines about how Badging can be accessible to all participants for their projects and events.  CHAOSS D&I mentors have really been helpful making me understand how badging works and the methods involved. It is an honour to work with them.

### Availability 
I will be available full time, 40 hours a week. I will be in contact with the mentors if there are any changes that will take place.  I plan to communicate with the mentors through Zoom calls and Emails.  

### For more information, send an email to temitopetola@gmail.com








