## nwn-nwsync-docker
WIP: Should be able to deliver hak content now.

## MAKE SURE YOU ONLY HAVE ONE MODULE FILE IN "server/modules/"

nwnxee version will be put into urothis/nwnxee-template

## Usage
"docker-compose up caddy"

This will spin up the required webserver for nwsync to generate manifest and files.

'You can safely disconnect from that terminal using ctrl-z'

"./nwnsnc.sh" should work on linux

Once nwsync has pulled the manifest, and files it needs to deliver the content. 

"docker-compose up nwnxee-server"

## Normal usage

Once files are in place and you want to restart everything.
'docker-compose down'
and 
'docker-compose up' 

Should be what you use in your normal testing routine.

## Windows

Need assistance

Currently there is a bat file in the root of the folder that does not work.
The binaries in var/www/nwsync is also linux binaries.

My plan is to wrap nwsync into a docker container so we can remove this complication. 