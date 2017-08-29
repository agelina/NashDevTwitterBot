# NashDev Twitter Bot

Automate posting events from cal.nashvl.org to Twitter

## Proposed Solution
![overview](https://user-images.githubusercontent.com/501822/27800820-96c16a6e-5fe0-11e7-919d-b7786bd35471.png)

## ToDo
* [X] Get a Github Repo
* [X] Write a readme
* [X] Answer Questions
* [X] Scope work
* [X] Add scoped work to ToDo
* [ ] Write docs
* [ ] Write tests
* [ ] Implement
  * [X] Parse Feed
  * [X] Define Structure
  * [X] Filter listings
  * [ ] Truncate for Twitter
  * [X] Authorize via Tweepy
  * [X] Tweet via Tweepy

## Installation on Heroku
> Prerequisites: Twitter and Heroku Accounts, Heroku CLI is installed, you are logged into Heroku via Heroku CLI

### Create Twitter App
1. Visit [https://apps.twitter.com](https://apps.twitter.com)
2. Login
3. Create a new app
4. Within your app visit the "Keys and Access Tokens" tab
5. Generate your access token and access token secret
6. Leave the page open, you will need it later

### Push to Heroku
1. Pull down nashDevTwitterBot
2. cd into nashDevTwitterBot
3. Ensure nashDevTwitterBot is initialized as a git repo. If not run `git init` within nashDevTwitterBot
4. Login into Heroku via a browser and create a new app
5. Add a git remote for the Heroku app within nashDevTwitterBot **Example:** `heroku git:remote -a nash-dev-twitter-bot`
6. Push source to Heroku `git push heroku master`
7. Visit your Heroku App's "Settings" tab
8. Locate the section "Config Variables"
9. Add config variables for CONSUMER_KEY, CONSUMER_SECRET, ACCESS_TOKEN, and ACCESS_TOKEN_SECRET. The values of these variables should be copied from the Twitter page you left open in step 6 of "Create Twitter App"
