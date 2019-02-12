
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

``` 
ellopunk@rabbit-hole:~> sudo zypper addrepo https://download.opensuse.org/repositories/X11:Unity/openSUSE_Tumbleweed/X11:Unity.repo
Adding repository 'Ubuntu Ayatana (openSUSE_Tumbleweed)' ................................................................................................................................................................................................................[done]
Repository 'Ubuntu Ayatana (openSUSE_Tumbleweed)' successfully added

URI         : http://download.opensuse.org/repositories/X11:/Unity/openSUSE_Tumbleweed/
Enabled     : Yes                                                                      
GPG Check   : Yes                                                                      
Autorefresh : No                                                                       
Priority    : 99 (default priority)                                                    

Repository priorities in effect:                                                                                                                                                                                                               (See 'zypper lr -P' for details)
      90 (raised priority)  :  1 repository  
      99 (default priority) : 10 repositories

```

Refresh: 

```
ellopunk@rabbit-hole:~> sudo zypper refresh
Retrieving repository 'Ubuntu Ayatana (openSUSE_Tumbleweed)' metadata ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------[\]

New repository or package signing key received:

  Repository:       Ubuntu Ayatana (openSUSE_Tumbleweed)        
  Key Name:         X11 OBS Project <X11@build.opensuse.org>    
  Key Fingerprint:  B1DA68DE 51949E7B 034237C4 BB1AF233 0F2672C8
  Key Created:      Tue 23 May 2017 05:13:55 PM CDT             
  Key Expires:      Thu 01 Aug 2019 05:13:55 PM CDT             
  Rpm Name:         gpg-pubkey-0f2672c8-5924b423                

```

Attempted install:

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