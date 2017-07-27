## git-diff-highlight

##### A tool from [here](http://theunixtoolbox.com/git-diff-highlight/), so you need see [it](http://theunixtoolbox.com/git-diff-highlight/) only, this just for record


#### Install

##### Perhaps you can't put it in `/usr/bin` at `MacOs`, because after the `MacOs V10`, system prevent the user edit it for safe, so need add the `$PATH[at the path: /etc/paths]` for other path or put in the `/usr/local/bin`

###### Get a copy of the script and put it somewhere in your `$PATH`

```
curl https://raw.githubusercontent.com/seaRecord/git-diff-highlight/master/diff-highlight > /usr/local/bin/diff-highlight

chmod +x /usr/bin/diff-highlight
```

#### Usage


###### Directly use as this:

```
 git diff --color | diff-highlight
```
###### Or like this if you use frequently

```
// edit the config file [~/.gitconfig] and add:

[core]
  pager = diff-highlight | less -r

```

```
// of course, you can add the alias in the config file

[alias]
    worddiff = !git diff --color | diff-highlight | less -r

```
