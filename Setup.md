# Setup

- [Setup](#setup)
  - [Create a New Repository](#create-a-new-repository)
  - [Add Mx. Collard as a Collaborator](#add-mx-collard-as-a-collaborator)
  - [Add a Development Branch](#add-a-development-branch)
  - [Push your branch to GitHub](#push-your-branch-to-github)
  - [Initialize Your Project](#initialize-your-project)
    - [C# Project](#c-project)
    - [Unity Project](#unity-project)
  - [Create a Pull Request](#create-a-pull-request)

## Create a New Repository

Start by making a new repository

1. On GitHub, click the `+` icon in the top right corner.
2. Click the `New repository` link

![New Repository](images/New%20Repository.png)

2. Name your repository something memorable and relevant to your project
3. Select Public or Private
4. Select `Add a README.md`
5. If you're making a Unity project, you should add the `Unity` project `.gitignore` file
6. Select Create Repository

![Create Repo](images/CreateRepo.png)

## Add Mx. Collard as a Collaborator

For grading purposes, you need to add me to your repository so I can see your
work.

1. On the repository go to the settings tab

![Settings](images/settings.png)

2. On the settings page, select the `Collaborators` option on the left.

![Manage Access](images/collaborators.png)

3. On the manage access page, select `Add people`

![Add People](images/addpeople.png)

4. Search for `jcollard` and add me as a collaborator.

## Add a Development Branch

With the exception of the group project, we have mostly been working on the
`main` branch of our repositories. This is considered poor practice. The `main`
branch is typically reserved for completed work on projects. A secondary branch
called `develop` is typically created where you can work without fear of
"polluting" the `main` branch.

1. If you have not already done so, use GitHub Desktop, Clone your new repository.
2. Open your project in Visual Studio Code
3. Use the command palette (Command + Shift + P) to run `Git: Create Branch`

![Create Branch](images/createbranch.png)

4. Name your branch `develop`

![Develop Branch](images/name_develop.png)

## Push your branch to GitHub

By default, a new branch is created locally on your computer (not published). To
ensure your work is visible, you need to push your repository to GitHub.

1. Use the command palette to run `Git: Push`

![Git Push](images/git-push.png)

2. You will likely be prompted that your branch is not published. Select `Okay`
   to publish the branch.

![Publish](images/publish-branch.png)

## Initialize Your Project

Next, you should initialize your project. Skip to the section that is relevant to your project.

### C# Project

Let's start by creating a new C# project in this repository.

Before continuing, verify that you are on your `develop` branch. You can see
which branch you are on by looking in the bottom left corner of Visual Studio
Code.

![Current Branch](images/current-branch.png)

1. Clone your repository to your computer using GitHub Desktop
2. Open the cloned repository in Visual Studio Code
3. In Visual Studio Code, open a new Terminal
   * From the top menu select Terminal > New Terminal

![New Terminal](images/newTerminal.png)

4. In the terminal, run the command `dotnet new console`
   * This creates a new template C# project.

![New Console](images/newconsole.png)

If all went well, you should now see several project files in your package
explorer.

![Project Files](images/projectfiles.png)

5. If Visual Studio Code prompts you that there are missing assets, you can
   safely click `Yes`.

![Required Assets](images/required_assets.png)

1. Open the `Program.cs` file. This file contains a simple "Hello World" program
   you can run.

![Hello World](images/helloworld.png)

6. Run the project by executing `dotnet run` in your terminal.

![Run Hello](images/runhello.png)

### Unity Project

TODO: Coming Soon!

## Create a Pull Request

Next, you will push your base project to GitHub and create a Pull Request that
will allow Mx. Collard (and yourself) to see the changes that have been made to
this project.

1. Commit your work. 
   * Your commit message should be something like `chore: Initialize project`
2. Push your work.
3. In your web browser, visit your repository
4. Select the `Pull Request` tab

![Pull Request Tab](images/select-pull-request.png)

5. Select the `New Pull Request` button

![New PR](images/new-pr.png)

6. Select that you would like to pull your `develop` into your `main` branch.

![Develop](images/select-develop.gif)

7. Select `Create Pull Request`

![Create PR](images/create-pr.png)

8. Next add `jcollard` as a reviewer. (Note: This option will not be available
   until Mx. Collard accepts your invitation. You may need to skip this for now
   and add them later.)

![Add Reviewer](images/add-reviewer.gif)

9. Finally, click `Create Pull Request`

![Create PR](images/final-create-pr.png)

![Do not Merge](images/dontmerge.png)

You should now be able to see the projects that were created when you initialized your project by running `dotnet new console`. Do **NOT** click the `Merge Pull Request` button. If you do so, it will update your main branch and you will no longer be able to see the difference.

