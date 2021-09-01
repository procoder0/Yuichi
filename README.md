# Yuichi

<p align="center">
  <img src="./resources/extras/logo_readme.jpg" alt="TeamYuichi Logo">
</p>
<h1 align="center">
  <b>Yuichi - UserBot</b>
</h1>

<b>A stable pluggable Telegram userbot + vc music bot, based on Telethon.</b>   

[![Stars](https://img.shields.io/github/stars/TeamYuichi/Yuichi?style=flat-square&color=yellow)](https://github.com/TeamYuichi/Yuichi/stargazers)
[![Forks](https://img.shields.io/github/forks/TeamYuichi/Yuichi?style=flat-square&color=orange)](https://github.com/TeamYuichi/Yuichi/fork)
[![Size](https://img.shields.io/github/repo-size/TeamYuichi/Yuichi?style=flat-square&color=green)](https://github.com/TeamYuichi/Yuichi/)   
[![Python](https://img.shields.io/badge/Python-v3.9-blue)](https://www.python.org/)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/TeamYuichi/Yuichi/graphs/commit-activity)
[![Docker Pulls](https://img.shields.io/docker/pulls/programmingerror/Yuichi?style=flat-square)](https://img.shields.io/docker/pulls/programmingerror/Yuichi?style=flat-square)
[![Open Source Love svg2](https://badges.frapsoft.com/os/v2/open-source.svg?v=103)](https://github.com/TeamYuichi/Yuichi)   
[![Contributors](https://img.shields.io/github/contributors/TeamYuichi/Yuichi?style=flat-square&color=green)](https://github.com/TeamYuichi/Yuichi/graphs/contributors)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com)
[![License](https://img.shields.io/badge/License-AGPL-blue)](https://github.com/TeamYuichi/Yuichi/blob/main/LICENSE)
[![Sparkline](https://stars.medv.io/TeamYuichi/Yuichi.svg)](https://stars.medv.io/TeamYuichi/Yuichi)

----

# Deploy
- [Heroku](#Deploy-to-Heroku)
- [Local Machine](#Deploy-Locally)
- [Railway](#Deploy-to-Railway)

# Documentation 
[![Documentation](https://img.shields.io/badge/Documentation-Yuichi-blue)](http://Yuichi.tech/)

# Tutorial 
- Full Tutorial - [![Full Tutorial](https://img.shields.io/badge/Watch%20Now-blue)](https://www.youtube.com/watch?v=9wF7k9qA0Q4)

- Tutorial to get Redis URL and password - [here.](./resources/extras/redistut.md)
---

## Deploy to Heroku
Get the [Necessary Variables](#Necessary-Variables) and then click the button below!  

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://dashboard.heroku.com/new?button-url=https%3A%2F%2Fgithub.com%2FNew-dev0%2FTraveliTg&template=https%3A%2F%2Fgithub.com%2FNew-dev0%2FTraveliTg)

## Deploy to Railway
Get the [Necessary Variables](#Necessary-Variables) and then click the button below!  

[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/new/template?template=https%3A%2F%2Fgithub.com%2FTeamYuichi%2FYuichi%2Ftree%2Fmain&plugins=redis&envs=SESSION%2CAPI_ID%2CAPI_HASH&optionalEnvs=API_ID%2CAPI_HASH&SESSIONDesc=Your+telethon+session+string.&API_IDDesc=api_id%2C+from+my.telegram.org&API_HASHDesc=api_hash%2C+from+my.telegram.org)

## Deploy Locally
- [Traditional Method](#local-deploy---traditional-method)
- [Easy Method](#local-deploy---easy-method)
- [Latest Method](#local-deploy---latest-method)


### Local Deploy - Latest Method
This is the latest and most fastest method currently.<br>
First, goto [This Project](https://github.com/BLUE-DEVIL1134/YuichiCli) and install the latest release from the Github Releases.<br>
Then, do as its given in the `README.md` to add the executable to your system path.

Further, take a look at the [`docs`](https://blue-devil1134.github.io/YuichiCli/) to get more information on this.


### Local Deploy - Easy Method
- Linux - `bash -c "$(curl -fsSL https://git.io/JY9UM)"`
- Windows - `cd desktop ; wget https://git.io/JY9UM -o locals.py ; python locals.py`
- Termux - `sh -c "$(curl -fsSL https://git.io/JY9UM)"`

### Local Deploy - Traditional Method
- Get your [Necessary Variables](#Necessary-Variables)
- Clone the repository: <br />
`git clone https://github.com/TeamYuichi/Yuichi.git`
- Go to the cloned folder: <br />
`cd Yuichi`
- Create a virtual env:   <br />
`virtualenv -p /usr/bin/python3 venv`
`. ./venv/bin/activate`
- Install the requirements:   <br />
`pip(3) install -U -r requirements.txt`
- Generate your `SESSION`:
  - For Linux users:
    `bash sessiongen`
     or
    `bash -c "$(curl -fsSL https://git.io/JY9JI)"`
  - For Termux users:
    `sh -c "$(curl -fsSL https://git.io/JqgsR)"`
  - For Windows Users:
    `cd desktop ; wget https://git.io/JY9JI -o Yuichi.py ; python Yuichi.py`
- Fill your details in a `.env` file, as given in [`.env.sample`](https://github.com/TeamYuichi/Yuichi/blob/main/.env.sample).
(You can either edit and rename the file or make a new file named `.env`.)
- Run the bot:
  - Linux Users:
   `bash resources/startup/startup.sh`
  - Windows Users:
    `python(3) -m pyYuichi`

## Necessary Variables
- `API_ID` - Your API_ID from [my.telegram.org](https://my.telegram.org/)
- `API_HASH` - Your API_HASH from [my.telegram.org](https://my.telegram.org/)
- `SESSION` - SessionString for your accounts login session. Get it from [here](#Session-String)
- `REDIS_URI` - Redis endpoint URL, from [redislabs](http://redislabs.com/), tutorial [here.](./resources/extras/redistut.md)
- `REDIS_PASSWORD ` - Redis endpoint Password, from [redislabs](http://redislabs.com/), tutorial [here.](./resources/extras/redistut.md)

## Session String
Different ways to get your `SESSION`:
* [![Run on Repl.it](https://replit.com/badge/github/TeamYuichi/Yuichi)](https://replit.com/@TeamYuichi/YuichiStringSession)
* Linux : `bash -c "$(curl -fsSL https://git.io/JY9JI)"`
* PowerShell : `cd desktop ; wget https://git.io/JY9JI ; python Yuichi.py`
* Termux : `sh -c "$(curl -fsSL https://da.gd/termux-tel)"`
* TelegramBot : [@SessionGeneratorBot](https://t.me/SessionGeneratorBot)

Made with 💕 by [@TeamYuichi](https://t.me/TeamYuichi). <br />

# License
Yuichi is licensed under [GNU Affero General Public License](https://www.gnu.org/licenses/agpl-3.0.en.html) v3 or later.

[![License](https://www.gnu.org/graphics/agplv3-155x51.png)](LICENSE)

# Credits
* [![TeamYuichi-Devs](https://img.shields.io/static/v1?label=TeamYuichi&message=devs&color=critical)](https://t.me/YuichiDevs)
* [Lonami](https://github.com/LonamiWebs/) for [Telethon.](https://github.com/LonamiWebs/Telethon)
* [Dan](https://github.com/delivrance) for [Pyrogram.](https://github.com/pyrogram/pyrogram)
* [Pytgcalls](https://github.com/pytgcalls) for [PyTgCalls.](https://github.com/pytgcalls/pytgcalls)
