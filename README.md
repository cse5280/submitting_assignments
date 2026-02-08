# Submitting Assignments Using GitHub (CSE5280)

In this course, programming assignments are submitted using **GitHub**.

------

## 1. Submission platform

All assignments must be submitted via **GitHub repositories**.

- Each student (or team for group assignments) submits **one private repository per assignment**
- ZIP files, screenshots-only submissions, or email submissions are **not accepted**
- ⚠️ **Important:** Submission instructions are part of the assignment and must be followed to ensure full grade. 


#### 🪟 For Windows users

If you are using Windows, we strongly recommend installing Windows Subsystem for Linux (WSL).
WSL lets you run a Linux command-line environment directly on Windows, so you can follow the Linux/macOS instructions exactly.

> **Windows Subsystem for Linux (WSL)** allows Windows users to run a native Linux command-line environment directly on Windows, enabling full compatibility with Unix-based tools and workflows.

------

## 2. Repository creation (REQUIRED)

For each assignment, students must create a **new private GitHub repository** under their personal GitHub account.

> ⚠️ **Important:** Git does *not* create GitHub repositories automatically.
>  You must create the repository on GitHub **before** pushing code. The repository must follow the naming convention described in these notes. 

**See Section:** `3. How to create your private assignment repository` for details. 

### Repository naming convention

```
cse5280-<assignment-name>-<netid>
```

- Where `<netid>` is your FIT Tracks username

**Example**

```
cse5280-animation-jdoe2026
```

### Repository requirements

- Visibility: **Private**
- Initialize with a `README.md`
- Contains only files relevant to the assignment

------


### Steps to create your private assignment repository

Assignments for this class will be provided as a GitHub repository. You will use the files in this repository the starter code for your own private repository for the assignment. 

❌ **Do NOT fork** the assignment repository
 ❌ **Do NOT submit a forked repository**

**Instead**:

1. Create your **own private repository** on GitHub.com (Follow the name convension: `cse5280-<assignment-name>-<netid>`)

2. Go to the directory where you want to work on your assignments, e.g., `~/Documents/computer_graphics/`.

3. Open a Terminal (In Windows, use the `WSL` terminal). Run the following:
   ```shell
    # Clone the assignment starter repository
    git clone <assignment-repository-URL>

    # Enter the cloned starter directory
    cd <assignment-starter-directory>

    # Remove the starter repository's Git history
    # (so you don't keep the instructor's commits)
    rm -rf .git

    # Initialize a brand-new Git repository
    git init

    # Stage all starter files for commit
    git add .

    # Create the first commit in your own repository
    git commit -m "Initial commit from assignment starter code"

    # Rename the default branch to 'main'
    git branch -M main

    # Link your local repository to your GitHub repository
    git remote add origin https://github.com/<username>/cse5280-<assignment-name>-<netid>.git

    # Push the initial commit to GitHub and set upstream tracking
    git push -u origin main
   ```
   👉 🔒 If prompted for a password, use a **GitHub Personal Access Token** (not your GitHub password). The simplest Token to generate is the Classic Access Token. Fine-grained tokens work but there are many settings to be selected. Here is the link: [Managing your personal access tokens](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens)

5. Reload the private repository page (GitHub.com) to see that the new files. 
6. Clone your private repository to create a local copy of the private repository on your local machine. To complete the assignment, you will work on the files in this local repository and then commit/push the files to the GitHub server to submit the assignment.
7. Remove the original repository of the starter code to avoid confusing it with your private repository for the assignment. 



------

## 3. Collaborators (REQUIRED)

Students **must** add the instructor and TAs as collaborators.

### Required collaborators

- **Instructor:** `eraldoribeiro`
- **Teaching Assistant:** 

> ⚠️ Repositories without correct collaborator access **will not be graded**.

------

## 4. Assignment content requirements

Each repository must include:

- ✅ All required source code (e.g., Jupyter notebooks, python scripts)
- ✅ Report in pdf and LaTeX source
- ✅ A completed `README.md` containing:
  - Student name
  - NetID
  - Assignment description
  - Build/run instructions
  - Notes or assumptions

### README template

Add the following information to the top part of the existing README.md file:

```
**Name:** Jane Doe  
**NetID:** jdoe2026
```

------

## 5. Submitting the assignment

On **Canvas**, submit **only** the URL of your GitHub repository:

```
https://github.com/<username>/cse5280-<assignment-name>-<netid>
```

No additional uploads unless explicitly requested.

------

## 6. Deadlines & late policy

- Submission time is determined by the **timestamp of the last pushed commit**
- Late submissions follow the course late policy

------

## 7. Academic integrity

- All submitted work must be **your own**
- Repositories must remain **private**
- Standard university academic integrity policies apply

------

## 8. Common reasons assignments will suffer deductions in grade

- Repository is public
- Instructor or TA not added as collaborator
- Incorrect repository name
- Forked repository submitted
- Missing README or required files
- Work not pushed before the deadline

------

## 9. Final submission checklist

- [ ]  Repository name is correct
- [ ]  Repository is private
- [ ]  Instructor (and TA) added
- [ ]  Code builds and runs
- [ ]  README completed
- [ ]  All changes pushed

