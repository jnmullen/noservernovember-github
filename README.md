
# No Server November Challenge Number 2

See this page [NoServerNovember](https://serverless.com/blog/no-server-november-challenge/)

Third challenge : 

>Automate a GitHub Check with Serverless.
> This project is one of our favorites around the office, for its sheer usability. Automating anything to do with GitHub is just incredibly useful.

> For the easy version, set up a GitHub check that makes sure there’s a reference to a GitHub / Jira / etc issue in the PR title. For the harder version, set up a GitHub check to automatically lint & reformat your code on a new commit.

> Or, do something else fun. We’ll leave this open-ended.

### Prerequisites

To try out this example you will need to install the Serverless Framework for your platform from here : 

[Install Serverless Framework](https://serverless.com/framework/docs/providers/aws/guide/quick-start/)

Assume you have created a file with your AWS credentials in __~./aws/credentials__ as the Serverless Framework will require these to be able to run.

You will need to create a serverless.emv.yml file in with your relevant Twitter API Keys :

```
cat serverless.env.yml
github:
  GITHUB_CONSUMER_KEY: 'KEY HERE'
```

### Running Serverless Framework

Assume you have created a file with your AWS credentials in __~./aws/credentials__ as the Serverless Framework will require these to be able to run.

To get the dependencies installed run:
```
npm install
```
To create the infrastructure run:
```
sls deploy
```
Once you have finished you can destroy the infrastructure with : 
```
sls remove 
```
