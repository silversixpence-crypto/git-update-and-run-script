# Overview

This script it used to startup a Node server and check for updates every 5 minutes.

# Getting started

- Setup SSH keys for access to your Github repo
- From `/home` run the following to clone your source repo to `/home/node-source`:

```bash
git clone git@github.com:silversixpence-crypto/node-source.git
```

- Download `git-update-and-run.sh` to `/home`

```
wget https://github.com/silversixpence-crypto/git-update-and-run-script/raw/main/git-update-and-run.sh
```

- Make it executable

```
chmod +x git-update-and-run.sh
```

- Run it

```
./git-update-and-run.sh
```

# Additional

Automatically start this script with crontab and run it inside `screen` to keep it running without a terminal open.

```
@reboot screen -dmS node /home/git-update-and-run.sh
```
