## nwn-nwsync-docker
WIP: Should be able to deliver hak content now.

## MAKE SURE YOU ONLY HAVE ONE MODULE FILE IN "server/modules/"

nwnxee version will be put into urothis/nwnxee-template

## Usage
Spin up the docker compose, then run the sh/bat script.

"./nwnsnc.sh" should work on linux




Once nwsync has pulled the manifest and files it needs to deliver the content. 

"docker-compose down"

modify the nwserver.env file to

NWN_NWSYNCURL=1

Once that is saved,

"docker-compose up"


## Windows

Need assistance

Currently there is a bat file in the root of the folder that does not work.
The binaries in var/www/nwsync is also linux binaries.

My plan is to wrap nwsync into a docker container so we can remove this complication. 