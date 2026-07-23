# Anti TCC

Security Mutator  
Copyright &copy; 2003-2009 by [Wormbo](http://www.koehler-homepage.de/Wormbo/)  
Copyright &copy; 2026 by OldUnreal

## Download

The latest release of AntiTCC [can be found here](https://github.com/OldUnreal/AntiTCC-Releases/releases/latest). 

Older releases [can be found here](https://github.com/OldUnreal/AntiTCC-Releases/releases).

## Installation (Server)

To install Anti TCC on your server, simply extract the content of the ZIP archive to your server's System directory.

To make sure Anti TCC is loaded all the time, add the following line to the `[Engine.GameEngine]` section of your server's main INI file (usually UT2004.ini):

```
ServerActors=AntiTCC_2026r6.MutAntiTCCFinal
```

The ServerActors line already ensures Anti TCC is loaded all the time, so you do not need to add it to other mutator loaders, such as UT2Vote's ServerMuts list. If you only want to load Anti TCC in certain configurations, e.g. via map voting, add it in the "?mutator=" the URL parameter instead.

If you want to record demos on the server or the clients, you should also add the following line in the `[Engine.GameEngine]` section:
```
ServerPackages=AntiTCC_2026r6
```

## Installation (Client)

As a client you should not install Anti TCC. When connecting to a server running Anti TCC, the package will be downloaded into your UT2004 Cache directory. The download is small and fast, and you will always have the correct version required by the server.


