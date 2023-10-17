
hello this is CTFd platform with discord webhook plugin i customize 
the FirstBlood send to discord webhook and the notification send to discord webhook

U can use this for your CTFd platform work in windows and linux

## Install

1. Install dependencies: `pip install -r requirements.txt` dont forget to install weebhook `pip install discord-webhook`
   or `python3 -m pip install -r requirements.txt`
   1. You can also use the `prepare.sh` script to install system dependencies using apt.
2. Modify [CTFd/config.ini](https://github.com/CTFd/CTFd/blob/master/CTFd/config.ini) to your liking.
      if you lazy u can just run `python serve.py` or `flask run` to run the server with default configuration.
3. Use `python serve.py` or `flask run` in a terminal to drop into debug mode.

You can use the auto-generated Docker images with the following command:

`docker run -p 8000:8000 -it ctfd/ctfd`

Or you can use Docker Compose with the following command from the source repository:

`docker-compose up`

Check out the [CTFd docs](https://docs.ctfd.io/) for [deployment options](https://docs.ctfd.io/docs/deployment/installation) and the [Getting Started](https://docs.ctfd.io/tutorials/getting-started/) guide

## Live Demo

https://demo.ctfd.io/

## Discord Webhook

1. Create a New Webhook in your Discord Server Settings

![wada](https://iili.io/JF7dlee.png)

2. Go to Folder CTFd-master/CTFd/plugins/ctfd_discord_webhook_plugin

3. Open File config.py

4. Change the value of the variable "WEBHOOK_URL" to the Webhook URL that you created in your Discord Server Settings

![adwa](https://iili.io/JF73sxs.png)

5. If you want to change the message that will be sent to your Discord Server, you can change the value in config.py

6. Or you can change the message in the file "webhook.py" in the folder CTFd-master/CTFd/plugins/ctfd_discord_webhook_plugin

7. Preview

![wad](https://iili.io/JF7OmoQ.png)


## Source Code/ Repository

- https://github.com/sigpwny/ctfd-discord-webhook-plugin
- https://github.com/CTFd/CTFd