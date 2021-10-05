# Ghost Restart
A short script to restart ghost whenever updates are pushed to the main branch of your github repo for [Ghost](https://github.com/TryGhost/Ghost).

## ghost_restart

Restarts ghost using [appleboy's ssh action](https://github.com/appleboy/ssh-action).
 
For the secrets,

  `SSH_HOST` refers to the host IP address/hostname.
  
  `SSH_USER` refers to the user. user@host.ip
  
  `PORT` refers to the port number you connect to your host at.
  
  `PATH_TO_GITHUB_REPO` refers to the folder you have your ghost code hosted. For me, this is different from the root ghost folder.
  
  `PATH_TO_GHOST` refers to the root folder of your ghost install on your server.
  
  `GIT_PULL_SCRIPT` is just `git pull token@github.com/repo`. See this [Stack Overflow answer](https://stackoverflow.com/questions/61447350/automatically-pull-from-remote-using-github-actions) for more details.
  
This was tested on DigitalOcean running Ubuntu 20.04
