# whatthecommit-cli

whatthecommit-cli, or wtc, grabs a random commit message from http://whatthecommit.com and outputs it in the terminal

### Usage

```sh
$ git commit -m "$(wtc)"
```

### Installation
If you want `wtc` to be reachable from anywhere make sure to include it in your PATH variable.

All you've got to do is to change permission of the `wtc` file.

```sh
$ git clone https://github.com/linde12/whatthecommit-cli.git
$ cd whatthecommit-cli
$ chmod +x wtc
```

If you're running bash you can add `wtc`to your .bashrc by doing:

```sh
$ echo 'export PATH=$PATH:/path/to/wtc'  >> ~/.bash_profile
```
License
----

MIT
