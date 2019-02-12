# GitHub GPG

## Configuring use of key

1)List GPG keys

`gpg --list-secret-keys --keyid-format LONG`

2)Set GPG signing key.

`git config --global user.signingkey` <ID>

3)To add your GPG key to your bash profile, paste the text below:

`test -r ~/.bash_profile && echo 'export GPG_TTY=$(tty)' >> ~/.bash_profile`
`echo 'export GPG_TTY=$(tty)' >> ~/.profile`

*Note* This file was made to test GPG signing.