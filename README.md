# Taberna Server 6

[![Codacy Badge](https://api.codacy.com/project/badge/Grade/7a8f486b237f4fb1810010e452e326f1)](https://app.codacy.com/gh/El-Taberna/Taberna-Server-6?utm_source=github.com&utm_medium=referral&utm_content=El-Taberna/Taberna-Server-6&utm_campaign=Badge_Grade)

Taberna server 6 is the package of Taberna Modpack 6 compiled in server file ready to start them.
He can be use to create your own private or public server with the Taberna Launcher 6.

## Requirement 

-   The server required `3Go` of Ram
-   A good CPU is appreciated
-   Java `8` or Newer
-   The last update of the server package

## Installation

Download the [last update source code](https://github.com/El-Taberna/Taberna-Server-6/releases/latest) to start the server.

## Usage

### On Windows

-   Unzip your file
-   start run.bat

### On Linux

-   In `Root` write in your bash :

```bash
sudo apt update && upgrade
```

```bash
apt-get install default-jdk screen
```

```bash
sudo adduser minecraft
```

-   Now you need to connect on minecraft :

```bash
su minecraft
```

```bash
cd /home/minecraft
```

-   Upload last update of server files in `/home/minecraft/`

```bash
touch eula.txt && echo "eula=true" >> eula.txt
```

-   Downlaod the `minecraft.sh` script to start easily  :

```bash
wget -O /etc/init.d/minecraft http://taberna6.el-taberna.com/server/minecraft.sh
```

-   Create a backup directory :

```bash
mkdir /home/minecraft/backups
```

-   Make your script executable :

```bash
chmod +x /etc/init.d/minecraft

chown minecraft:minecraft /etc/init.d/minecraft

chown -R minecraft:minecraft /home/minecraft/
```

-   Launch at Startup (Not Recommended) :

```bash
update-rc.d minecraft defaults
```

-   Now you can start your server with this command :

``` bash
service minecraft start
```

- All the commands :

``` bash
service minecraft {start|stop|update|backup|status|restart}
```

**/!\ Attention /!\**

If you want to edit the script to increase the ram, follow the instructions :

```bash
nano /etc/init.d/minecraft
```

edit this line : `INVOCATION='java -Xmx3072M -Xms3072M -jar minecraft_server.jar nogui'`

for save and leave make *ctrl+o*, enter and *ctrl+x*.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
