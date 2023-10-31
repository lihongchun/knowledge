
### git 代码量统计
``
git log --since="2022-07-01" --before="2023-01-01" --author="lihongchun02" --pretty=tformat: --numstat | awk '{ add += $1; subs += $2; loc += $1 - $2 } END { printf "added lines: %s, removed lines: %s, total lines: %s", add, subs, loc }
``