---
layout: post
maintitle: Meteor production deploy
subtitle: setting external mongo db
---

## What issuse

Setting external mongo db & meteor production deploy

## How to study

```
apt-get install mongodb-server

netstat -ln | grep -E '27017|28017'

cd /etc/cron.d/

vi mongodb-backup

@daily root mkdir -p /var/backups/mongodb; mongodump --db groov --out /var/backups/mongodb/$(date +'\%Y-\%m-\%d')

cd groov

sudo MONGO_URL=mongodb://localhost:27017/groov meteor run --port 80 --production > test.log &
```

## Additional

check mongo db

```
mongo localhost:27017/groov
```
