# sdsrs-anki-server
Anki server backend for [austin226/sdsrs](https://github.com/austin226/sdsrs)

Dependencies:
* [AnkiServer](https://github.com/dsnopek/anki-sync-server)
* [Anki](https://apps.ankiweb.net/)

# Setup Instructions
```bash
sudo ./setup
```

This will download and install the required dependencies, AnkiServer and Anki itself.
This will also create a config file at `config/server-config.ini`
The prompt will ask you for an IP address and a server port. These will
be saved to `config/env.ini`. You can also create this file yourself, and it will
read the values from there. Follow `config/env.ini.example` for an example.

# Running the server
Follow the [AnkiServer instructions](https://github.com/dsnopek/anki-sync-server#configuring-and-running-your-anki-server):

```bash
$ ./ankiserverctl.py adduser <username>
$ ./ankiserverctl.py debug
$ ./ankiserverctl.py start
$ ./ankiserverctl.py stop
```
