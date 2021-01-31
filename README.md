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

Download the [last update source code](https://github.com/El-Taberna/Taberna-Server/releases/latest) to start the server.

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
sudo apt install openjdk-8-jre-headless screen
```

```bash
sudo adduser minecraft
```

-   Now you need to connect on minecraft

```bash
su minecraft
```

-   Upload last update of server files in `/home/minecraft/`
-   Create `Run.sh` and paste this inside `/home/minecraft/`

```bash
#!/bin/sh

java -Xms1024M -Xmx3072M -jar minecraft_server.jar -o true
```

-   Make `Run.sh` executable

```bash
chmod +x /home/minecraft/run.sh
```

-   To start your server :

``` bash
screen /home/minecraft/run.sh
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
