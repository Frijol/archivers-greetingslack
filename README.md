# Greetings Slackers
This simple script written in basic Python will allow you to hook into the real time API of Slack and perform a greeting to every new joiner!
Usually this is used to tell new joiners about the network, the guidelines, rules, useful links etc etc

If you like this project and you use it for your community or anything else, please hit the STAR button ⭐️ on the top right side so I know you dig it! It makes me feel appreciated and it's free.

## About this Fork

This fork was created for the following reasons:

  * Use a hardcoded welcome message in code, as opposed to an
    environment variable.
  * Add the python `logging` module.
  * Bump the `websocket-client` package version to avoid a bug.
  * Add the ability to debug via a special channel that sends
    welcome message when joined.

**Important:** This branch, `develop/archivers`, auto-deploys to Heroku.
We recommend submitting changes to this branch via pull request.

# Requirements
Python 2.7+
Edit `bot.py` on lines 7-8 to customise with your greeting and token

# Installation
```bash
git clone <thisgitrepo>
cd <thisgitrepo>
virtualenv greetingslack
. greetingslack/bin/activate
pip install requests
pip install websocket-client
python bot.py &
```

# Debugging

If you create a channel named `#greetingslack`, then the bot will send
you a message every time you join it.

# Heroku
Deploy with a click supported now

[![Deploy](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

🔥 **DONT FORGET TO SCALE YOUR FREE DYNO**
