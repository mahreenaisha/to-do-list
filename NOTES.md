# Notes

Created the GitHub repo without README.md, license file, and .gitignore because the local repo already has git configured. It is done when creating the Angular application.

## Commands to Create the Application
`node -v`  
`npm -v`  
`npm install @angular/cli`  
`ng new to-do-list`  
`ng version`  
`cd to-do-list`    

## Git Commands  
`git remote add origin https://github.com/mahreenaisha/to-do-list.git`    
`remote`: relates to the online repo hosted by GitHub  
`add`: creates a link  
`origin`: name of the remote repo  
the URL: where the remote repo actually lives  

`git branch -M main`  
`-M`: this flag forcefully renames the current branch even if there is a naming conflict  
`main`: new name of the current branch  

`git push -u origin main`  
`-u`: this flag sets a **tracking relationship** between the local main branch and the remote's main branch  
`origin`: the remote repo  
`main`: which branch to push  

