# discordia

**discordia** is a basic python wrapper for discord's rest api (bot token only).  
it lets you interact with discord as a bot without needing a gateway connection—just use http requests.

---

## features

- get bot, user, server, and channel info
- list server channels and members
- send, edit, and delete messages
- add reactions to messages

---

## installation

install from pypi:

```sh
pip install discordia
```

or, for development, clone the repo and install dependencies:

```sh
pip install -r requirements.txt
```

---

## usage

```python
from discordia_client import discordia

token = ""
client = discordia(bot_token)

# get info about the bot user
print(client.get_me())

# send a message
channel_id = ""
client.send_message(channel_id, "hi from discordia")
```

---

## requirements

- python 3.7+
- `requests` library

---

## project structure

- `discordia_client.py` – main api wrapper
- `discordia_init.py` – version and imports
- `pyproject.toml` – build system
- `setup.cfg` – package metadata/configuration
- `readme.md` – this file
- `license` – license

---

## license

[mit](license)

---