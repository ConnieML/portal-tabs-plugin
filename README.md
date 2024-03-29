<a  href="https://www.connieconnect.com">
<img  src="https://i.postimg.cc/MGd7M6Cp/connie-logo-white-thin-deja-Vu-Sans.png"  alt="Connie SaaS For Nonprofits"  width="250"  />
</a>

# Agent Desktop Portal Tabs Plugin
This repository is the plugin source code that powers the Agent Desktop Portal Tabs. The portal tabs make the data portal section of the agent's desktop exponentially more useful by allowing agents to have one-click access to the tools they need to answer questions and deliver CBO services. Additionally, the tabs are responsive based on the task attribues and variable that get passed when the agent accepts a new task. 

Twilio Flex Plugins allow you to customize the appearance and behavior of [Twilio Flex](https://www.twilio.com/flex). If you want to learn more about the capabilities and how to use the API, check out our [Flex documentation](https://www.twilio.com/docs/flex).

## Setup

Make sure you have [Node.js](https://nodejs.org) as well as [`npm`](https://npmjs.com) installed.

Afterwards, install the dependencies by running `npm install`:

```bash
git clone git@github.com:cweems/plugin-emergency-contact-center.git
cd plugin-emergency-contact-center

# If you use npm
npm install
```

## Development

In order to develop locally, you can use the Webpack Dev Server by running:

```bash
npm start
```

This will automatically start up the Webpack Dev Server and open the browser for you. Your app will run on `http://localhost:8080`. If you want to change that you can do this by setting the `PORT` environment variable:

```bash
PORT=3000 npm start
```

When you make changes to your code, the browser window will be automatically refreshed.

## Deploy

Once you are happy with your plugin, you have to bundle it in order to deploy it to Twilio Flex.

Run the following command to start the bundling:

```bash
npm run build
```

Afterwards, you'll find in your project a `build/` folder that contains a file with the name of your plugin project. For example, `plugin-example.js`. Take this file and upload it into the Assets part of your Twilio Runtime.

Note: Common packages like `React`, `ReactDOM`, `Redux` and `ReactRedux` are not bundled with the build because they are treated as external dependencies so the plugin will depend on Flex to provide them globally.
