# node npm ng info

As of July 12, 2018, the web page https://angular.io/guide/quickstart indicates the following versions of Node.js and npm are required.  I do not know if that is only in the context of Angular 6, or if it applies to any earlier versions of Angular also.

Verify that you are running at least Node.js version 8.x or greater and npm version 5.x or greater by running node -v and npm -v in a terminal/console window. Older versions produce errors, but newer versions are fine.

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
        
    ashburndave@dphnuc4:~/ngprojects$ ng mew hello-cli
        
    added 1103 packages in 36.853s
        Successfully initialized git.
    ashburndave@dphnuc4:~/ngprojects$ 
    ashburndave@dphnuc4:~/ngprojects$ cd hello-cli
    ashburndave@dphnuc4:~/ngprojects/hello-cli$ 
    ashburndave@dphnuc4:~/ngprojects/hello-cli$ ls -latr
    total 436
    -rw-r--r--   1 ashburndave ashburndave   2805 Jul 12 05:26 tslint.json
    -rw-r--r--   1 ashburndave ashburndave    384 Jul 12 05:26 tsconfig.json
    -rw-r--r--   1 ashburndave ashburndave   1025 Jul 12 05:26 README.md
    -rw-r--r--   1 ashburndave ashburndave    503 Jul 12 05:26 .gitignore
    -rw-r--r--   1 ashburndave ashburndave    245 Jul 12 05:26 .editorconfig
    -rw-r--r--   1 ashburndave ashburndave   3575 Jul 12 05:26 angular.json
    drwxr-xr-x   3 ashburndave ashburndave   4096 Jul 12 05:26 ..
    drwxr-xr-x   5 ashburndave ashburndave   4096 Jul 12 05:26 src
    drwxr-xr-x   3 ashburndave ashburndave   4096 Jul 12 05:26 e2e
    drwxr-xr-x 808 ashburndave ashburndave  32768 Jul 12 05:27 node_modules
    -rw-r--r--   1 ashburndave ashburndave   1314 Jul 12 05:27 package.json
    -rw-r--r--   1 ashburndave ashburndave 362565 Jul 12 05:27 package-lock.json
    drwxr-xr-x   6 ashburndave ashburndave   4096 Jul 12 05:27 .
    drwxr-xr-x   8 ashburndave ashburndave   4096 Jul 12 05:27 .git
    ashburndave@dphnuc4:~/ngprojects/hello-cli$ 
    ashburndave@dphnuc4:~/ngprojects/hello-cli$ cat README.md 
    # HelloCli
        
    This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 6.0.8.
        
    ## Development server
        
    Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.
        
    ## Code scaffolding
        
    Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.
        
    ## Build
        
    Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.
        
    ## Running unit tests
        
    Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).
        
    ## Running end-to-end tests
        
    Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).
        
    ## Further help
        
    To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
    ashburndave@dphnuc4:~/ngprojects/hello-cli$ 
    ashburndave@dphnuc4:~/ngprojects/hello-cli$ cat package.json 
    {
      "name": "hello-cli",
      "version": "0.0.0",
      "scripts": {
        "ng": "ng",
        "start": "ng serve",
        "build": "ng build",
        "test": "ng test",
        "lint": "ng lint",
        "e2e": "ng e2e"
      },
      "private": true,
      "dependencies": {
        "@angular/animations": "^6.0.3",
        "@angular/common": "^6.0.3",
        "@angular/compiler": "^6.0.3",
        "@angular/core": "^6.0.3",
        "@angular/forms": "^6.0.3",
        "@angular/http": "^6.0.3",
        "@angular/platform-browser": "^6.0.3",
        "@angular/platform-browser-dynamic": "^6.0.3",
        "@angular/router": "^6.0.3",
        "core-js": "^2.5.4",
        "rxjs": "^6.0.0",
        "zone.js": "^0.8.26"
      },
      "devDependencies": {
        "@angular/compiler-cli": "^6.0.3",
        "@angular-devkit/build-angular": "~0.6.8",
        "typescript": "~2.7.2",
        "@angular/cli": "~6.0.8",
        "@angular/language-service": "^6.0.3",
        "@types/jasmine": "~2.8.6",
        "@types/jasminewd2": "~2.0.3",
        "@types/node": "~8.9.4",
        "codelyzer": "~4.2.1",
        "jasmine-core": "~2.99.1",
        "jasmine-spec-reporter": "~4.2.1",
        "karma": "~1.7.1",
        "karma-chrome-launcher": "~2.2.0",
        "karma-coverage-istanbul-reporter": "~2.0.0",
        "karma-jasmine": "~1.1.1",
        "karma-jasmine-html-reporter": "^0.2.2",
        "protractor": "~5.3.0",
        "ts-node": "~5.0.1",
        "tslint": "~5.9.1"
      }
    }
    ashburndave@dphnuc4:~/ngprojects/hello-cli$ 


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

The web page http://www.tutorialspoint.com/nodejs/nodejs_environment_setup.htm suggests these steps for installing Node.js

        $ cd /tmp
        $ wget http://nodejs.org/dist/v6.3.1/node-v6.3.1-linux-x64.tar.gz
        $ tar xvfz node-v6.3.1-linux-x64.tar.gz
        $ mkdir -p /usr/local/nodejs
        $ mv node-v6.3.1-linux-x64/* /usr/local/nodejs

In the web page https://blog.angularindepth.com/angular-5-or-angular-6-yes-please-d71b08b5e59b Todd Palmer has suggestions about a single development environment for both Angular 6 and Angular 5 development.  I had problems installing angular-cli 5 after having first installed angular-cli 6.

Install (or reinstall) Angular 6 globally before creating a new Angular 6 project with angular-cli

        npm install -g @angular/cli@6
        ng version
        ng new my-ng6-app

Install (or reinstall) Angular 5 globally before creating a new Angular 6 project with angular-cli

        npm install -g @angular/cli@1
        ng version
        ng new my-ng5-app

## sample angular 6 project (created with angular-cli)

        ashburndave@dphnuc4:~/ng6projects/myng6app$ ls -latr
        total 436
        -rw-r--r--   1 ashburndave ashburndave   2805 Jul 15 08:49 tslint.json
        -rw-r--r--   1 ashburndave ashburndave    384 Jul 15 08:49 tsconfig.json
        -rw-r--r--   1 ashburndave ashburndave   1025 Jul 15 08:49 README.md
        -rw-r--r--   1 ashburndave ashburndave    503 Jul 15 08:49 .gitignore
        -rw-r--r--   1 ashburndave ashburndave    245 Jul 15 08:49 .editorconfig
        -rw-r--r--   1 ashburndave ashburndave   3566 Jul 15 08:49 angular.json
        drwxr-xr-x   3 ashburndave ashburndave   4096 Jul 15 08:49 ..
        drwxr-xr-x   5 ashburndave ashburndave   4096 Jul 15 08:49 src
        drwxr-xr-x   3 ashburndave ashburndave   4096 Jul 15 08:49 e2e
        drwxr-xr-x 808 ashburndave ashburndave  32768 Jul 15 08:50 node_modules
        -rw-r--r--   1 ashburndave ashburndave   1313 Jul 15 08:50 package.json
        -rw-r--r--   1 ashburndave ashburndave 362570 Jul 15 08:50 package-lock.json
        drwxr-xr-x   6 ashburndave ashburndave   4096 Jul 15 08:50 .
        drwxr-xr-x   8 ashburndave ashburndave   4096 Jul 15 08:50 .git
        ashburndave@dphnuc4:~/ng6projects/myng6app$ 
        ashburndave@dphnuc4:~/ng6projects/myng6app$ tree -d -L 2 > ~/myng6app.tree.md
        ashburndave@dphnuc4:~/ng6projects/myng6app$ 
        ashburndave@dphnuc4:~/ng6projects/myng6app$ cat README.md
        # Myng6app
        
        This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 6.0.8.
        
        ## Development server
        
        Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.
        
        ## Code scaffolding
        
        Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.
        
        ## Build
        
        Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.
        
        ## Running unit tests
        
        Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).
        
        ## Running end-to-end tests
        
        Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).
        
        ## Further help
        
        To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
        ashburndave@dphnuc4:~/ng6projects/myng6app$ 
        ashburndave@dphnuc4:~/ng6projects/myng6app$ cat package.json
        {
          "name": "myng6app",
          "version": "0.0.0",
          "scripts": {
            "ng": "ng",
            "start": "ng serve",
            "build": "ng build",
            "test": "ng test",
            "lint": "ng lint",
            "e2e": "ng e2e"
          },
          "private": true,
          "dependencies": {
            "@angular/animations": "^6.0.3",
            "@angular/common": "^6.0.3",
            "@angular/compiler": "^6.0.3",
            "@angular/core": "^6.0.3",
            "@angular/forms": "^6.0.3",
            "@angular/http": "^6.0.3",
            "@angular/platform-browser": "^6.0.3",
            "@angular/platform-browser-dynamic": "^6.0.3",
            "@angular/router": "^6.0.3",
            "core-js": "^2.5.4",
            "rxjs": "^6.0.0",
            "zone.js": "^0.8.26"
          },
          "devDependencies": {
            "@angular/compiler-cli": "^6.0.3",
            "@angular-devkit/build-angular": "~0.6.8",
            "typescript": "~2.7.2",
            "@angular/cli": "~6.0.8",
            "@angular/language-service": "^6.0.3",
            "@types/jasmine": "~2.8.6",
            "@types/jasminewd2": "~2.0.3",
            "@types/node": "~8.9.4",
            "codelyzer": "~4.2.1",
            "jasmine-core": "~2.99.1",
            "jasmine-spec-reporter": "~4.2.1",
            "karma": "~1.7.1",
            "karma-chrome-launcher": "~2.2.0",
            "karma-coverage-istanbul-reporter": "~2.0.0",
            "karma-jasmine": "~1.1.1",
            "karma-jasmine-html-reporter": "^0.2.2",
            "protractor": "~5.3.0",
            "ts-node": "~5.0.1",
            "tslint": "~5.9.1"
          }
        }
        ashburndave@dphnuc4:~/ng6projects/myng6app$ 
        ashburndave@dphnuc4:~/ng6projects/myng6app$ cat .gitignore 
        # See http://help.github.com/ignore-files/ for more about ignoring files.
        
        # compiled output
        /dist
        /tmp
        /out-tsc
        
        # dependencies
        /node_modules
        
        # IDEs and editors
        /.idea
        .project
        .classpath
        .c9/
        *.launch
        .settings/
        *.sublime-workspace
        
        # IDE - VSCode
        .vscode/*
        !.vscode/settings.json
        !.vscode/tasks.json
        !.vscode/launch.json
        !.vscode/extensions.json
        
        # misc
        /.sass-cache
        /connect.lock
        /coverage
        /libpeerconnection.log
        npm-debug.log
        yarn-error.log
        testem.log
        /typings
        
        # System Files
        .DS_Store
        Thumbs.db
        ashburndave@dphnuc4:~/ng6projects/myng6app$ 
        ashburndave@dphnuc4:~/ng6projects/myng6app$ tree src
        src
        ├── app
        │   ├── app.component.css
        │   ├── app.component.html
        │   ├── app.component.spec.ts
        │   ├── app.component.ts
        │   └── app.module.ts
        ├── assets
        ├── browserslist
        ├── environments
        │   ├── environment.prod.ts
        │   └── environment.ts
        ├── favicon.ico
        ├── index.html
        ├── karma.conf.js
        ├── main.ts
        ├── polyfills.ts
        ├── styles.css
        ├── test.ts
        ├── tsconfig.app.json
        ├── tsconfig.spec.json
        └── tslint.json
        
        3 directories, 18 files
        ashburndave@dphnuc4:~/ng6projects/myng6app$ 



## sample angular 5 project (created with angular-cli)

        ashburndave@dphnuc4:~$ npm install -g @angular/cli@1
        npm WARN registry Using stale data from https://registry.npmjs.org/ because the host is inaccessible -- are you offline?
        npm WARN registry Using stale package data from https://registry.npmjs.org/ due to a request error during revalidation.
        [..................] \ fetchMetadata: sill fetchPackageMetaData error for node-modules-path@^1.0.0 request to https://registry.npmjs.org/node-modules-path fail
        
        ashburndave@dphnuc4:~$ 
        ashburndave@dphnuc4:~$ npm install -g @angular/cli@1
        npm WARN registry Using stale data from https://registry.npmjs.org/ because the host is inaccessible -- are you offline?
        npm WARN registry Using stale package data from https://registry.npmjs.org/ due to a request error during revalidation.
        npm ERR! code ENOTFOUND
        npm ERR! errno ENOTFOUND
        npm ERR! network request to https://registry.npmjs.org/@ngtools%2fjson-schema failed, reason: getaddrinfo ENOTFOUND registry.npmjs.org registry.npmjs.org:443
        npm ERR! network This is a problem related to network connectivity.
        npm ERR! network In most cases you are behind a proxy or have bad network settings.
        npm ERR! network 
        npm ERR! network If you are behind a proxy, please make sure that the
        npm ERR! network 'proxy' config is set properly.  See: 'npm help config'
        
        npm ERR! A complete log of this run can be found in:
        npm ERR!     /home/ashburndave/.npm/_logs/2018-07-15T13_05_34_110Z-debug.log
        ashburndave@dphnuc4:~$ 
        ashburndave@dphnuc4:~$ angular version
        angular: command not found
        ashburndave@dphnuc4:~$ 
        ashburndave@dphnuc4:~$ node --version
        v10.1.0
        ashburndave@dphnuc4:~$ npm --version
        5.6.0
        ashburndave@dphnuc4:~$ 
        ashburndave@dphnuc4:~$ npm install -g @angular/cli@6
        /home/ashburndave/.nvm/versions/node/v10.1.0/bin/ng -> /home/ashburndave/.nvm/versions/node/v10.1.0/lib/node_modules/@angular/cli/bin/ng
        
        > @angular/cli@6.0.8 postinstall /home/ashburndave/.nvm/versions/node/v10.1.0/lib/node_modules/@angular/cli
        > node ./bin/ng-update-message.js
        
        npm WARN optional SKIPPING OPTIONAL DEPENDENCY: fsevents@1.2.4 (node_modules/@angular/cli/node_modules/fsevents):
        npm WARN notsup SKIPPING OPTIONAL DEPENDENCY: Unsupported platform for fsevents@1.2.4: wanted {"os":"darwin","arch":"any"} (current: {"os":"linux","arch":"x64"})
        
        + @angular/cli@6.0.8
        updated 4 packages in 9.633s
        ashburndave@dphnuc4:~$ 
        
        ashburndave@dphnuc4:~$ ng --version
        
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
        rxjs                         6.2.2
        typescript                   2.7.2
            
        ashburndave@dphnuc4:~$ 

## experiment with git

        ashburndave@dphnuc4:/tmp$ mkdir testproj
        ashburndave@dphnuc4:/tmp$ cd testproj
        ashburndave@dphnuc4:/tmp/testproj$ git status
        fatal: Not a git repository (or any of the parent directories): .git
        ashburndave@dphnuc4:/tmp/testproj$ 
        ashburndave@dphnuc4:/tmp/testproj$ git init
        Initialized empty Git repository in /tmp/testproj/.git/
        ashburndave@dphnuc4:/tmp/testproj$ 
        ashburndave@dphnuc4:/tmp/testproj$ git status
        On branch master
        
        No commits yet
        
        nothing to commit (create/copy files and use "git add" to track)
        ashburndave@dphnuc4:/tmp/testproj$ date > foo.txt
        ashburndave@dphnuc4:/tmp/testproj$ date > bar.txt
        ashburndave@dphnuc4:/tmp/testproj$ date > baz.txt
        ashburndave@dphnuc4:/tmp/testproj$ git status
        On branch master
        
        No commits yet
        
        Untracked files:
          (use "git add <file>..." to include in what will be committed)
        
            bar.txt
            baz.txt
            foo.txt
        
        nothing added to commit but untracked files present (use "git add" to track)
        ashburndave@dphnuc4:/tmp/testproj$ git add .
        ashburndave@dphnuc4:/tmp/testproj$ git status
        On branch master
        
        No commits yet
        
        Changes to be committed:
          (use "git rm --cached <file>..." to unstage)
        
            new file:   bar.txt
            new file:   baz.txt
            new file:   foo.txt
        
        ashburndave@dphnuc4:/tmp/testproj$ git commit -a -m "first commit"
        [master (root-commit) b106b46] first commit
         3 files changed, 3 insertions(+)
         create mode 100644 bar.txt
         create mode 100644 baz.txt
         create mode 100644 foo.txt
        ashburndave@dphnuc4:/tmp/testproj$ git status
        On branch master
        nothing to commit, working tree clean
        ashburndave@dphnuc4:/tmp/testproj$ 

## using git with an angular project created with angular-cli

        ng new myang6app
        cd myang6app
        git remote add origin git@github.com:ashburndev/myng6app.git
        git push -u origin master

        ashburndave@dphnuc4:~/ng6projects/myng6app$ git remote add origin git@github.com:ashburndev/myng6app.git
        ashburndave@dphnuc4:~/ng6projects/myng6app$ git push -u origin master
        Counting objects: 38, done.
        Delta compression using up to 4 threads.
        Compressing objects: 100% (36/36), done.
        Writing objects: 100% (38/38), 93.35 KiB | 4.45 MiB/s, done.
        Total 38 (delta 1), reused 0 (delta 0)
        remote: Resolving deltas: 100% (1/1), done.
        To github.com:ashburndev/myng6app.git
         * [new branch]      master -> master
        Branch master set up to track remote branch master from origin.
        ashburndave@dphnuc4:~/ng6projects/myng6app$ 

I did not expect that everything created by angular-cli would already be commited and pushed to the .git created by angular-cli ... an alternative to the above is as follows

        ng new myang6app --skip-git
        cd myang6app
        git init
        git add .
        git commit -a -m "first commit"
        git push

As a test, I deleted everything and started over again.  After entering this command ...

        ng new myang6app

... I entered the commands below ... and I ended up with the desired content in the github repository

        ashburndave@dphnuc4:~/ng6projects$ cd myng6app/
        ashburndave@dphnuc4:~/ng6projects/myng6app$ git status
        On branch master
        nothing to commit, working tree clean
        ashburndave@dphnuc4:~/ng6projects/myng6app$ git add .
        ashburndave@dphnuc4:~/ng6projects/myng6app$ git commit -a -m "first commit"
        On branch master
        nothing to commit, working tree clean
        ashburndave@dphnuc4:~/ng6projects/myng6app$ git remote add origin git@github.com:ashburndev/myng6app.git
        ashburndave@dphnuc4:~/ng6projects/myng6app$ git push -u origin master
        Counting objects: 38, done.
        Delta compression using up to 4 threads.
        Compressing objects: 100% (36/36), done.
        Writing objects: 100% (38/38), 93.41 KiB | 4.67 MiB/s, done.
        Total 38 (delta 1), reused 0 (delta 0)
        remote: Resolving deltas: 100% (1/1), done.
        To github.com:ashburndev/myng6app.git
         * [new branch]      master -> master
        Branch master set up to track remote branch master from origin.
        ashburndave@dphnuc4:~/ng6projects/myng6app$ 

As a further experiment, I tried to clone the repository created above.

        ashburndave@dphnuc4:~$ cd /tmp
        ashburndave@dphnuc4:/tmp$ git clone git@github.com:ashburndev/myng6app.git
        Cloning into 'myng6app'...
        remote: Counting objects: 38, done.
        remote: Compressing objects: 100% (35/35), done.
        remote: Total 38 (delta 1), reused 38 (delta 1), pack-reused 0
        Receiving objects: 100% (38/38), 93.41 KiB | 2.92 MiB/s, done.
        Resolving deltas: 100% (1/1), done.
        ashburndave@dphnuc4:/tmp$ 
        ashburndave@dphnuc4:/tmp$ cd myng6app/
        ashburndave@dphnuc4:/tmp/myng6app$ ng serve
        Could not find module "@angular-devkit/build-angular" from "/tmp/myng6app".
        Error: Could not find module "@angular-devkit/build-angular" from "/tmp/myng6app".
            at Object.resolve (/home/ashburndave/.nvm/versions/node/v10.1.0/lib/node_modules/@angular/cli/node_modules/@angular-devkit/core/node/resolve.js:141:11)
            at Observable.rxjs_1.Observable [as _subscribe] (/home/ashburndave/.nvm/versions/node/v10.1.0/lib/node_modules/@angular/cli/node_modules/@angular-devkit/architect/src/architect.js:132:40)
            at Observable._trySubscribe (/home/ashburndave/.nvm/versions/node/v10.1.0/lib/node_modules/@angular/cli/node_modules/rxjs/internal/Observable.js:43:25)
            at Observable.subscribe (/home/ashburndave/.nvm/versions/node/v10.1.0/lib/node_modules/@angular/cli/node_modules/rxjs/internal/Observable.js:29:22)
            at DoOperator.call (/home/ashburndave/.nvm/versions/node/v10.1.0/lib/node_modules/@angular/cli/node_modules/rxjs/internal/operators/tap.js:29:23)
            at Observable.subscribe (/home/ashburndave/.nvm/versions/node/v10.1.0/lib/node_modules/@angular/cli/node_modules/rxjs/internal/Observable.js:24:22)
            at /home/ashburndave/.nvm/versions/node/v10.1.0/lib/node_modules/@angular/cli/node_modules/rxjs/internal/util/subscribeTo.js:22:31
            at Object.subscribeToResult (/home/ashburndave/.nvm/versions/node/v10.1.0/lib/node_modules/@angular/cli/node_modules/rxjs/internal/util/subscribeToResult.js:7:45)
            at MergeMapSubscriber._innerSub (/home/ashburndave/.nvm/versions/node/v10.1.0/lib/node_modules/@angular/cli/node_modules/rxjs/internal/operators/mergeMap.js:75:38)
            at MergeMapSubscriber._tryNext (/home/ashburndave/.nvm/versions/node/v10.1.0/lib/node_modules/@angular/cli/node_modules/rxjs/internal/operators/mergeMap.js:72:14)
        ashburndave@dphnuc4:/tmp/myng6app$ 

But if I issue the commands below, everything works without any problems

        npm install
        ng serve

