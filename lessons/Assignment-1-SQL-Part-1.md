# SQL Intro - Assignment 1

## Requirements

- Complete [Configuring Your Machine for Ruby/Rails Development](https://learn.codethedream.org/configuring-your-machine-for-ruby-rails-development/)

## Instructions

### Set-Up

1. Fork the [`sqlintro` repository](https://github.com/Code-the-Dream-School/sqlintro)
   > _See the GitHub [**Forking a Repository**](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo?tool=webui#forking-a-repository) Docs_
2. Clone **your fork** to your workstation:
   - On the GitHub page for your fork, click the `Code` button
   - Copy the URL (HTTPS version)
     
      ![image](https://github.com/Code-the-Dream-School/sqlintro/assets/82777181/538fef7b-fb9e-452c-9b9a-b1d8a135b7d4)

   - On your workstation terminal, `cd` into the folder where you keep your assignments
   - `git clone` the repo using the copied URL
     
     ```sh
     git clone <URL>
     ```
     
     > 💡 **FYI:** _A **clone** is a copy of a respository branch._
     > 
     > _Creating a clone sets up a connection between the cloned branch on your local machine, called a **local branch**, and the same branch hosted on from where it was cloned, called a **remote branch**_
   
4. `cd` into your local clone and create a branch called `lesson1`

    ```sh
    cd sqlintro
    git checkout -b lesson1
    ```
    
5. Install the repository dependencies and make a `test.db` by copying the provided `starter.db` file:
   
    ```sh
    bundle install
    cp ./starter.db ./test.db
    ```

6. Finally, start up the `sqlcommand` program with:

    ```sh
    ruby sqlcommand.rb
    ```

    > 💡 **FYI**: _You can exit the program at any time with `ctrl` + `c`_

### Assignment

Your objective is to complete the requested `SELECT` statements in the [`sql1.txt`](../.sql1.txt) file. 

For each requested statement:

1. Compose the statement
2. Test it against the database using the `sqlcommand` program
3. Once you have confirmed it works, paste it into `sql1.txt`

> ❗**If you need to restore the database to its original state:**
> 1. Exit the `sqlcommand` program (`ctrl` + `c`)
> 2. Copy starter.db to test.db again with `cp ./starter.db ./test.db`


## Submitting Your Work

To submit your work:

1. Commit and push your changes
   
   ```sh
   git add -A
   git commit -m "lesson 1 commit"
   git push -u origin lesson1
   ```
   
2. On GitHub, navigate to **your fork** of `sqlintro`
3. Create a pull request for your `lesson1` branch
   - **IMPORTANT**: Set the `base repository` to be YOUR `main` branch. GitHub will default to using the Code-the-Dream-School repo as the `base`, so you must change this.
4. Submit the link to your pull request with your homework submission.
5. DO NOT merge the pull request until your reviewer has approved it! Your reviewer may request changes.

### Making Changes

If your reviewer requests changes to your work:

1. On your local machine, return to the `lesson1` branch of the repo
   
    ```sh
    git checkout lesson1
    ```
    
3. Make the requested changes
4. Commit and push the changes as before.
   
> 💡 **FYI**: _Pushing the changes applies them to the remote copy of your branch, making the updates visible to your reviewer in your existing pull request._

This is the procedure you will follow to submit each of the class assignments.
