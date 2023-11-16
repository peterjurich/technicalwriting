# Connecting a Snake file to GitLab

This documentation will show you how to connect your Snakefile to GitLab so you can maintain your files in one place.

### Prerequisites

You first need to <a href="https://wiki.converge.gene.com/en/quickstart/integrating-gitlab-with-converge" target="_blank">intergrate GitLab with your Converge workspace</a>.
. 
## Step 1: Create a new repository in GitLab
1. From your GitLab home screen at code.roche.com, click the "+" symbol in the upper left corner and choose "New project/repository".

<img src="/img/create-project.png" alt="Click the + symbol to create a new project." width="300"/>

2. Choose "Create blank project".
3. Name your project.

For the purposes of this example, we will call it "test-snakemake-workflow". But anywhere you see that name in these instructions, you will insert your own project name.

4. Click "Create project" at the bottom of the page.

This will take you to your new repository.

## Step 2: Clone your new repository locally

1. Click on the "Clone" button on the right side of the screen. It is next to the "Find file", "Edit", and download buttons.
2. Copy the URL under "Clone with SSH" by clicking on the clipboard icon to the right of that URL.

![clone-project.png](/img/clone-project.png)

3. Go to your Terminal and run the command `git clone [copied URL]`.
For example:
```
git clone git@ssh.code.roche.com:jurichp/test-snakemake-workflow.git
```

While your repo may currently be empty, you are now connected to GitLab and can sync this repo with the one in GitLab.

## Step 3: Create a Snake file
Now that you are connected to GitLab locally, you are ready to create your first Snakefile with your preferred text editor. We recommend VS Code due to its usability and GitLab integration. <a href="https://code.visualstudio.com/download">Click here to download VS Code</a>.

For information on how to create a Snakefile, your best resource is going to to be <a href="https://snakemake.readthedocs.io/en/stable/tutorial/basics.html" target="_blank">the official Snakemake documentation</a>.

While the specifics of a Snake file are yours to define, here are some high level suggestions for your Snakefile:

#### Define Rules

Start by defining rules within your Snakefile. Each rule outlines a specific task and includes attributes like input, output, shell commands, threads, and resources.

#### Specify Threads and Resources

For each rule, specify the number of threads and resources required. Threads indicate parallel processing capability, while resources determine memory and CPU allocation.

#### Use Variables and Parameters

Define variables and parameters in your Snakefile for customization. These can be referenced within rules to make your workflow flexible.

#### Set Inputs and Outputs

Define the input and output files for each rule. Inputs are files needed for the task, while outputs are generated as a result.

#### Include Shell Commands

Inside each rule, incorporate shell commands that describe the task's execution process. These commands manipulate inputs to create desired outputs.

**Similarly**, here are some suggestions for what to do with a Snake file once it's complete.


#### Execution on Kubernetes

Ensure you have the required tools and configurations to execute Snakemake workflows on Kubernetes clusters.

#### List Available Tools

Use the `ml avail` command to list tools and utilities available for use within your Snakefile. This helps identify compatible tools.


#### Edit and Customize

Open your Snakefile in a text editor or IDE and customize rules, variables, parameters, and commands to suit your specific workflow.

#### Execute and Monitor

Execute your Snakemake workflow using your custom Snakefile.
Monitor the execution process, review logs, and address any errors or issues encountered during the run.

For the sake of this documentation, an example Snake file would look similar to this:
```
rule all:
  input: "output/{filename}.output.txt"

rule hello_world:
  input: "input/{filename}.txt"
  output: "output/{filename}.output.txt"
  shell:
    echo "Hello world, {filename}!" > {output}
```


## Step 4: Stage Snake file into git
1. In Terminal, run the command `git add Snakefile` to stage your file.
2. Run `git commit`.
3. Run `git push` to push commit changes into your repository in GitLab.
4. Go to your test-snakemake-workflow repository in GitLab and you should see your Snakefile.
> NOTE: If you click into your Snakefile in your GitLab repo, you will be able to edit it in your remote workspace. However, these changes will **not** be reflected locally. {.is-warning }

## Step 5: Connect Snake file to local Converge workstation

Before you move on, be sure that you have a Converge workstation set up. [Click here for more info on how to do that](/getting-started).

1. **While logged into your Converge workstation**, repeat all of "Step 2: Clone your new repository locally" above.

You will now be able to edit your Snake file in Converge. Push it to your remote repository in GitLab by repeating Step 4 above, also while logged into Converge.
