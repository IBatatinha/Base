## Documentation
### Startup
> To start the base you will need to create a file in paste called `config` in `server-data`, the file must be called `license.cfg`, after creating you must put the code in the file and fill with your keys.
```cfg
set steam_webApiKey "" # (https://steamcommunity.com/dev/apikey)
sv_licenseKey changeme # (https://portal.cfx.re)
```

### Extra
> In same cases, might you have been using **ace permissions**, so for this you will need to put this code in `server.cfg`.
```cfg
add_ace group.admin command allow
add_ace group.admin command.quit deny
add_principal identifier.steam:STEAM_HEX group.admin
```
