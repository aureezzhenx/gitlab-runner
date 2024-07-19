# Step #1: Add the Official GitLab Repository
First add the official GitLab Repository using below command
```
curl -L "https://packages.gitlab.com/install/repositories/runner/gitlab-runner/script.deb.sh" | sudo bash
```

# Step #2: Install GitLab Runner on Ubuntu
Run below command to install latest GitLab Runner on Ubuntu 20.04 LTS
```
sudo apt-get install gitlab-runner
```

Commands to Start, Stop and Restart GitLab Runner

```
sudo gitlab-runner start
sudo gitlab-runner stop
sudo gitlab-runner restart
```

# Step #3: Grant sudo Permission to GitLab Runner User

```
gitlab-runner ALL=(ALL:ALL) ALL
```
```
gitlab-runner ALL=(ALL) NOPASSWD: ALL 
```

Output:
```
# Host alias specification

# User alias specification

# Cmnd alias specification

# User privilege specification
root    ALL=(ALL:ALL) ALL
gitlab-runner ALL=(ALL:ALL) ALL

# Members of the admin group may gain root privileges
%admin ALL=(ALL) ALL

# Allow members of group sudo to execute any command
%sudo   ALL=(ALL:ALL) ALL

# See sudoers(5) for more information on "#include" directives:

#includedir /etc/sudoers.d
gitlab-runner ALL=(ALL) NOPASSWD: ALL
```


