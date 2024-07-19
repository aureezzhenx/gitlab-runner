Step #1: Add the Official GitLab Repository

```
curl -L "https://packages.gitlab.com/install/repositories/runner/gitlab-runner/script.deb.sh" | sudo bash
```

Step #2: Install GitLab Runner on Ubuntu

```
sudo apt-get install gitlab-runner
```

Commands to Start, Stop and Restart GitLab Runner

```
sudo gitlab-runner start
sudo gitlab-runner stop
sudo gitlab-runner restart
```

Add the gitlab-runner user in sudoers group and set NOPASSWD as shown below

```
gitlab-runner ALL=(ALL:ALL) ALL
```



