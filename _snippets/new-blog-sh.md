---
layout: post
title: new-blog.sh
---

```bash
NOW=$(date '+%Y-%m-%d')
TITLE=$1
TITLE_UNDERSCORE=${TITLE// /_}
FILE="${NOW}-${TITLE_UNDERSCORE}.md"

if [ -f $FILE ]; then
  echo "Blog post already exists"
else
  echo "---" >>$FILE
  echo "layout: post" >>$FILE
  echo "title: ${TITLE}" >>$FILE
  echo "---" >>$FILE
  $EDITOR $FILE
fi

```
