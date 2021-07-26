# TERMINAL
- Format command line to show only current directory

`PS1='${debian_chroot:+($debian_chroot)}\[\033[01;32m\]\u@\h\[\033[00m\]:\[\033[01;34m\]\W\[\033[00m\]\$ '
`
# DOCKER
- list IPs of all running containers

`sudo docker inspect -f '{{.Name}} - {{range .NetworkSettings.Networks}}{{.IPAddress}}{{end}}' $(sudo docker ps -aq)`

- kill all running containers

`docker kill $(docker ps -q)`

- delete all stoped containers
