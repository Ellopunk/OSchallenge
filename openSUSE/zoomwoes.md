# Zoom woes

1) [Download Zoom rpm](https://zoom.us/download)

2) Import Key 

`rpm --import package-signing-key.pub`

```
ellopunk@rabbit-hole:~/Downloads> sudp zypper in zoom_openSUSE_x86_64.rpm 
If 'sudp' is not a typo you can use command-not-found to lookup the package that contains it, like this:
    cnf sudp
ellopunk@rabbit-hole:~/Downloads> sudo zypper in zoom_openSUSE_x86_64.rpm 
Loading repository data...
Reading installed packages...
'_tmpRPMcache_:srcpackage:zoom=0:2.7.162522.0121_openSUSE-1' not found in package names. Trying capabilities.
No provider of '_tmpRPMcache_:srcpackage:zoom=0:2.7.162522.0121_openSUSE-1' found.
ellopunk@rabbit-hole:~/Downloads> sudo rpm -i zoom_openSUSE_x86_64.rpm 
warning: zoom_openSUSE_x86_64.rpm: Header V4 RSA/SHA1 Signature, key ID 61a7c71d: NOKEY
error: Failed dependencies:
        libxcb-xtest.so.0()(64bit) is needed by zoom-2.7.162522.0121_openSUSE-1.x86_64
        ibus is needed by zoom-2.7.162522.0121_openSUSE-1.x86_64
        ibus-m17n is needed by zoom-2.7.162522.0121_openSUSE-1.x86_64

```

Issue with installing missing packages
```
ellopunk@rabbit-hole:~/Downloads> sudo rpm -i zoom_openSUSE_x86_64.rpm 
error: Failed dependencies:
        libxcb-xtest.so.0()(64bit) is needed by zoom-2.7.162522.0121_openSUSE-1.x86_64
        
ellopunk@rabbit-hole:~/Downloads> sudo zypper install  libxcb-xtest.so.0
Loading repository data...
Reading installed packages...
'libxcb-xtest.so.0' not found in package names. Trying capabilities.
'libxcb-xtest0-32bit' providing 'libxcb-xtest.so.0' is already installed.
Resolving package dependencies...

Nothing to do.
ellopunk@rabbit-hole:~/Downloads> sudo rpm -i zoom_openSUSE_x86_64.rpm 
error: Failed dependencies:
        libxcb-xtest.so.0()(64bit) is needed by zoom-2.7.162522.0121_openSUSE-1.x86_64
```