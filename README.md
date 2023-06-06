# Deploy to HEROKU

**Important Note**
1. Upload all of your private files here: `config.env`, `token.pickle`, `rcl.conf`, `accounts.zip`, `shorteners.txt` etc...

**Mandatory Veriables in Config**

- `UPSTREAM_REPO`: Your github repository link, if your repo is private add `https://<deploy_token>:<empty_password>@gitlab.com/<your_username>/<repository_name>
` format. `Str`.
  - **NOTE**: Don't forget to remove '<' and '>' . Follow [**THIS TUTORIAL**](https://graph.org/GitLab-Upstream-Tutorial-06-02) to generate upstream repo. 
              - Any change in docker or requirements you need to deploy/build again with updated repo to take effect. 
              - **DON'T delete .gitignore file**. For more information read [THIS](https://github.com/NadifMasamba/CMT-Hero#upstream-repo-recommended).
- `UPSTREAM_BRANCH`: Upstream branch for update. Default is `zh_run`. `Str`

- `BOT_TOKEN`: The Telegram Bot Token that you got from [BotFather](https://t.me/BotFather). `Str`
- `OWNER_ID`: The Telegram User ID (not username) of the Owner of the bot. `Int`
- `TELEGRAM_API`: This is to authenticate your Telegram account for downloading Telegram files. You can get this from <https://my.telegram.org>. `Int`
- `TELEGRAM_HASH`: This is to authenticate your Telegram account for downloading Telegram files. You can get this from <https://my.telegram.org>. `Str`

- `BASE_URL`: Valid BASE URL where the bot is deployed to use torrent web files selection. Format of URL should be `https://app-name.herokuapp.com/`, where `app-name` is the name of your heroku app. `Str`
- `TORRENT_TIMEOUT`: Timeout of dead torrents downloading with qBittorrent and Aria2c in seconds. `Int`

------

## Deploy using CLI

- Deployment instructions uploaded [HERE](https://gist.github.com/NadifMasamba/a5893e30dc4dfab34a6fa118402b53a7)
- Carefully copy-paste every CMD one by one. If you miss maybe your BOT will not run.
