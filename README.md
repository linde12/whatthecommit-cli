# whatthecommit-cli

whatthecommit-cli, or wtc, grabs a random commit message from http://whatthecommit.com and outputs it in the terminal

### Usage

```sh
$ wtc
That last commit message about silly mistakes pales in comparision to this one
$
$ wtc -h
Usage: /path/to/wtc [commit]
$ wtc commit -a
1) -m \'So I hear you like commits ...\'
2) woa!! this one was really HARD!
3) [no message]
4) Corrected mistakes
5) marks
#? 4
[master bff7fac] Corrected mistakes
 1 file changed, 27 insertions(+), 3 deletions(-)
 rewrite wtc (85%)
$
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
