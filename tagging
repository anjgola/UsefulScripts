#!/bin/bash

tagname=$1

#Update local
git pull 

#Remove if this tag exists in remote
git push origin :refs/tags/"$tagname"

#Replace the tag to reference the most recent commit
git tag -f "$tagname"

#Push to remove
git push origin master --tags
