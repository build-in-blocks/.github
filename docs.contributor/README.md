# Git workflow guide

> [!NOTE]
> Adopted from @collabocate-osc for use in @build-in-blocks GitHub repositories.

#

> [!TIP]
> - If you don't have git installed before on your computer, please install git from here [git-scm.com/downloads](https://git-scm.com/downloads) or from here [githowto.com](https://githowto.com)
> - Follow the instruction to setup your git credentials from this page: [githowto.com/more_setup](https://githowto.com/more_setup)

#

### Fork the GitHub repo of interest

Open your web browser, navigate to the GitHub repository you wish to contribute to, and fork the repository.

#

### Clone forked repo to your local computer

**Step 1:** Open your terminal, clone your forked repository unto your local computer. Clone URL options explained below:

- **HTTPS url option:** If you are using `https` **_clone url_**, the clone command with your url will look like this:

  ````
  git clone https://github.com/your-github-user-name-here-instead/the-repo-name.git
  ````

- **SSH url option:** [See GitHub documentation for SSH configuration](https://docs.github.com/en/authentication/connecting-to-github-with-ssh) incase you wish to be able to work with SSH url for git operations (that is, if you have not set it up before). If you are using `SSH` _**clone url**_, the clone command with your url will look like this:

  ````
  git clone git@github.com:your-github-user-name-here-instead/the-repo-name.git
  ````

  #

  > [!TIP]
  > You can get the url to clone the project with, through the green code button in the repository on Github as shown below in the screenshot.

  #

  <img width="1480" alt="Screenshot 2026-03-03 at 05 23 02" src="https://github.com/user-attachments/assets/67d560b7-11ac-4c45-99ca-e3f6845743f7" />


**Step 2:** Change directory into the folder downloaded after you cloned:

````
cd the-name-of-the-folder-cloned-unto-your-computer
````

#

### Install dependencies and run project locally

For this part, refer to the **contributor guide** located at the `docs.contributor/README.md` file of the particular GitHub repository that you wish to contribute to.

Install and run the project locally on your computer as instructed in there. Then proceed to make and submit your changes as directed below.

#

### Create new branch to make your changes in

> [!IMPORTANT]  
> Except you are requested to create your branch from another branch, always create your new branch from the develop branch.

First checkout to develop:

````
git checkout develop
````

Create your branch using our branch naming convention:

````
git checkout -b @GH-replaceThisPartWithYourGitHubIssueTicketNumber
````

#

### Add, commit and push changes to remote

Make the desired changes you wish to submit to the project in your code editor. After that, add, commit and push your changes as shown below:

````
git add .
````

````
git commit -m "replace this part with a commit message that describes your changes"
````

First time pushing a particular branch to the remote, do:

````
git push -u origin replace-this-part-with-the-name-of-your-branch
````

Every other time (for that same branch), use the simpler command:

````
git push
````

#

> [!TIP]
> Go to your fork on the GitHub web UI, you should see your branch there. Send a pull request as usual.

