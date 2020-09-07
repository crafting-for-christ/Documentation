# Verse Of The Day {docsify-ignore-all}
This projects aim is to provide the Verse Of The Day provided by [YouVersion](https://www.youversion.com/). This takes the Verse Of The Day and at the set time determined in the `config.json` will send the Verse Of The Day to the channel that is listed in `config.json`.

## Configuration
<hr>

# `config.json`
```
{
  "messagechannel": "general",

  "hour": "07",
  "minute": "00"
}
```

| Setting        | Function                                |
|----------------|-----------------------------------------|
| messagechannel | The channel that the VOTD is sent to.   |
| hour           | The hour that the VOTD is to be sent.   |
| minute         | The minute that the VOTD is to be sent. |

> If the `messagechannel` cannot be found, the VOTD will not be sent and you will receive an error in the console.

> The hour and minute configuration options are dependant on the system time.

<hr>

# `.env`
```
discordtoken=TOKEN
youversiontoken=TOKEN
```

| Setting         | Function                                                           |
|-----------------|--------------------------------------------------------------------|
| discordtoken    | The bot application token to communicate with Discord.             |
| youversiontoken | The token that allows the application to interact with YouVersion. |

> You will need to have a Discord account with a API application token and invite it to a Discord server, you can read more about that [here](https://discordpy.readthedocs.io/en/latest/discord.html).

> To obtain a YouVersion API token for the application, you can read more about it [here](https://yv-public-api-docs.netlify.app/getting-started.html#getting-an-api-token).
