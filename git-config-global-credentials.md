# Config Global Credentials


## Configure your Git username/email
```
git config --global user.name "FIRST_NAME LAST_NAME"
git config --global user.email "MY_NAME@example.com"
```


## Cache Credentials in Mac OS X
```
git config --global credential.helper osxkeychain
```


## Cache Credentials in Ubuntu
```
sudo apt-get install libsecret-1-0 libsecret-1-dev
cd /usr/share/doc/git/contrib/credential/libsecret
sudo make
git config --global credential.helper \
    /usr/share/doc/git/contrib/credential/libsecret/git-credential-libsecret
```


## Cache Credentials in Memory
```
git config --global credential.helper cache
```

By default, Git will cache your password for 15 minutes. To change the default password cache timeout to 1 hour:

```
git config --global credential.helper 'cache --timeout=3600'
```

## Reference
- https://support.atlassian.com/bitbucket-cloud/docs/configure-your-dvcs-username-for-commits/
- https://docs.github.com/en/free-pro-team@latest/github/using-git/caching-your-github-credentials-in-git
- https://stackoverflow.com/questions/5343068/is-there-a-way-to-cache-github-credentials-for-pushing-commits
