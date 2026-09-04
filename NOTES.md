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

## Angular Commands  
`ng serve`: builds the application and hosts on localhost  
`ng generate component todo`: creates a component called "todo"  
`ng generate service todo`

---
Everything is an Angular application is made up of components. Each component has a TypeScript file for data and logic, an HTML file for template or DOM (idk how to be technically correct), and a CSS file for styling.  
`app.ts` is the main component. It is responsible for displaying all the other components.  
In my code, the component has files like app.ts, app.html, and app.css. Whereas on the internet, they are mentioned as app.component.ts, app.component.html, and app.component.ts. I will figure out why later. Probably because of different Angular versions.  

Added the todo component by using its selector (app-todo) in app.html. Selectors in Angular alway start with "app" to not confuse with the HTML tags.  

AI INLINE SUGGESTIONS ARE SO ANNOYING.  
Add `"chat.disableAIFeatures": true` in settings.json in VSCode.  

*Service* is just another feature of Angular like component. It shares data between components. It is a reusable piece of code. It handles data fetching. Multiple components can use it.

Why are we using a service here? On top of my head, I'm gonna say, it is used to fetch data from the database. In this case, the data would be a single task of 'string' type.  

We are gonna store our data in JSON format in a file in the repo for the time being instead of using a database. This data will be served to us from this API endpoint `https://jsonplaceholder.typicode.com/todos`. This is a private endpoint. Mentioned in `todo.ts` (service).  (didnt add the url yet)

---  
### Goal 1: Fetch and display items


