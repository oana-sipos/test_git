git fetch --all --prune && git branch --remote --merged | grep -v -P 'master|develop$' | sed -e 's/\// /g' | xargs -L1 -r git push -d; echo Done cleaning remote branches.

