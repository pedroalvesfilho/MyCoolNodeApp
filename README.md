### Heroku
#### How to deploy a NodeJS app to Heroku from 

	Github (without installing Heroku on your machine)
https://medium.freecodecamp.org/how-to-deploy-a-nodejs-app-to-heroku-from-github-without-installing-heroku-on-your-machine-433bec770efe


--

We recommend every repository include a README, LICENSE, and .gitignore.

```
... or create a new repository on the command line
echo "# MyCoolNodeApp" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/pedroalvesfilho/MyCoolNodeApp.git
git push -u origin master
…or push an existing repository from the command line
git remote add origin https://github.com/pedroalvesfilho/MyCoolNodeApp.git
git push -u origin master
…or import code from another repository
You can initialize this repository with code from a Subversion, Mercurial, or TFS project.
```

---


https://elements.heroku.com/buildpacks/heroku/heroku-buildpack-nodejs

```
Hacking
To make changes to this buildpack, fork it on GitHub. Push up changes to your fork, then create a new Heroku app to test it, or configure an existing app to use your buildpack:

# Create a new Heroku app that uses your buildpack
heroku create --buildpack <your-github-url>

# Configure an existing Heroku app to use your buildpack
heroku buildpacks:set <your-github-url>

# You can also use a git branch!
heroku buildpacks:set <your-github-url>#your-branch

```


```
CLI Installation
  
  
heroku create --buildpack https://github.com/heroku/heroku-buildpack-nodejs.git
```
