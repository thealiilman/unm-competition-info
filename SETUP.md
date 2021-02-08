# Setup
For setup, we will go through 5 things.

1. How to create a GitHub account
2. How to use this repository as a template
3. How to setup development environment
4. How to setup the back-end
5. How to setup the front-end

## 1. How to create a GitHub account
This one is straightforward. Visit [_Join GitHub_](https://github.com/join), enter details into the form and submit.

## 2. How to use this repository as a template
<details>
To use this repository as a template, these are the steps.

1. Click the _Use this template_ button
![https://i.imgur.com/EBqlDz2.png](https://i.imgur.com/EBqlDz2.png)

2. Set a name for our repository and click _Create repository from template_ button. Feel free to select a private repository or a public repository.
![https://i.imgur.com/8xGcKG4.png](https://i.imgur.com/8xGcKG4.png)

And there we go! You've created a repository from this template.

### IMPORTANT NOTICE
Should you use a private repository and want your teammates to access the repo, visit the following page.
https://github.com/your-github-username/repository-name/settings/access

Clicking the _Invite a collaborator_ button will open a modal where you can enter the usernames of your teammates.

</details>

## 3. How to setup development environment
We have two categories here. macOS and Windows. Please choose the appropriate category based on your operating system.

### macOS
<details>
  
#### 1. Check whether you have Homebrew installed
[Homebrew](https://brew.sh/) is a package manager for macOS and Linux. We require this to install tools that help with running Ruby.
Check whether Homebrew is installed by running the following command.
```zsh
brew
```
If Homebrew is installed, running `brew` should print this to your terminal.
```zsh
aliilman$ brew
Example usage:
  brew search [TEXT|/REGEX/]
  brew info [FORMULA...]
  brew install FORMULA...
  brew update
  brew upgrade [FORMULA...]
  brew uninstall FORMULA...
  brew list [FORMULA...]

Troubleshooting:
  brew config
  brew doctor
  brew install --verbose --debug FORMULA

Contributing:
  brew create [URL [--no-fetch]]
  brew edit [FORMULA...]

Further help:
  brew commands
  brew help [COMMAND]
  man brew
  https://docs.brew.sh
```

If you see something like this printed:
```zsh
aliilman$ brew
bash: command not found: brew
```
This means you need to install Homebrew. You can do this by running this command in your terminal.
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

#### 2. Check whether you have rbenv installed
[rbenv](https://github.com/rbenv/rbenv) is a tool to manage Ruby versions on our machine.
To check whether you have Ruby 3.0.0 running, run the following command.
```zsh
rbenv
```
If it prints the following:
```bash
aliilman$ rbenv
bash: command not found: rbenv
```
Then you'll need to install rbenv. Check out this guide by rbenv on how to install rbenv using Homebrew.
https://github.com/rbenv/rbenv#homebrew-on-macos

#### 3. Install Ruby 3.0.0
Now that you have rbenv installed, it's time to install Ruby 3.0.0.
```bash
rbenv install 3.0.0
```
Then, run the following command to set the version of Ruby on your machine to 3.0.0.
```bash
rbenv global 3.0.0
```

</details>

## 4. How to setup the back-end
<details>

1. Run `bundle install` to install packages used on the project
2. Run `rails db:create` to create databases

And now, `rails s` should work!

</details>

## 5. How to setup the front-end
