# Easily made mistakes that (almost) happened to me explained, to save you some trouble

## Blanc White Page when trying to access the App in the Browser

Look into your network logs in you browser. If there is a 504 error, try to hard reload
the page. Incognito mode should also work.

This is caused when the browser cache holds old versions of Vite files. Clearing the 
cache gets rid of this.

## Delete your volumes before cloning the repository again

Compose uses the name of your folder for the project name. This causes it to assume you want
to use the exact same Postgres Volume from before. Postgres also saved the the password from 
the very first time it was started and ignores any new POSTGRES_PASSWORD variables.
The Backend tries to connect with the new password, which Postgres won't allow.

Solution:

Since the cloned project has the same name as the old one you can run `docker compose down -v`
from your project root. Although you need to set the password for the old Postgres DB again with
`read -rs "POSTGRES_PASSWORD?Enter Password:" && printf "\n" && export POSTGRES_PASSWORD`

## Bash vs zsh

The README of mtg-commander-stats uses bash. If you are on zsh like me, you need to check
some commands for compatibility. This Handbook uses zsh because I use zsh locally, the README
is written in Bash because it is the standard for Linux and CI usage. 

README (Bash): `read -r -s -p 'Local PostgreSQL password: ' POSTGRES_PASSWORD`
Handbook (zsh): `read -rs "POSTGRES_PASSWORD?Local PostgreSQL password:"`