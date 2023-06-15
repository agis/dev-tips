### Calculate additions/deletions between two commits

```
$ git log --numstat --pretty="%H" <ref>..<ref> | awk 'NF==3 {plus+=$1; minus+=$2} END {printf("+%d, -%d\n", plus, minus)}'
```

### Exclude paths from various git commands

Use
[pathspec](https://git-scm.com/docs/gitglossary#Documentation/gitglossary.txt-aiddefpathspecapathspec):

```
$ git grep -e return --and -e err --and -e "," --and --not -e "(nil|false|0), " -- ':(exclude)vendor'
```
