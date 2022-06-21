# Contributing

## How to contribute

**1. Fork the repository**
   
Fork the `pvsas-user-guide` repository by clicking on the fork button on the top of the main repository page.

<figure>
    <img class="github-screenshot center" src="https://raw.githubusercontent.com/paralympics/pvsas-user-guide/master/docs/_img/inline/github-fork-repo.png" alt="Fork the repository">
    <figcaption>Fork the repository</figcaption>
</figure>

**2. Clone the repository**
   
Create a copy of the repository by cloning it to your machine. This is done by clicking the **Clone or download** button.

<figure>
    <img class="github-screenshot center" src="https://raw.githubusercontent.com/paralympics/pvsas-user-guide/master/docs/_img/inline/github-clone-repo.png" alt="Clone the repository">
    <figcaption>Clone the repository</figcaption>
</figure>

**3. Create a branch**
   
Change to the repository directory on your computer (if you are not already there):

 ```
 cd first-contributions
 ```

Create a branch using the `git checkout` command.
 
 ```
 git checkout -b <name-of-branch>
 ```

**4. Make necessary changes and commit**
   
Implement the changes you want and then commit those changes. Please follow our [Commit Messages](#commit-messages) guideline.
   
**5. Push your changes to GitHub**
   
Push the changes you implemented to the remote repository using the `git push` command

```
git push origin <name-of-branch>
```

Replace <name-of-branch> with the name of the branch you created in step 3.

**6. Submit your changes for review**
   
When you go to the repository on GitHub, there will be a `Compare & pull request` button. Click that button to compare changes across the two branches to analyse if your changes will be automatically merged. 

<figure>
    <img class="github-screenshot center" src="https://raw.githubusercontent.com/paralympics/pvsas-user-guide/master/docs/_img/inline/github-compare-and-pull-request.png" alt="Compare">
    <figcaption>Compare</figcaption>
</figure>

They you now have to submit the pull request.

<figure>
    <img class="github-screenshot center" src="https://raw.githubusercontent.com/paralympics/pvsas-user-guide/master/docs/_img/inline/github-submit-pull-request.png" alt="Submit pull request">
    <figcaption>Submit pull request</figcaption>
</figure>

Once the pull request is submitted it will reviewed, and then merged. After the merge, you will receive a notification email.

**Credit**: [A Step by Step Guide to Making Your First GitHub Contribution](https://codeburst.io/a-step-by-step-guide-to-making-your-first-github-contribution-5302260a2940)

## Commit Messages

### Structure

```
{message} {description}
``` 
### Message

The message should adhere to the following requirements:
- Should not exceed 72 characters
- Write in the imperative e.g. Use "Create README" instead of "Created README"
- Provide as much context as you can
- Use consistent terminology
  
### Description

If there is more information you can add in order to provide more context for your commit message please do that but this is entirely **optional**.

### Example for a commit message

`Fix typo in README for docs`