### CHANGE BOT BANNER 
> javascript, node.js & discord.js
```js
        const fs = require('node:fs');
        const { REST } = require("@discordjs/rest");
        const { Routes } = require("discord-api-types/v9");
        const { DataResolver } = require("discord.js");

        const rest = new REST({ version: "9" }).setToken("BOT_TOKEN_HERE");

        try {
            await rest.patch(Routes.user(), {
                body: { banner: await DataResolver.resolveImage("CAMINHO DO ARQUIVO OU LINK DO BANNER") },
            });
            console.log("Banner updated successfully!!!")
        } catch (err) {
            console.log("Failed to update banner:\n"+ err)
        }
```
For more information join the server [Discord Developers (DDevs)](https://discord.com/invite/discord-developers)

![image](https://github.com/ravenastar-js/shortlinks-scams/assets/31909648/44c7a375-dc2e-48cc-af41-0549e3914e64)
