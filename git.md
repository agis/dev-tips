### Calculate additions/deletions between two commits

```
$ git log --numstat --pretty="%H" <ref>..<ref> --author Agis | awk 'NF==3 {plus+=$1; minus+=$2} END {printf("+%d, -%d\n", plus, minus)}'
```
