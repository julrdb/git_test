# The Odin Project

## Prereq and Git
<details>
  <summary>GIT & SSH</summary>
  <p>
    
  ### Git setup
    
  ##### To configure Git:
  
  ```shell
  1. git config --global user.name "Your Name"
  2. git config --global user.email "yourname@example.com"
  ```
  ##### Changing default repo branch from `master` to `main`:
  
  ```shell
  git config --global init.defaultBranch main
  ```
  ##### For MacOS only; to ignore .DS_store files:
  
  ```shell
  1. echo .DS_Store >> ~/.gitignore_global
  2. git config --global core.excludesfile ~/.gitignore_global
  ```
    
  ### SSH Key Setup
    
  ##### To generate ssh key:
  
  ```shell
  ssh-keygen -t ed25519 -C <youremail>
  ```
  ##### To display your ssh key to copy onto GH:
  
  ```shell
  cat ~/.ssh/id_ed25519.pub
  ```
    
  ### Git Basics <sub>[R. click this, open new tab](https://www.theodinproject.com/lessons/foundations-git-basics)</sub>
  
  <summary>The setup to create new repo on GH:</summary>
  
  ```markdown
  1. New Repository
  2. Give it a name; add a `README` file; create repo.
  3. Click `Code`, select `SSH` option, copy to clipboard.
  4. On terminal, `cd ~` (to be on home folder);
  5. `mkdir repos` create a repo folder
  6. `cd repos/`
  7. `git clone git@github.com:julrdb/git_test.git`
  ```
  <summary>Create files on local and updating on GH:</summary>
  
  ```markdown
  1. On terminal, `cd repos/git_test/` 
  2. `touch test_local.txt`
  3. `git add test_local.txt`; this adds to staging area in Git.
  4. `git commit -m "Your commit message here"`
  5. `git push` (if you're only working on main, no branch) or `git push origin main` (to be explicit)
  ```
  <summary>Create files on GH and updating on local:</summary>
  
  ```markdown
  1. On GH, don't forget to `Commit changes` on the file being edited.
  2. On terminal, `cd repos/git_test/`
  3. `git pull`
  4. Enter passphrase if you have one
  ```
  </p>    
</details>



## HTML Foundations

<details>
<summary>HTML Boilerplate (from VSCode, type "!"):</summary>

  ```HTML
  <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
  ```
###### Breakdown:
  **DOCTYPE** -declaration that tells the browser what version of HTML it should use to render.
  
  **lang** -this attribute sets the language of the text content; primarily used to improve accessibility.
  
  **head** -this is where you'd put meta-information about the webpage.
  
  **meta charset** -proper encoding so that special symbols and chars are displayed correctly.

  **title** -this gives a readable title on the webpages's browser tab.
  
  **body** -this is where all the content will go.
  
</details>
