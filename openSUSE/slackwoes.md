
# [Slack](https://slack.com/downloads/instructions/fedora)

## Attempt number 1

libappindicator seems to be missing with none of my repos seem to be providing it.

```
ellopunk@rabbit-hole:~/Downloads> sudo zypper in slack-3.3.7-0.1.fc21.x86_64.rpm 
[sudo] password for root: 
Sorry, try again.
[sudo] password for root: 
Loading repository data...
Reading installed packages...
Resolving package dependencies...

Problem: nothing provides libappindicator needed by slack-3.3.7-0.1.fc21.x86_64
 Solution 1: do not install slack-3.3.7-0.1.fc21.x86_64
 Solution 2: break slack-3.3.7-0.1.fc21.x86_64 by ignoring some of its dependencies

Choose from above solutions by number or cancel [1/2/c] (c): c

```

### Solution attept number 1

Add unity repo: 

`zypper addrepo https://download.opensuse.org/repositories/X11:UnitUntitled-1y/openSUSE_Tumbleweed/X11:Unity.repo ` 

``` 
ellopunk@rabbit-hole:~/Downloads> sudo zypper install libappindicator
Loading repository data...
Reading installed packages...
'libappindicator' not found in package names. Trying capabilities.
No provider of 'libappindicator' found.
ellopunk@rabbit-hole:~/Downloads> 
```
No luck

*Note:* Removed repo after this attempt

## Attempt number 2

Lets do it live and worry about notifications later?

``` 
ellopunk@rabbit-hole:~/Downloads> sudo zypper in slack-3.3.7-0.1.fc21.x86_64.rpm 
Loading repository data...
Reading installed packages...
Resolving package dependencies...

Problem: nothing provides libappindicator needed by slack-3.3.7-0.1.fc21.x86_64
 Solution 1: do not install slack-3.3.7-0.1.fc21.x86_64
 Solution 2: break slack-3.3.7-0.1.fc21.x86_64 by ignoring some of its dependencies

Choose from above solutions by number or cancel [1/2/c] (c): 2
Resolving dependencies...
Resolving package dependencies...

The following NEW package is going to be installed:
  slack
```

**Help?** Slack is installed and running, however if you were able to do this with out ignoring dependencies please let me know your fix.