# Telegram VC Player Bot
Play any song directly into your group voice chat.

Official Bot : [TgVCPlayerBot](https://telegram.me/Tgvcplayerbot)   |   Discussion Group : [VoiceChat Music Player Support](https://telegram.me/Pyar_China_Ka_Maal_Hai)

<p align="center">
  <img width="200" height="200" src="https://telegra.ph/file/036b04ee24ca3965dd51b.jpg">
</p>

[Checkout AutoForwarder Bot](https://sktechhub.com/auto-forward)


# Requirements
1. Telegram Api Id and Hash [ Get it from my.telegram.org ]
2. A Telegram Bot Token. Get it from @botfather.
3. Python 3.6+
4. ffmpeg [ [How to Install ? ](https://linuxize.com/post/how-to-install-ffmpeg-on-ubuntu-18-04/) ]

# Deploying To Heroku
1. Get your telegram API ID and API HASH from my.telegram.org and the BOT TOKEN from @botfather.
2. Generate your telegram session string using the `Run on Repl` button below (Click on run after opening the url below) or use the `generateSession.py` file.

- [![Run on Repl.it](https://repl.it/badge/github/kshubham506/vcplayerbot)](https://replit.com/@kshubham506/GenerateSession?lite=1&outputonly=1)


3. Clcik on the `Deploy to Heroku` button below. Fill in the required fields on the website that opens.

- [![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

- [![Deploy+To+Railway](https://railway.app/button.svg)](https://railway.app/new/template?template=https://github.com/mrnitric/tgvcplayerbot&envs=SESSION_NAME,BOT_TOKEN,BOT_NAME,API_ID,API_HASH,SUDO_USERS,DURATION_LIMIT)

4. Add the bot to your group and send the [commands](https://github.com/rishabhanand2/lucymusic_bot#features) to start using the VCPlayer Bot :)


# Steps To Setup
1. Install pyrogram for generatong session string : `pip3 install -U pyrogram`
2. Generate your telegram session string. Run `python3 generateSession.py`
3. Rename `.env copy` to `.env` and fill all the required/mandatory fields in there.

# Steps to Run
1. After the setup is done.
2. Install ffmpeg : `sudo apt-get install ffmpeg`
3. Install the requirements : `pip3 install -U -r requirements.txt`
4. Run the service by : 
  - Run `python3 main.py --help` for available settings.  
  - Or Run `python3 main.py -env prod` to use default settings

# Environmental Variables

Starting from command line:
- python3 main.py -env `prod|local` -mode `single|multiple` -autoleave `on|off`

Available env varibales
- `Mandataory` **SESSION_NAME** :  Pyrogram session string.
- `Mandataory` **BOT_TOKEN** : A bot token from @BotFather.
- `Mandataory` **BOT_NAME** : Your MusicPlayer Bot Name.
- `Mandataory` **API_ID** : App ID from my.telegram.org/apps.
- `Optional` **API_HASH** : App hash from my.telegram.org/apps.
- `Optional` **SUDO_USERS** : List of user IDs counted as admin everywhere (separated by space).
- `Optional` **DURATION_LIMIT** : Max audio duration limit for downloads (minutes).

# Features
Command | Description
------------ | -------------
/start , /help | Lists the available commands.
/play song_name | Starts the song in the voice chat.
/skip | Skips the current song.
/end | End the voice player.

# Developer
[Mr Nitric](https://t.me/its_Nitric)

For any issues/questions please contact [here](https://telegram.me/SankiBots)

Pull Requests are more than welcome.


 ### [A Sanki Product](https://t.me/Sanki_Bots)
