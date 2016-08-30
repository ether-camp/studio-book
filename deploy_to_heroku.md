# Deploying to Heroku*

Heroku is a well known PaaS (Platform as a Service) site with free access to [deploy your Apps](https://devcenter.heroku.com/articles/getting-started-with-nodejs#prepare-the-app). It is scalable and reasonable in cost for small projects. Read Heroku's [excellent documentation and tutorials](https://devcenter.heroku.com/articles/deploying-nodejs#prerequisites). The isntructions here are for conventional Apps -not Ethereum Dapps*.  You will need a github account if you don't have one. Set a IDE project folder as master with a repository on github. Then when ready, sign-up to a free Heroku account.

A typical Heroku deploy sequence from the terminal:

```git remote add origin https://github.com/[USER_NAME]/[PROJECT_FOLDER]             

npm init --yes

git add --all

git commit -am "improved something"

git push heroku master

heroku ps:scale web=1

heroku open```

*It is beyond the scope of this document to explain git version control, Heroku's api extensions, procfile, Web3 , accessing and/or setting up a node server outside the IDE. Visit the slack channel if you have questions.