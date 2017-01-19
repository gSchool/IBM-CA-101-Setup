# IBM CS 101 Setup

In a new terminal window run the following commands 

- `wget https://raw.githubusercontent.com/gschool/IBM-CA-101-Setup/master/c9-setup.sh`
- `chmod +x c9-setup.sh`
- `./c9-setup.sh`
- `exit'
  - **NB**: Be sure to exit this terminal after running the script. A new terminal is required to pick up the changes made by this script.
- Inside of `~/.gitconfig`, modify the name and email address to match what you use to log into Bluemix
	- type `vi ~/.gitconfig` to edit the file
	- Type `i` to enter insert mode 
	- `ESC` key returns the editor to command mode 
	- See [VI Cheatsheet](http://www.lagmonster.org/docs/vi.html) for more VI commands

## Testing That Everything Was Installed as Expected

In a new terminal window, run the following commands to make sure everything was installed as expected

CloudFoundry
```
$ cf -v
```

Should be `cf version 6.22.2+a95e24c-2016-10-27` or higher

Git
```
git --version
```

Should be `git version 2.10.0` or higher

Node
```
node -v
```

Should be `v6.6.0` or higher

Curl
```
curl --version
```

Should give you a message like

```
curl 7.35.0 (x86_64-pc-linux-gnu) libcurl/7.35.0 OpenSSL/1.0.1f zlib/1.2.8 libidn/1.28 librtmp/2.3
```

http
```
http --version
```

Should be `0.9.9` or higher

Open Whisk
```
wsk -h
```

Should give you a message like

```
usage: wsk [-h] [-v] [--apihost hostname] [--apiversion version] [-i] [-s]
           {action,activation,namespace,package,rule,trigger,sdk,property,list}
           ...

OpenWhisk is a distributed compute service to add event-driven logic to your
apps.
```





