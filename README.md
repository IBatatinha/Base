### About the project
The project was developed to help the developers a create their  projects without worrying in create own base or search ones to use. This base provide just essential scripts and the best optimization. So as to developers have a good experience using the base and creating their projects.

---
#### Project's Details
- **Framework used:** vRP 1.0 (https://github.com/vRP-framework/vRP/tree/1.0)
- **Language**: Lua
- **Database**: MariaDB (to view use **HeidiSql** or **phpMyadmin**)
- **Wrapper**: Oxmysql (https://github.com/overextended/oxmysql)
### 📄 Documentation

### Startup
>   Before starting the base you will have to do somethings before.
1. Create `license.cfg` in `server-data/config`, after this copy/cut this code and paste it in `license.cfg` and fill with your keys.
```cfg
set steam_webApiKey "" # (https://steamcommunity.com/dev/apikey)
sv_licenseKey changeme # (https://portal.cfx.re)
```

2. You will need to install the **artifacts** of server in [FiveM Artifacts](https://runtime.fivem.net/artifacts/fivem/build_server_windows/master/) so that start the server. After installing, you will have to create a folder called `server-artifacts` in the root directory,outside of `server-data`.

3. After all steps complete, you will need to install a **database view** (like HeidiSql) and you will have to install also the **MariaDB** or **Xampp** to start the database and can use it.
   1. Download **HeidiSql** or if you have a own database view and can view **MariaDB** you can skip this. [Download Here](https://www.heidisql.com/)
   2. Download **MariaDB**: In this situation you can use [**Xampp**](https://www.apachefriends.org/pt_br/index.html), but i prefer use own [**MariaDB**](https://mariadb.org/), because after install this you "never" will have problems and you don't need more start the database to use it, because this have a automatic start with Windows. Besides this, I think this more optimized than **Xampp** and don't have much problem like one.

### Extras
> In some situations, if you need to use **ace permissions**, you can copy this example code below and paste in `server.cfg`.

```cfg
  add_ace group.admin command allow
  add_ace group.admin command.quit deny
  add_principal identifier.steam:STEAM_HEX group.admin
```