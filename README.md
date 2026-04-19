# SLACK - N8N Automation

build a bot that describes images dumped in a channel

## N8N import workflow
n8nserver: nivsn8n.com <br>
user: admin@handson-academy.com <br>
pass: Nivsn8n! <br>

get openai token from: https://platform.openai.com/settings/profile/api-keys <br>


Import `workflows/slack-image-desc.json`. In **Download Image** and **Post Back to Slack**, replace the placeholder `YOUR_BOT_USER_OAUTH_TOKEN` in the Authorization header with your Slack Bot User OAuth token (after `Bearer `). In **OpenAI describe image**, replace `YOUR_OPEN_AI` with your OpenAI API key (after `Bearer `).

## SLACK configuration

### CREATE a workspace

### CREATE app 
goto https://api.slack.com/apps/ and create an app called image-desc

#### Event Subscriptions
https://nivsn8n.com/webhook/slack-image-describe <br>
message.channels  <br>
message.groups    <br>


#### Outh and permissions
channels:history <br>
channels:read    <br>
chat:write       <br>
files:read       <br>
groups:history   <br>
groups:read      <br>


#### Install app
install app                <br>
copy Bot User OAuth Token  <br>

create channel images-desc and invite the app to the channel



