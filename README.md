# restic-systemd_automatic-backup

Just a very simple systemd service for [restic](https://restic.net/).


## Install
 
* Place the systemd.service files [restic-backup.service](https://github.com/LeoWinterDE/restic-systemd_automatic-backup/blob/main/restic-backup.service) and [restic-backup.timer](https://github.com/LeoWinterDE/restic-systemd_automatic-backup/blob/main/restic-backup.timer) in `/etc/systemd/system/`.
- Edit the environment variables like `RESTIC_PASSWORD` in the .service file.
- Run `systemctl daemon-reload`.
- Enable the timer `systemctl enable restic-backup.timer`.
