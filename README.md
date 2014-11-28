Dj4x
===

Utility bot for IRC. Runs on HexChat 2.10 and later versions.

How to clone the bot
--------------------

First of all, make sure you have Python installed and Python Plugin installed with the HexChat your bot will use.

Second, create an account on Freenode for your bot. Ask for a cloak to your name on the `#Freenode` channel.

Finaly, set HexChat server configuration to autoconnect and autologin your bot. Use SSL to secure your connexion.

After that, change the bot files to suite your needs:

1. Copy the code and the json files into `.config/hexchat/addons/` (Linux) or `%appdata%\HexChat\addons\` (Windows). This will make HexChat run the code automatically on startup.

2. Rename the files depending on your bot name and change settings in the files:

* `_data.json` file:
>
> Rename the bot (`bot:name`).
>
> Set a description for the bot (`bot:description`).
>
> Name the version (bot:version_info:name and `:link`).
>
> The `:cmd_default` option is a kameo-like that creates a command which displays information on the current version (there's are two commands there, one that displays text and another that makes a `/me` action).
>
> By default, triggers are: `+` for user commands, `%` for admin commands, `#` for special user commands, `+` for help commands and `*` for API-dependant commands. You can change that in triggers property.
>
> Set the admins, the special users, the `tip_params` and the `rain_params`.
>
> `timer_first_timout` is a timeout that launches only once after the bot registers and loads. Set it to 2 minutes or less if you are sure that the bots connects quickly. `timer_timeout` is by default set to 10 minutes. It checks for the balance and regains the bot original nickname.
>
> `rain_params:rain_timeout` defines how much time one can be inactive and stays in the rain list.
>
> As the bot receives tips and tips randomly, `tip_timeout` is used to automatically keep tips if the used does not use the coins. Default to 5 minutes.
>
> Don't change `tip_manage_commands` unless you are willing to change the code that manages the tips.
>
> If you are willing to use the Microsoft Translation API, register on api.microsofttranslator.com and get a "client id" and a "client secret". Set them in `ms_params:ms_client_id` and `:ms_client_secret`.
>
> Sets the reminders in `reminders` as you wish. Give them a name, a message to post, a timeout and list the channels where the message will be periodically posted.

* `_users.json` file:
>
> Keep the same data structure and define user data. Examples are given. Don't forget to set data for your bot. Set `data:donation` to the address you want people to send donations to. It will be displayed when someone uses the donate command.
>
> The `data` part lists data for pools and addie, it is used when querrying a command with the `me` argument. Next versions will let users define their own data.

* `.py` file:
>
> Define the `SYSTEM`, `PYTHON` and `LOCAL` constants. Change the `data_file` paths.
>
> `help_api` allows you to add help for api-dependant commands.
>
> You can add simple commands by adding entries to `get_msg` and `get_action`.
>
> `get_msg` creates commands that sends message to the channel where the trigger is used. `:words` is a string of the message to send to the channel. `:descr` is an array of lines that will be displayed as help to the command.
>
> `get_action` creates /me-like actions on the channel where the trigger is used. `:words` is an array of two elements. The first is the infinitive form and the second the form in the 3rd person of singular, Present tense. `:suppl` is an array of supplements that will be randomly shown to complete the action; use `[""]` if you want nothing to be shown after the action. `:reason_no` describes the reason why the action cannot be performed on ChanServ. `:descr` is an array of lines to show in help on the command.
>
> `get_reaction` creates reactions to strings in what users say in a channel.
>
> Finaly, you can search for "Dj4x" or "dj4x" in the code and replace it with your bot's name. This will be fixed in the following versions.

