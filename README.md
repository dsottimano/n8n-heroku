# n8n heroku deployment for MozCon

This is a fork of the original repository from Sarveshwarge https://github.com/sarveshwarge/n8n-heroku

Changes:
- Use version 0.70
- Added additional config vars for Heroku

## Steps

1. Open up a free account with https://heroku.com and click the deploy button below.

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/dsottimano/n8n-heroku)

2. Get a PageSpeed Insights API key

3. Set up Stitchdata.com with Bigquery and a Webhook integration. You'll need your webhook URL

4. Copy the code from this page to your clipboard, login to your new Heroku n8n app and paste it into a workflow. Next, add in your PageSpeed API Key and Stitchdata webhook URL

5. Save the workflow and set it to active (top right of the workflow)

6. Create a new workflow with a webhook trigger, get the webhook URL and create a cron job to ping it every 15 minutes to prevent the Heroku hobby app from sleeping.


### Sources

https://github.com/n8n-io/n8n
https://github.com/sarveshwarge/n8n-heroku
