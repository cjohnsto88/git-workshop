# GitHub Workshop Conversation
The GitHub workshop conversation is intended to give participants a no distractions insight into using git to colaborate and share contributions to a project. Two people are required to demonstrate git add, commit, push and pull by have a simple conversation through a text file.

l. Participant A clones the repo. Remember to `cd` into the directory where the empty repository has been cloned!
l. Participant A creates a text file called conversation.txt and adds "Hi"
l. Participant A runs `git status` to show that git sees the conversation.txt file and is informing the user that they should run `git add` in order to stage the file
l. Participant A runs `git add .` followed by `git status` to show that the file is now in the staging area
l. Participant A runs `git commit -m <MESSAGE>` in order to commit the file
l. Participant A runs `git status` to show that we are now back to a clean state
l. Participant A goes to the project in GitHub in their browser and shows that the file is still not there in GitHub
l. Participant A runs `git push` in order to push master to GitHub

