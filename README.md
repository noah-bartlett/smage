# smage
Just a little bash tool I made to help manage btrfs snapshots

Smage (snapshot mage)

This is a simple tool that will help manage snapshots in btrfs with default structure

The tool creates snapshots of home, pkg and root depending on flags and has an auto cleanup feature
that saves limited numbers of files (probably, I don't know what I'm doing lol) with some plans to
make it a little more robust at some point.
names snapshots in a YYYY-MM-DD-HR-MM-SS-(subvolname) structure in the .snapshots folder in your root

put the file in your usr bin to use the command and chmod +x it

anyways, syntax

smage -c
creates a snapshot of home by default
smage -c -p
creates a snapshot of pkg
smage -c -r
same as above but root
smage -c -a
all the above

smage -l
list snapshots

smage -r
rollback (I would probably not trust this right now)

smage --cleanup
automatically cleans up snapshots
1 a year > 1 year old
1 every 2 months > 6 months old
1 a week > 1 week
1 a day anything else

smage -h
help message

not really a programmer, don't know what I'm doing so don't trust this tool with anything important
