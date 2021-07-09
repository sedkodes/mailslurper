## Run a local SMTP Server

#### Prerequisites
- Docker
- Python (to test email)


1. Run the MailSlurper server
```
$ docker run -it -p 2500:2500 -p 8080:8080 -p 8085:8085 --rm marcopas/docker-mailslurper
```

You're done.  Navigate to `http://localhost:8085` to see your inbox!


2. Test the SMTP Server:

If you've cloned the repo:
```
$ python send-mail-test.py
```

or just paste the command into your terminal to run the script from CLI:
```

```

and then check the repo
