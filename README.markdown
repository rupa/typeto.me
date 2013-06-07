typeto.me
---------

typeto.me is a character-level realtime chat, like the old talk program on Unix
and Unix-like operating systems.

This is made possible via [socket.io](http://socket.io) and Google's [js diff library](http://code.google.com/p/google-diff-match-patch/).

(C) 2011 Derek Arnold under the MIT License

Derek did all the work; [Daniel](http://3e.org/dmd/) nagged him to do it.

[See it live](http://typeto.me/)

NOTE: Ensure that you are using an up-to-date version of Node.js, socket.io, and ideally, all related modules:

* socket.io
* coffee-script
* eco
* express

Install on Ubuntu 13

    aptitude install git nodejs npm
    git clone <repo>
    cd typeto.me
    npm install express@2.5.11 eco socket.io coffee-script
    nodejs node_modules/coffee-script/bin/coffee -c app.coffee
    cp config.json-dist config.json
    nodejs app.js
