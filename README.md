# Teddy Garcia-Aroca GitHub

## This space is dedicated to document Teddy's research and bioinformatic projects.

# CONTENT

This GitHub repository serves as a resource for students and graduate students interested in bioinformatics applied to fungal ecology. Students can find information on the datasets available to them as well as tools for analysis and visualization here.

Our intention is to make this GitHub site available indefinitely as a resource for ongoing and future projects. If you are interested in collaborating with these repositories, please contact one of the creators.


| **CONTENTS**                                         |
| -----------------------------------------------------|
| 1. [INSTRUCTIONS](#instructions)                |
|												  |
| 2. [DATASETS](#datasets)                        |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Metadata](#metadata)                      |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Raw data](#raw_data)                      |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[analyses](#analyses)                      |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[output](#output)                      |
|																			|
| 3. [OBJECTIVES](#objectives)                             |
|																			|
| 4. [DATA ANALYSIS TOOLS](#data-analysis-tools)                             |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Donwloading genomes](#downloading_genomes) |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Assembling genomes](#assembling_genomes) |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Annotation](#annotation)                                           |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[core genome alignments](#core_genomes)                                           |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Tree Building](#tree-building)                                        |
|																			|
| 5. [VISUALIZATION TOOLS](#visualization-tools)                              |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Visualizations with R](#visualizations-with-r)                                |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Visualizing Trees With iTOL](#visualizing-trees-with-itol)|
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Making a FastANI Heatmap](#making-a-fastani-heatmap)                        |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Pan-genome Visualizations](#pan-genome-visualizations)                            |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Combining Trees and Data](#combining-trees-and-data)                            |			
| 6. [HOW TO VIDEOS](#how-to-videos)                              |



# 1. INSTRUCTIONS

The following tutorial describes what you will be expected to do in order to complete this summer fellowship. We will be using github for version control for files and outputs (figures, tables, etc.). Please, try to avoid adding large files (GB) to this repository, since the amount of space is limited. The purpose of this repository is to guide you through the process of analyzing bacterial genomic data and introducing you to version control with git, an important skill in both academia and industry these days.

## First, create a github account and then [fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo) this repository from the github website (top right corner).

<img width="479" alt="fork_repository_example" src="https://docs.github.com/assets/cb-28613/images/help/repository/fork_button.png"> 


Once you have forked the repository, you will have your own version in your GitHub account. You can see that the link to your new version of the repository has changed to:

`
"https://github.com/<your github username>/bioted.github.io.git.git"
`

## Follow the instructions below to clone this repository to your local computer/laptop and submit pull requests after changes have been made in your own computer/laptop (all done in the command line).

| Command | Description |
| :--- | :------------------------------------- |
| `git clone https://github.com/<your GitHub username>/bioted.github.io.git` | Clone your version of the repository into your laptop or computer |
| `cd bioted.github` | Change directory to where you downloaded the repository |
| `cd datasets` | Change directory to the folder containing datasets |
| `mkdir <your_name>` | Make a new folder and name it as your_name |
| `cd your_name` | Change directory to the folder with your name |
| `mkdir data` | Make a new directory for core genes |
| `cp ../../datasets/panaroo/gene_presence_absense.csv ./` | Copy your list of core genes to the current directory for further analyses |
| `cd ../../` | Go back two levels to the main folder of the repository |
| `git status` | You should be able to see the changes you made (new folder) in red |
| `git add .` | This command will help you add all the changes to the current repository |
| `git commit -m "I added pres/absence data matrix my folder"` | This command will help you commit those changes back to github |
| `git push` | This command will help you push the changes back to your forked repository |

Once you have done all of the above, you can submit a "pull request" back to the the original repository at [Summer_2022_bioinformatics](https://github.com/teddyaroca/Summer_2022_bioinformatics), for your changes to take effect on the master branch. This is an example on how to submit a pull request:

<img width="479" alt="fork_repository_example" src="https://docs.github.com/assets/cb-26570/images/help/pull_requests/pull-request-start-review-button.png">


Note: If you are having troubles when you try `git push`, follow [these](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) instructions to add your personal token in the command line.


**Congratulations! Now you have succesfully made changes to an existing repository and submitted those changes!**

This is an important skill that is widely used in bioinformatics to create new or edit existing code/programs, make data publicly available, release new information, etc... 

**Updating your local repository with any changes in the original repository**

In order to keep your repository up-to-date, I suggest running the following before starting to make changes again:

```
git fetch
```

This will simply pull any new changes made in the master branch into your local version of the repository, effectively updating any files that have been changed by other people in your group.
