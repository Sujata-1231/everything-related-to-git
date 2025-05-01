### git init

- The git init command creates a new Git repository. It can be used to convert an existing, unversioned project to a Git repository or initialize a new, empty repository. Most other Git commands are not available outside of an initialized repository, so this is usually the first command you'll run in a new project.
- We can follow this url to know more. [git init | Atlassian Git Tutorial](https://www.atlassian.com/git/tutorials/setting-up-a-repository/git-init)
- We can follow this url to know how to setup the repo thing [setting-up-a-repository](https://www.atlassian.com/git/tutorials/setting-up-a-repository)

### git config

- The git config command is a convenience function that is used to set Git configuration values on a global or local project level. These configuration levels correspond to .gitconfig text files. Executing git config will modify a configuration text file.

- The most basic use case for git config is to invoke it with a configuration name, which will display the set value at that name. Configuration names are dot delimited strings composed of a 'section' and a 'key' based on their hierarchy. For example: user.email

To know more we can visit here.. [setting-your-username-in-git](https://docs.github.com/en/get-started/git-basics/setting-your-username-in-git)

```js
# Check your Git username
git config user.name
# If it returns nothing, set your GitHub username
git config user.name "your-github-username"

# Verify the change
git config user.name
# This should now return your GitHub username (can see screenshot below)

# Note: The same applies for your email

# Check your Git email
git config user.email
# If it returns nothing, set the email associated with your GitHub account
git config user.email "your-email@example.com"

# Verify the change
git config user.email
# This should now return the email linked to your GitHub account

```

![Application Screenshot](images/username.png)

#### Why we generally do configure user.name and user.email in Git ?

- To Identify the author of each commit.
- Without setting user.name and user.email, Git won’t allow you to commit (in most cases), or it will use default/global settings, which might not match your GitHub account.

#### Multiple Accounts or Machines

- If you're using:
- Multiple GitHub accounts
- Shared or new machines
- You should set the correct user.name and user.email locally per repository, so your commits remain correctly attributed.

### Set Globally (for all repositories on your machine):

```js
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

### Set Locally (for one specific repo):

```js
git config user.name "Your Name"
git config user.email "your-email@example.com"
```
