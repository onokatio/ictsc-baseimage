**deprecated** This repository moved to https://github.com/ictsc/ictsc-playbooks (provate repository)

# ictsc baseimage ansible play book

```
curl -sS https://raw.githubusercontent.com/ictsc/ictsc-github-member/production/terraform.tfstate | jq '.modules[].resources | keys' | grep github_team_membership.ictsc2019 | sed -e 's/^.*ictsc[0-9]\{4\}-\(.*\)\",/\1/'| while read line;do echo https://github.com/${line}.keys;done > keys
```
