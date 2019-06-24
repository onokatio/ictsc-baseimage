# ictsc baseimage ansible play book

curl -sS -H "Authorization: token $key" https://api.github.com/teams/3300293/members|jq -r .[].login|while read line;do curl -sS "https://github.com/${line}.keys";done > keys
