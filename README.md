This is my MODPACK AND SERVER (Separatly and Optional) for SPT Aki 3.10

***WARNING***

**YOU MUST NEED TO HAVE Escape From Tarkov OFFICIAL GAME VERSION INSTALLED AND UPDATED**
[Official EFT](https://www.escapefromtarkov.com/preorder-page/)
**YOU NEED TO DOWNLOAD SPT AKI FROM THE OFFICIAL WEBSITE**
[SPT Aki Installer](https://hub.sp-tarkov.com/files/file/672-spt-installer/)

How to **INSTALL** :

1.  Unzip the folder on your SSD or SSD M.2 (ONLY ON SSD NOT HDD)
2.  You got 2 zip files one for the SPT Aki (GAME FOLDER) seconde one for the SPT Aki SERVER (SERVER FOLDER)
3.  Unzip this two zip (If you want to run server separatly from another PC move the SERVER zip to your 2nd PC and unzip it) See ***Server config*** for CONFIGURATION
4.  Copy and Past, allow if demanded.

**Launcher Config**

1.  Verify and modify if nessessary "user/launcher/config.json" And add "127.0.0.1"
2.  Modify the "GamePath" to your actulal PATH of your GAME FOLDER is
3.  Run the SPT.Server.exe after he say server you can start launch the SPT.Launcher.exe (If you dont want to run server on antoher PC localy)

**Server Config**

1.  Go to your PATH server folder and open "SPT_Data\Server\configs" you can found file named **http.json**
2.  Open this file with VSCode or any other text editor
3.  Modify "ip" and "backendIp" to you 2nd PC that you want to run the server with your local ip address
4.  Go to  "SPT_Data\Server\" and open server.json and do the same thing 
5.  After that done go to your Windows FireWall and add TCP and UDP rules to allow the 6969 port on INCOMING and OUTCOMING trafic to allow other PC to enable connection to your pc with the mentioned port
6.  See ***Launcher Config***

**Launcher Config**

1.  Go to your ***Main PC*** and open "user/launcher/config.json"
2.  Modify the "GamePath" to your actulal PATH of your GAME FOLDER is
3.  Do same thing of the ***Server Config*** and mofify "Url" to match to your 2nd PC that the server is stored 

**Performance**

1.  Go to "EscapeFromTarkov_Data" folder and open boot.config 
2.  Copy and Paste : 
                        gfx-enable-gfx-jobs=1
                        gfx-enable-native-gfx-jobs=1
                        gfx-disable-mt-rendering=1
                        wait-for-native-debugger=0
                        vr-enabled=0
                        hdr-display-enabled=0
                        gc-max-time-slice=10
                        job-worker-count=15 (**See how many core your CPU have and -1, ex : if you have 16 = 16-1=15**)
                        single-instance=
