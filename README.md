## alt:V - Quick Start

This repo will do everything for you; including download the latest server files.

## Official Links

-   [alt:V Website](https://altv.mp/#/)
-   [alt:V Forums](https://forum.altv.mp/)
-   [alt:V Discord](https://discordapp.com/invite/q3zUUEC)

### Installation

Install NodeJS Prior to Starting

0. Open a command prompt in a folder.

1. Run this:

```
git clone https://github.com/Stuyk/altv-quickstart
cd altv-quickstart
```

2. Run the code block below this.

    5.1. This can be used whenever you need to update your server files.

    5.2. Run the code block below; wait for packages to install.

    5.2. Then follow the instructions on screen.

```
npm run update
```

3. Bootup the Server

    3.1. This script downloads for Linux or Windows automatically.

    3.2. Use a screen on Linux to run the server in the background.

    3.3. Use a built in command prompt such as in VSCode to run the server.

    3.4. You may press `Ctrl + C` to stop the server at any time.

Linux:

```
./start.sh
```

Windows (CMD):

```
altv-server.exe
```

Windows (Powershell):

```
./altv-server.exe
```

### Recommend VSCode Plugins

-   [alt:V Auto Complete for VSCode](https://marketplace.visualstudio.com/items?itemName=stuyk.atlv-complete)

-   [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)

-   [Bracket Pair Colorizer](https://marketplace.visualstudio.com/items?itemName=CoenraadS.bracket-pair-colorizer)

### Useful Links

-   [alt:V Getting Started Guide](https://wiki.altv.mp/Tutorial_Getting_Started)

-   [alt:V JS Tutorial Series](https://www.youtube.com/watch?v=sMWCcTv4kqY&list=PLBNRUifAMZ-MzLjb-lzOTJy-PyuN6ffgw)

-   [alt:V Natives Repo](https://natives.altv.mp)

-   [alt:V JS Docs](https://altmp.github.io/altv-typings/modules/_alt_server_.html)

-   [alt:V Wiki](http://wiki.altv.mp/)

-   [alt:V O:RP Resource](https://github.com/Stuyk/altV-Open-Roleplay-altLife-Official)

-   [alt:V Auto Complete for VSCode](https://marketplace.visualstudio.com/items?itemName=stuyk.atlv-complete)

-   [alt:V Attack and Defense](https://github.com/Stuyk/altV-Attack-Defense)

### Other Useful Info

Adding Typings Naturally to the Project:

1. Run the following where your package.json is.

```
npm i -D @altv/native-types
```

2. Replace current imports with these special imports.

    2.1 For Server:

```
/// <reference types="@altv/types" />
import * as alt from 'alt-server'
```

    2.2 For Client:

```
/// <reference types="@altv/types" />
import * as alt from 'alt-client'
```

### Known Issues

If you get an issue saying that it can't use `require` for the install. What you can do instead is remove the `type: "module"` from the `package.json` file. **REMEMBER TO PUT IT BACK AFTER YOU INSTAll/UPDATE**.
