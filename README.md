# github_actions
GitHub actions is a tool that lets you automate your software development workflows. GitHub actions is the most common tool used to build CI/CD pipelines.

So let's say you have a GitHub repository and on this repository event can happen, an event like someone pushed a script or a pull request was opened or an issue was created or closed, and so on.

And these things are referred to as events. And we would like to perform a workflow when these events happen.

A workflow can contain one or more jobs and each job runs on its virtual machine.

A virtual machine will be booted up for each job that we have in our workflow and this virtual machine can be a Windows machine or a Linux or a Mac OS. We can define the OS directly in the workflow. For each job, we define a bunch of steps and each step should either act. This step who performs these jobs is known as a Github runner.

In a nutshell, every workflow consists of several different core concepts. These include:

    Events : Events are defined triggers that kick off a workflow. They can be set to run on specific coding branches within a given repository on GitHub.

    Jobs : Jobs are a set of steps that execute on the same runner. Each runs in its VM and parallel to other jobs.

    Steps : Steps are individual tasks that run commands in a job. These can be an action or a shell command. All steps in a job execute on the same runner.

    Actions : An action is a command that is executed on a runner and the core element of GitHub Actions, which is named after it.

    Runners : A runner is a GitHub Actions server. It listens for available jobs, runs each in parallel, and reports back progress, logs, and results. Each runner can be hosted by GitHub or self-hosted on a localized server. GitHub Hosted runners are based on Ubuntu Linux, Windows, and macOS

Our first workflow

So now let's now create our first GitHub workflow. You will need to use your GitHub account. We will run a workflow broken down into 3 jobs on different versions of Ubuntu.
