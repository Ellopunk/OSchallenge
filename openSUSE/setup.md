# Setup

## Issue number 1: KDE Wallet

Not being able to connect to wifi due to the lack go GPG keys.

### Solution number 1

1)Check if you have GPG installed. 

`which gpg`

2)Generate your key pair:

`gpg --gen-key`

*Note* Follow prompts to enter your name and email address.

3)Verify that your key pair has been generated.

`gpg -K`

## Packages need updating

When you do a fresh install best practice is to update. I have been warned by several individuals not to do this through the GUI as it may cause issues on the system.

1)List repositories to ensure you are pulling from Tumbleweed repos.

`zypper lr -u`

```
Results should be something similar to:
     | Alias             | Name              | Enabled | Refresh | URI
 --+-------------------+-------------------+---------+---------+--------------------------------------------------------
 1 | repo-debug        | repo-debug        | Yes     | Yes     | http://download.opensuse.org/tumbleweed/repo/debug
 2 | repo-non-oss      | repo-non-oss      | Yes     | Yes     | http://download.opensuse.org/tumbleweed/repo/non-oss
 3 | repo-oss          | repo-oss          | Yes     | Yes     | http://download.opensuse.org/tumbleweed/repo/oss
 4 | repo-src-non-oss  | repo-src-non-oss  | No      | Yes     | http://download.opensuse.org/tumbleweed/repo/src-non-oss
 5 | repo-src-oss      | repo-src-oss      | No      | Yes     | http://download.opensuse.org/tumbleweed/repo/src-oss
 6 | update            | repo-update       | Yes     | Yes     | http://download.opensuse.org/update/tumbleweed/
```

2)Run your upgrade:

`sudo zypper dup`

*Note* zypper dub is shorthand for zypper dist-upgrade 
