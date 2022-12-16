# *Read: 03 - Revisions and the Cloud*

## **Open a GitHub Project into VSCODE**

     - Open up terminal
     - Enter ls into terminal
     - You should see a list of folders
     - Type cd and the folder that you cloned your .md file too (in my case it is projects)
     - Enter ls again so you can see where you are in terminal
     - Enter cd 102
     - Enter ls once again
     - Enter cd reading-notes (or whatever you named your .md file)
     - You should see: reading-notes git:(main)
     - Enter code .
     - If you followed every step VSCODE should open with no issues

## **Cloning from VSCODE to GitHub**

     - After your done making you changes in VSCode you'll want to clone this back to GitHub.
     - If you kept your terminal open reading-notes git: (main) still be there.
     - Enter git status after reading-notes git: (main)
     - It should show Changes not staged for commit
     - Enter git add .
     - Enter git status to see if the files you updated turned green.
     - If it did enter git commit -m "what changes you made"
     - Next you enter git push origin main (you may have to this once or twice)
     - If you did everything right your GitHub link to the sight should reflect these changes you made to your .md file
