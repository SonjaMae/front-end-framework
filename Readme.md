# Basic Framework For Front End Vanilla.js Projects

## Preflight Check
1. Check you're in the project file by using the current working directory command
```
  pwd
```
2. Initialize your project
```
  npm init
```
3. Run npm install from the framework root folder. This will create the node_modules and install the dependancies found in the package.json file.
```bash
  npm install 
  npm install -D http-server parcel 
```
4. Run development build using the parcel bundler.
```bash
   npx parcel src/index.html
```
or
```
  npm start
```
5. Run production build using the parcel bundler.
```bash
   npx parcel build src/index.html
```
or
```
  npm run build
```


## Git Setup
1.  .gitignore ignores files and they will not be uploaded to your remote repository

2.  Set up repo from VS Code
   -  user profile icon (Accounts)
   -  sign in to sync settings
   -  sign in with GitHub
   -  click green button to accept
   -  enter the Source Control tab on VS Code
   -  publish to GitHub public repository


## Remove Repo
1.  go to the GitHub repo's page
2.  select its Settings tab
3.  scroll to the bottom (Danger Zone)
4.  delete the repository


## If You Make An Init Mistake
1.  search your local repository for hidden files
```bash
  ls -lah (on mac)
  ? (on windows powershell)
```
2.  look for a file titled
```
  .git
```
3.  remove the .git file by typing
```
  rm -rf .git
```
4.  then re-init your repository


## Deploying to Netlify
1.  create a Netlify account linked to GitHub
2.  select the Sites tab
3.  click the New Site From Git button
4.  click GitHub and choose which repo to build
5.  write the correct git command, in this case
```bash
  npx parcel build src/index.html
```
6.  Netlify will deploy your repo automatically