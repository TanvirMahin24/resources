# You may face some issues while hosting React.js project to Netlify as the react Router do not work.

## To solve this issue you can use the following steps:
- Make a file called "_redirects" in the public folder of your project.
- Copy the following code to the file: 
  
  `/*    /index.html   200 `
- Then build the project and host the site.