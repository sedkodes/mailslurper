## Run a local SMTP Server

#### Prerequisites
- [Docker](https://docs.docker.com/get-docker/)
- Python, optional(to test email)


### 1. Run the MailSlurper server
```
$ docker run -it -p 2500:2500 -p 8080:8080 -p 8085:8085 --rm marcopas/docker-mailslurper
```

You're done.  Navigate to `http://localhost:8080` to see your inbox!


### 2. Test the SMTP Server:

Paste the command into your terminal to run the email script, Python needs to be installed.
```
$ wget -qO- https://raw.githubusercontent.com/sedkodes/mailslurper/main/send-mail-test.py | python
```

and then refresh your inbox at `http://localhost:8080` to see your email!
