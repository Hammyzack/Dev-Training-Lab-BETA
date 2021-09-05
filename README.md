# Dev Lab BETA/486 Story Card 

## User Story (Story Points = med👕) 

**As a** user of your hello-node app

**I want** to use this app online, _on the web_

**So That** I don't have to (a) go to your REPO, (b) download code (c) unzip (d) vsCode project (e) install `node.js` & `express.js` (f) etc. 

## Comments/Discussion
- pretty much same as before...new node app => localhost => github => heroku => persistent URL. 
- use Grammarly 
- Level up your cmd line: `$:` `PS1='shorter-prompt'` (where `'shorter prompt'` is an alias for your cmd prompt)

## Resources
- [zoom class from hurricane day](https://una.zoom.us/rec/share/hdLvEpmjxIi5Ffv4VOp7pMumW8c473fVKLWxyJW_mGz4X83P8M7Gf00kM3cOXCQ.RtMy181jXMG1RScW?startTime=1630431327000) 
- [ghyt repo](https://github.com/barrycumbie/hello-heroku)

## Test/Acceptance Criteria/Rubric (how do you know when you are done) 

- [ ] navigate to a URL: _______ (heroku): 0 | 5 | 10
- [ ] link back to ghyt repo w/target: 0 | 5 | 10
- [ ] file directory and naming, ghty link to herok: 0 | 5 | 10 
- [ ] clear instructions (w/shortcuts), in m/d, on readme to <del>spin up</del> tell about the project, how to build on: 0 | 5 | 10 
- [ ] code quality: logical, readable, functional: 0 | 5 | 10  

## Step-by-Step

- [ ] open **vsCode** 
- [ ] open **terminal** `ctrl+~`
   - [ ] check if **git bash** is default (`ctrl+shift+p` to open **cmd pallete**: "select default..." choose "git bash"
- [ ] navigate to your workspace, e.g.: `cd Desktop`
- [ ] make your **project root diretory**: `mkdir my-super-awesome-project-name`
- [ ] navigate to the new dir/: `cd my-super-awesome-project-name`
- [ ] open up the **project root** in **vsCode**: use the gui...wish I knew the cmd,
   - it's something like: `open -a 'visual studio code' my-super-awesome-project-name`
- [ ] initialize a **Node.js** project: `$:` `npm init -y`
- [ ] install **express.js**: `$:` `install i express --save`
- [ ] create a new file `$:` `touch index.js`
- [ ] open index.js in **vsCode**
   - [ ] create an express server (see the **ghyt repo** for the `source code`)
- [ ] edit `package.json`:
...
"scripts": {
-        "test": "echo \"Error: no test specified\" && exit 1"
+        "test": "echo \"Error: no test specified\" && exit 1",
+       "start": "node index.js"
    },

...
 create a .gitignore file: $: echo 'node_modules' >> .gitignore (//I think that'll do it, could be wrong)
 initialize the local git repo: $: git init
 head over to https://github.com
 sign in (requires an active account)
 create a new repo: name it something like: hello-heroku or node-on-heroku or whatever
 do not check any defaults, just give it a name and create it.
 follow the steps on the next screen to connect this remote repo to your local git repo
 they give you something like this:
echo "# hello-heroku-or-whatever-you-named-it" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/{YOUR-USER-NAME}/{YOUR-REPO-NAME}.git
git push -u origin main
 but might need to make sure we know what we are doing
echo "# hello-heroku-or-whatever-you-named-it" >> README.md
- git init //we already did this
- git add README.md
+ git add . 
☝️ add everything, not just the readme

the rest is 😎, might have to authenticate/login

git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/{YOUR-USER-NAME}/{YOUR-REPO-NAME}.git
git push -u origin main
okay...taking a breather. Pick up here later, Cumbie 🦖 initializing heroku & running it all.
