Install dconf and try the command below

dconf dump / > full-backup

If it doesn't work, try with -f flag. If you only want gnome related settings try this

dconf dump /org/gnome > gnome-backup

If you use custom theme and icon, backup those separately.

Restore
Full restore dconf load / < full-backup

Gnome only restore dconf load /org/gnome < gnome-backup
