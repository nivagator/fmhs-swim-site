# guide to making updates

## meets

to add or remove a meet, it must be done in three places:
- data/meets.json
- layouts/shortcodes/calendar.html
- content/meets/{meet hame}.md

## albums/photos

## publish process
- `hugo` or `hugo --cleanDestinationDir`
- verify site has built correctly. there are times when subdirectories of the public dir will not clear and this seems to break hugo's build. 
  - manually deleting or clearing the public dir and running `hugo` again will force a full rebuild.
- `rsync --rsync-path "sudo -u {user} rsync" -avz --delete public/ {user}@{server}:/dest/dir/html/`