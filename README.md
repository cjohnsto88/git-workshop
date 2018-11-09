# GitHub Workshop Conversation
The GitHub workshop conversation is intended to give students a no distractions insight into using `git` to collaborate and share contributions to a project. Two people are required to demonstrate `git add`, `git commit`, `git push` and `git pull` by have a simple conversation through a text file.

## Conducting the Conversation
The best way to conduct the conversation is via a single laptop, but with 2 terminals side by side. The terminal on the left being participant A's "computer" and the right terminal being participant B's "computer". You will also need a browser with a tab open at the git repo to be used for the demo. Start with an **empty** git repo hosted on GitHub.

### Cloning, adding, committing and pushing
1. Participant A clones the repo. Remember to `cd` into the directory where the empty repository has been cloned!
2. Participant A creates a text file called `conversation.txt` and adds "Hi"
3. Participant A runs `git status` to show that git sees the conversation.txt file and is informing the user that they should run `git add` in order to stage the file
4. Participant A runs `git add .` followed by `git status` to show that the file is now in the staging area
5. Participant A runs `git commit -m <MESSAGE>` in order to commit the file
6. Participant A runs `git status` to show that we are now back to a clean state
7. Participant A goes to the project in GitHub in their browser and shows that the file is still not there in GitHub
8. Participant A runs `git push` in order to push master to GitHub
9. Participant A refreshed the GitHUb project in their browser and shows that the file is there and has the content expected

### Cloning, adding, committing and pushing II (Participant B)
1. Participant B clones the repo
2. Participant B adds "Hi, how are you?" to `conversation.txt`
3. Participant B does `git add .`, `git commit -m <MESSAGE>`, optionally running `git status` between each `git` command
4. Participant B highlights that the file in GitHub does not yet have the changes that we made locally
5. Participant B runs `git push` and shows that the file on GitHub now has the changes

### Pulling
1. Participant A shows that they don't have the changes made to `conversation.txt` by participant B
2. Participant A Run `git pull` and open `conversation.txt`. We now have participant B's contribution
3. Participant A Add the text "I'm good thanks"
4. Participant A runs `git add .`, `git commit -m <MESSAGE>` and `git push`

### Simple response
1. Participant B runs `git pull` to get latest contributions
2. Participant B adds "How was dinner?" to `conversation.txt`
3. Participant B runs `git add .`, `git commit -m <MESSAGE` and  `git push`

### Respond about dinner, **but DO NOT push!!!**
1. Participant A runs `git pull` to get latest contributions
2. Participant A adds "Fantastic" to `conversation.txt`
3. Participant A runs ONLY `git add .` and `git commit -m <MESSAGE>`. DO NOT RUN `git push`!!!

### Interruption, GitHub has stuff you don't
1. Participant B is a rather pedantic soul and is frustrated that this conversation doesn't have a title. How horrendously awful... Add "CONVERSATION" as a new line **AT THE TOP** of the file
2. Participant B runs `git add .`, `git commit -m <MESSAGE>` and `git push`

### GitHub has stuff we don't, let's pull
1. Participant A now tries to push their `conversation.txt` commit. It won't push and suggests that you run `git pull`
2. Participant A runs `git pull`
3. Participant A shows that their `conversation.txt` now has the title added by Participant B
4. Participant A runs `git push` and shows in GitHub that all the changes are now safley there

### Set up for conflict. Brace yourself!!! **Do NOT push!!!**
1. Participant B runs `git pull`
2. Participant B adds "Hey do you have any pets?" to  **AS THE LAST LINE** in `conversation.txt`
3. Participant B runs `git add .`, `git commit -m <MESSAGE>` but does NOT run `git push`

### Creating conflict
1. Participant A adds "Hey, do you have any pets?" **AS THE LAST LINE** in `conversation.txt`
2. Participant A runs `git add .`, `git commit -m <MESSAGE>` and `git push`
3. Participant A runs `git pull`. There's a conflict. Highlight to students that are unfamiliar with git that it may be best to ask for some help from an SME if this occurs
