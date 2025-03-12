# ai-startup-website
This is my first repository as a DevOps Engineer.


## PART 1 - Setting up and initial configuration
1. Install Git on windows from official Git website
2. Create a Git repository

  - Login to Github
  - Create a new repository, name it as **"ai-startup-website"** and initiate with a README file
  - Add description


    ![Alt text](image1.png)

3. Clone the repository
  - Click **"code"** button on repository page and copy the HTPS URL
  - Open terminal and create a directory named **"git-project"**
  - Change directory into the **git-project** dirctory
  

>git clone https://github.com/Damilaresobulo/ai-startup-website.git

 ![Clone Repository](image2.png)

 - Navigate into the cloned repository **"ai-startup-website"**
 
 > cd ai-startup-website
 - Create empty file and name it **"index.html"**

>vim index.html

- Add contents below
> This is the Admin creating an index.html file for Tom and Jerry
- Check if changes have not been staged
>git status

![index.html file](image3.png)

- Stage changes
> git add index.html
- Confirm changes
> git status

![staging changes](image4.png)

- Commit changes and attach a meesgae indication the change. The "-m" allows us to attach a message or a descriptor to the change commited

> git commit -m "This is my first commit"

- Push main branch to Github remote

> git push origin main

## PART 2 - Simulating Tom and Jerry"s work

1.Tom"s work

  - Navigate to the clones repository "ai-startup-website"

> cd ai-startup-website

  - Check the current branch
  >git branch
 
  - Create a new branch for Tom"s work
   >git checkout -b update-navigation
 
- Open index.html file and add the contents below

> This is Tom adding Navigation to the AI-website

![Tom" branch](image5.png)

  - Check that changes have not been staged 
  >git status

![Tom's](image6.png)

- Stage Tom's changes
>git add index.html

- Confirm changes have been staged for commit
>git status

- Commit Tom/s changes 
>git commit -m "Udate Navigation bar"

- Push Tom's branch to Github remote
>git push origin update-navigation


![Tom"s commitand push](image7.png)



2. Jerry's work
  - Switch to main branch
  >git checkout main

  - Pull the latest changes
  >git pull origin update-navigation

  ![jerry's pull request](image8.png)

- Create new branch for Jerry's work
>git checkout -b add-contact-info

- Open index.html and contact information
- Stage Jerry's changes 
>git add index.html

- Commit jerry's changes
>git commit -m "Add contact information"

- Push Jerry's changes to Github
>git push origin add-contact-info

![jerry's commit](image9.png)
