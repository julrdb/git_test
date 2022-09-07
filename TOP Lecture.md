# The Odin Project

### Git Basics
<details>
<summary>The setup to create new repo on GH:</summary>
  
  ```markdown
  1. New Repository
  2. Give it a name; add a `README` file; create repo.
  3. Click `Code`, select `SSH` option, copy to clipboard.
  4. On terminal, `cd ~` (to be on home folder);
  5. `mkdir` create a repo folder
  6. `cd repos/`
  7. `git clone git@github.com:julrdb/git_test.git`
  ```
</details>

<details>
<summary>Create files on local and updating on GH:</summary>
  
  ```markdown
  1. On terminal, `cd repos/git_test/` 
  2. `touch test_local.txt`
  3. `git add test_local.txt`; this adds to staging area in Git.
  4. `git commit -m "Your commit message here"`
  ```
</details>

<details>
<summary>Create files on GH and updating on local:</summary>
  
  ```markdown
  1. On GH, don't forget to `Commit changes` on the file being edited.
  2. On terminal, `cd repos/git_test/`
  3. `git pull`
  4. Enter passphrase is you have one
  ```
</details>
