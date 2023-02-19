# docker

How it works?

the system is working on demand with local environment + external api to add some new features

poloshell (port:8022) --[command]--> (port:80) apicontext --[text2botreck]--> botreck plugin on browser

poloshell (port:8022) --[command]--> apicontext --[text2apidsl]--> (port:22) shell with native commands


## Tech stack
+ fedora os 
+ shell: poloshell to write commands
+ apicontext: convert the commands from poloshell to botreck on browser
+ browser: chromium 
+ browser plugins: botreck 
+ remotedekstop
+ keepass - local passwords


### Automatisation

over browser + keepass passworts + shell commands


## Fedora os

OS on docker with option to connect throughr RDP
fast and is working as default with remote desktop to use it on windows environment




