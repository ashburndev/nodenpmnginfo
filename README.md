# node npm ng info

    ashburndave@dphnuc4:~$ node --version
    v10.1.0
    ashburndave@dphnuc4:~$ npm --version
    5.6.0

       ╭─────────────────────────────────────╮
       │                                     │
       │   Update available 5.6.0 → 6.1.0    │
       │     Run npm i -g npm to update      │
       │                                     │
       ╰─────────────────────────────────────╯
    
    ashburndave@dphnuc4:~$ 
    ashburndave@dphnuc4:~$ ng version
    The program 'ng' is currently not installed. You can install it by typing:
    sudo apt install ng-common
    ashburndave@dphnuc4:~$ 
    ashburndave@dphnuc4:~$ 
    ashburndave@dphnuc4:~$ npm install -g @angular/cli

    ashburndave@dphnuc4:~$ ng version

         _                      _                 ____ _     ___
        / \   _ __   __ _ _   _| | __ _ _ __     / ___| |   |_ _|
       / △ \ | '_ \ / _` | | | | |/ _` | '__|   | |   | |    | |
      / ___ \| | | | (_| | |_| | | (_| | |      | |___| |___ | |
     /_/   \_\_| |_|\__, |\__,_|_|\__,_|_|       \____|_____|___|
                    |___/
        

    Angular CLI: 6.0.8
    Node: 10.1.0
    OS: linux x64
    Angular: 
    ... 

    Package                      Version
    ------------------------------------------------------
    @angular-devkit/architect    0.6.8
    @angular-devkit/core         0.6.8
    @angular-devkit/schematics   0.6.8
    @schematics/angular          0.6.8
    @schematics/update           0.6.8
    rxjs                         6.2.1
    typescript                   2.7.2
        
    ashburndave@dphnuc4:~$ 


## nvm (node version manager)

I installed nvm (node version manager) using the instructions in the book "Get Programming wth Node.js".

https://github.com/creationix/nvm

    ashburndave@dphnuc4:~$ nvm list
    ->      v10.1.0
    default -> 10.1.0 (-> v10.1.0)
    node -> stable (-> v10.1.0) (default)
    stable -> 10.1 (-> v10.1.0) (default)
    iojs -> N/A (default)
    lts/* -> lts/carbon (-> N/A)
    lts/argon -> v4.9.1 (-> N/A)
    lts/boron -> v6.14.2 (-> N/A)
    lts/carbon -> v8.11.2 (-> N/A)
    ashburndave@dphnuc4:~$ 
    ashburndave@dphnuc4:~$ nvm ls-remote node | tail
            v9.11.2
            v10.0.0
    ->      v10.1.0
            v10.2.0
            v10.2.1
            v10.3.0
            v10.4.0
            v10.4.1
            v10.5.0
            v10.6.0
    ashburndave@dphnuc4:~$ 

I could have downloaded the node distribution from these URLs (the first is for LTS, long term support, versions)

https://nodejs.org/en/download/
https://nodejs.org/en/download/current/

    ashburndave@dphnuc4:~/Downloads$ ls -latr | tail
    -rw-rw-r--  1 ashburndave ashburndave         40 Jul  8 09:46 apache-maven-3.5.4-bin.zip.sha1
    -rw-rw-r--  1 ashburndave ashburndave        236 Jul  8 09:46 apache-maven-3.5.4-bin.zip.asc
    drwxr-xr-x 44 ashburndave ashburndave       4096 Jul 11 07:46 ..
    -rw-rw-r--  1 ashburndave ashburndave   11351132 Jul 11 07:50 node-v8.11.3-linux-x64.tar.xz
    -rw-rw-r--  1 ashburndave ashburndave   31115954 Jul 11 07:51 node-v8.11.3.tar.gz
    -rw-rw-r--  1 ashburndave ashburndave       4585 Jul 11 07:51 node-v8.11.3.SHASUMS256.txt.asc
    -rw-rw-r--  1 ashburndave ashburndave   12139756 Jul 11 08:04 node-v10.6.0-linux-x64.tar.xz
    -rw-rw-r--  1 ashburndave ashburndave   35531041 Jul 11 08:05 node-v10.6.0.tar.gz
    -rw-rw-r--  1 ashburndave ashburndave       4187 Jul 11 08:06 node-v10.6.0.SHASUMS256.txt.asc
    drwxr-xr-x  2 ashburndave ashburndave      20480 Jul 11 08:07 .
    ashburndave@dphnuc4:~/Downloads$ 




