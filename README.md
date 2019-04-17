![Logo](docs/meteor-desktop.png)

# Meteor Desktop
###### aka Meteor Electron Desktop Client
> Build desktop apps with Meteor & Electron with full stack bundling.

## What is this?

This is a try to implemnt the full stack bundling in [Meteor Desktop](https://github.com/wojtkowiak/meteor-desktop).

The final result is have working a complete Meteor server in the local electron app.

### Quick start

```bash
 cd /your/meteor/app

 # 1. Install meteor-destop
 meteor npm install --save-dev @kaptux/meteor-desktop

 # 2. Add a `desktop` script in npm scripts that equals to "meteor-desktop".
 Usage: npm run desktop -- [command] [options]

 # 3. Scaffolds .desktop dir in your metoer app
 npm run desktop -- init
 # Check the .desktop/settings.json and now you'll see a new key "serverEnv" where you can set the environment variables for your local meteor server.

# 4. Dev build
npm run desktop -- build --full-stack
# This takes de Meteor app bundle from .meteor/local/build/programs

# 5. Production build
npm run desktop -- build --full-stack --production
# Builds the Meteor app bundle with "meteor buid".

# 6. Run local build
npm run desktop -- just-run
# When run a production build the first step is try to download the correct node version (arch + platform) to run the local meteor server. 

# 7. Build the installer
npm run desktop -- build-installer --full-stack --production

```

## TODOS

- [X] Check win installer
- [X] Check macOs installer
- [] Check linux installer
- [] Check autoupadate.
- [] Improve the feedbak in the splash screen. (download node version, starting local server, ...)

